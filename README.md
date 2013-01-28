# Intro
vagrant-dns enables easy dns management of multiple local Vagrant machines.


It composed from a Vagrant plugin and standalone dns server, the plugin auto registers the host and ip of the VM once it boots up making it available for lookup on both the host and guest machines.

# Demo
<iframe width="560" height="315" src="http://www.youtube.com/embed/6GFobNDvwpI" frameborder="0" allowfullscreen></iframe>

# Install
 
```bash
  $ sudo aptitude install libzmq1  libzmq-dev
  $ gem install vagrant-dns-server
```

# Usage

Add the plugin to the project Gemfile, use vagrant_dns server to boot the local dns server


# Alternatives

There are two existing project that aim to provide similar functionality:

 * BerlinVagran [vagrant-dns](https://github.com/BerlinVagrant/vagrant-dns) which seems to be able to manage only a single machine and is OSX only.
 
 * [vagrant-hostname](https://github.com/mosaicxm/vagrant-hostmaster) which manipulates /etc/hosts, this requires to enter sudo password for each machine (not an option when starting numerous machines).
