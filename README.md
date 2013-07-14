# Get up and running

## 1. Install Vagrant and plugins
https://www.vagrantup.org/
```bash
$ vagrant plugin install vagrant-berkshelf
$ vagrant plugin install vagrant-digitalocean
```

## 2. Install berkshelf
```bash
$ bundle
```

## 3. Install chef cookbooks
```bash
$ berks install
```

## 4. Build the VM
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
