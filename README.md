OpenDroneMap

---

* Easy to use computer vision software for civilian drones and more

---

Download and install VirtualBox, Vagrant, and MeshLab

* VirtualBox: https://www.virtualbox.org/
* Vagrant: http://www.vagrantup.com/
* http://meshlab.sourceforge.net/­

---

If you are a Windows user, please also install Putty and github for windows:

* http://tartarus.org/%7Esimon/putty-snapshots/x86/putty-installer.exe
* https://windows.github.com/

If a Mac user, install github for Mac:

* https://mac.github.com/

---

Now clone the Vagrant machine repository, and start up:

```SHELL
git clone https://github.com/OpenDroneMap/odm.git
cd odm
vagrant up
vagrant ssh #(for windows users see http://stackoverflow.com/questions/9885108/ssh-to-vagrant-box-in-windows)
```

---

Now, on the host machine (not our shiny new Ubuntu machine) copy BundlerTools.zip to our odm directory.  This will appear in the /vagrant/ directory on our Ubuntu Virtual Machine.

---

Copy and unzip the directory to our VM from within the VM.
If you are not logged in, then:
`vagrant ssh`

otherwise
```SHELL
cp /vagrant/BundlerTools.zip ~/.
unzip BundlerTools.zip
cd BundlerTools
```

---

Let's run a test dataset.

```SHELL
cd ~/BundlerTools/bundler-v0.4-source/examples/kermit
~/BundlerTools/./run.pl
```

---

Go get a cup of coffee.

![](http://i.imgur.com/8cK0aVj.gif)

---



---
