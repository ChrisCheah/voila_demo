
# Getting Started
## Setting Up
``` shell
git clone https://github.com/ChrisCheah/voila-demo.git
cd voila-demo
python -m venv env
env\Scripts\activate.bat
```
## Build & Run
``` shell
pip install -r requirements.txt
voila
```

### Define a manifest file (optional)
Add manifest.yml in the root directory with the following content
``` yaml
---
version: 1
applications:
    - name: voila-dmeo
      random-route: true
      memory: 64M
      buildpacks: 
        - https://github.com/cloudfoundry/python-buildpack.git
```

### Steps:
``` shell
cf push
```

