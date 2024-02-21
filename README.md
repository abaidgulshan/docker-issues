# 🔪 Docker Issues and Troubelshooting 🔭
## Docker "less" not installed 
* 🤔  Try to run AWS CLI command inside docker container
* ❌ **error**: `"less" not installed`
* 🎯 **solution**: Check Docker image using and install less, in my case it is Ubuntu so I added following commands to Dockerfile 
    ```
    RUN apt update && apt install less -y
    ```
