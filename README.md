# Get up and running

## 1. Install Vagrant
https://www.vagrantup.org/

## 2. Install berkshelf
```bash
$ vagrant plugin install vagrant-berkshelf
$ bundle
```

## 3. Install Digital Ocean Provider

Installation of the provider requires two steps:

```bash
$ vagrant plugin install vagrant-digitalocean
$ vagrant box add digital_ocean https://github.com/smdahlen/vagrant-digitalocean/raw/master/box/digital_ocean.box
```

## 4. Install chef cookbooks
```bash
$ berks install
```

## 5. Build the VM
```bash
$ vagrant up
```

# Usage

To login to the VM run:

```bash
$ vagrant ssh
```

When you are done, exit the VM and run the following command to suspend it until later.

```bash
$ vagrant suspend
```

Resume work at anytime:

```bash
$ vagrant up
```
