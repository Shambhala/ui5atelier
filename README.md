# NodeJS on Kubernetes

## Project Structure

The _vagrantfile_ This is file for creating the docker kubernetes environment at non-unix environments such as Windows OS.

```ruby
# -*- mode: ruby -*-
# vi: set ft=ruby :
# Specify minimum Vagrant version and Vagrant API version
Vagrant.require_version '>= 1.6.0'
VAGRANTFILE_API_VERSION = '2'

# Require 'yaml' module
require 'yaml'

# Read YAML file with VM details (box, CPU, and RAM).
# The Configuration file contains the Azure, AWS details
config = YAML.load_file(File.join(File.dirname(__FILE__), 'config.yml'))

unless Vagrant.has_plugin?("vagrant-some-plugin")
  raise 'some-plugin is not installed!'
end

# Create and configure the VMs
Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|


# Install Minikube
curl -Lo minikube https://storage.googleapis.com/minikube/releases/v0.12.2/minikube-linux-amd64 && chmod +x minikube && sudo mv minikube /usr/local/bin/
end
```

## Container Features

It allows to scale at the Process Level

Kubernetes(K8s) is open source system for automating and managing container orchestration. Kubernetes has a master-node based architecture which enables rapid, horizontal scaling.

*   _Pod:_
*   _Node:_
*   _Service:_
*   _ReplicaSet:_
*   _Deployment:_
*   _Namespace:_

_Minikube_ is a tool that makes it easy to run kubernetes locally

## Setup Babel



## Setup UI5 project
ui5loader

/sapui5/resources/uiloader.js
/sapui5/resources/uiloader-autoconfig.js
_sap.ui.define()_
_sap.ui.require()_

*   [You don't know openui5 Bootstrapping](https://blogs.sap.com/2017/12/27/you-dont-know-openui5-bootstrapping/)
* [You don't know openui5 App and Pages ](https://blogs.sap.com/2018/01/01/you-dont-know-openui5-app-and-pages/)
* (https://blog.scottlowe.org/2018/06/08/quadruple-provider-vagrant-environment/)
