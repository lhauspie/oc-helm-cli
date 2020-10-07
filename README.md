# oc-helm-cli
Docker image with Openshift CLI and Helm CLI


## Usage 

This image take 3 args : 
* OC_CLI_VERSION : Openshift target version (ex: 3.10.0) 
* OC_CLI_SHORTSHA : Openshift target version short sha tag commit (ex: dd10d17)
* HELM_VERSION : Helm target version (ex: 2.13.1)

You will find openshift cli versions [there](https://github.com/openshift/origin/releases)

### Example
```bash
docker build . --build-arg HELM_VERSION=2.13.1 --build-arg OC_CLI_VERSION=3.10.0 --build-arg OC_CLI_SHORTSHA=dd10d17
```
