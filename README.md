Description
===========

DeployButton.com is a service that makes it easy to trigger deploys.

It works particularly well with Chef, especially if you want your Chef server synchronized with your repository.


Requirements
============

none


Attributes
==========

- deploy_button_project: project url. set this to the url string for your deploy button project (e.g. "http://deploybutton.com/p/o5r2cgamqhwaabmwluse/")


Usage
=====

Put `recipe[deploy_button]` in your run list.

On your node, set the attribute "deploy_button_project"

    override_attributes({
      "deploy_button_project" => "http://deploybutton.com/p/o5r2cgamqhwaabmwluse/"
    })


Running chef-client will register itself and allow you to use DeployButton.com to trigger deploys.


License and Author
==================

Author:: Jacques Crocker (<jacques@lizibot.com>)

Copyright:: 2012, Lizi, Inc

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
