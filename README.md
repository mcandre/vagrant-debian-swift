# vagrant-debian-swift: a Vagrant box for building Swift binaries for GNU/Linux (Debian)

# DISCLAIMER

The Swift programming language is currently not available in the official Debian repositories, and the "swift" package name is currently reserved for a database unrelated to the Swift language.

# VAGRANT CLOUD

https://app.vagrantup.com/mcandre/boxes/vagrant-debian-swift

# EXAMPLE

```console
$ cd test
$ vagrant up
$ vagrant ssh -c "cd /vagrant && swiftc -o hello Hello.swift && ./hello"
...
```

# RUNTIME REQUIREMENTS

* [Vagrant](https://www.vagrantup.com)
* The [VirtualBox](https://www.virtualbox.org) hypervisor provider

## Recommended

* [vagrant-rsync-back](https://github.com/smerrill/vagrant-rsync-back) assists in copying artifacts from the guest to the host

# BUILDTIME REQUIREMENTS

* [Vagrant](https://www.vagrantup.com)
* The [VirtualBox](https://www.virtualbox.org) hypervisor provider
* [make](https://www.gnu.org/software/make/)

# EXPORT

```console
$ make vagrant-debian-swift.box
```
