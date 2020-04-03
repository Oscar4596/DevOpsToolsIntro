# Virtualization

The easy way to mount virtual machines is vagrant, you can read more information [here](https://www.vagrantup.com/intro/index.html)

[Here](https://www.vagrantup.com/intro/getting-started/install.html) you can check how to install Vagrant.

Vagrant uses a `Vagrantfile` to know how to create the virtual machine.

You can create a basic `Vagrantfile` with
```
$ vagrant init
```

I recommend to create a directory before, so you create the `Vagrantfile` inside a new directory.

This is a basic `Vagrantfile` using a ubuntu box. To know more about boxes clic [here](https://www.vagrantup.com/intro/getting-started/boxes.html)

Copy this Vagrant file and save it as `Vagrantfile`
`Vagrantfile`:
```
Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/xenial64"
  config.vm.network "forwarded_port", guest: 8080, host: 8080, host_ip: "127.0.0.1"
end
```
And then run 

```
$ vagrant up
```

Once the VM is up run
```
$ vagrant ssh
```
To get into the machine

And that's it.

[Index](index.md)
