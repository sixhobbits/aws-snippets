# aws-snippets
Some reusable AWS-related code, mainly to stop me making the same mistakes over and over and over...

## User Data scripts
This sets up an Ubuntu instance with some Python libraries. 

```
#!/bin/bash
export LC_ALL="en_US.UTF-8"
apt update
apt install -y python3 python3-pip
pip3 install pip --upgrade --force-reinstall
pip3 install numpy scipy matplotlib jupyter sklearn awscli requests
```
