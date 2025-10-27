Every function is important, but some are more important then others! This file will explain some of the most important functions and endpoints in the pwn.college DOJO.

### /workspace: generate iframe urls

location: [/dojo_plugin/api/v1/workspace.py](/dojo_plugin/api/v1/workspace.py#L21)

The /workspace endpoint is responsible for generating iframes which will be used for either the `desktop` or the `desktop-windows` services. Let's break it into parts:

##### Get arguments
```
user_id = request.args.get("user")
password = request.args.get("password")
service = request.args.get("service")
```
This part just get the user id, the password and the service from the request.
