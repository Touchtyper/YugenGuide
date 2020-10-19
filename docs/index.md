# Yugen: Getting Started

This guide will take you through deploying your app to the Yugen PaaS platform for the first time.

## 1. Setting up your application

Yugen uses Git to manage version control and deploy your application to the platform. As such, it's necessary to add a Git remote to tell Git where to deploy your application. This can be done simply using our Setup Script found [here](https://www.dropbox.com/s/ot8ag7hnesrni6z/YugenBetaScript.sh?dl=1)

Before you can run this script you'll need to make it executable:

```
$ chmod +x YugenBetaScript.sh
```

You can then run it like so:

```
$ ./YugenBetaScript.sh 
```

The script will guide you through adding the git remote and will allow you to deploy your app for the first time, if you wish. You'll need to know your Yugen application name (given in signup) and the location of your project locally.

All further deployments to the platform can be achieved using a simple git push command:

```
$ git push yugen master
```

## 2. Installing the Yugen CLI

For remote management of your app in production you'll want to use the Yugen CLI. This utility will allow you to stop and start your application, view logs, and set environmental variables. The Yugen CLI is a ruby gem and can be install using the command:

```
$ gem install yugen
```
*Note: you may have to use sudo.*

Typing ` yugen help ` will display all possible commands.

**If you have any other questions about Yugen or issues with getting up and running send us an email at support@yugen.app** 

Thanks for joining the PaaS revolution :) - Henry
