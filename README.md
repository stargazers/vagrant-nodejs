# Vagrant box for NodeJS development

## Requirements

This Vagrantbox uses Ansible, so make sure you have it installed.

In MacOSX you can install it like this:

    sudo easy_install pip
    sudo pip install ansible

**NOTE** This box uses network configurations which will work on my WLAN and
on my computer, but propably not on others! Make sure you will update
network settings of the box!

## Starting the box

Just type:

    vagrant up

When box is up and running, you can go there with:

    vagrant ssh
