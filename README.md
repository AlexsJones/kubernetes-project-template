# Kubernetes-project-template

This project is designed to fast track kubernetes projects
Out of the box you get:

- Per environment deployment settings
- Simple deployment execution
- Helper shell scripts to make it a seamless CI/CD process
- Deployment directory that can be zipped and sent off.

## Requirements

- Golang
- vortex (A golang tool for interpolation) `go get github.com/AlexsJones/vortex`

## Getting started

- Generate an environments file and follow the interpolation syntax `{{.replaceme}}`
with your k8s templates

- Run `./build_environment.sh MYENV` or use the default environment
  Once this command is run, there will be a deploy directory created that matches the file structure of your templates      directory.
- `kubectl create -f deployment/example-deployment`
