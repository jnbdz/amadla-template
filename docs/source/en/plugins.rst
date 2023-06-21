Plugins
=======

Amadla is made to be as none-opinionated as possible.

For example if you want to use something different than Terraform for defining your infrastructure, you can write a plugin for it.

Or you want to use other template engines than Jinja2, you can also write a plugin for it.

Already tools like Terraform, Ansible, Packer can be used to call other tools, Amadla can also be used to call other tools.

The same for the rest of the configurations you can use it for any cloud service, server OS, container system, etc that you want.

The purpose of Amadla is to make it easy to use all these tools together and you manage your configurations with the tools that you want.

Plugin Types
------------

There are 3 types of plugins:

* **Template Engine** - Used to render templates
* **Provisioner** - Used to provision the server (e.g.: Packer)
* **Deployer** - The commands that are called to deploy