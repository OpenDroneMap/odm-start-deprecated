
OpenDroneMap

---

Easy to use computer vision software for civilian drones and more.

---

Download and install VirtualBox, Vagrant, and MeshLab

* VirtualBox: https://www.virtualbox.org/
* Vagrant: http://www.vagrantup.com/
* http://meshlab.sourceforge.net/­

---

If you are a Windows user, please also install GitHub for windows:

* https://windows.github.com/

If a Mac user, install GitHub for Mac:

* https://mac.github.com/

---

Now clone the Vagrant machine repository, and start up:

```SHELL
git clone https://github.com/OpenDroneMap/odm.git
cd odm
vagrant up
vagrant ssh 
```
(for Windows users-- run this in your Git Shell)

---

otherwise
```SHELL
cd
git clone https://github.com/OpenDroneMap/BundlerTools.git
```

This will take a while-- it's a 500MB repo...

```SHELL
cd ~/BundlerTools
./install.sh
```

---

Let's run a test dataset.

```SHELL
cd ~/BundlerTools/src/bundler/examples/kermit
~/BundlerTools/./run.pl
```

---

Go get a cup of coffee.

![](http://i.imgur.com/8cK0aVj.gif)

---

Once complete, we should have some extra directories created. Since we specified no parameters, we get the following by default:

```
reconstruction-with-image-size-1200
reconstruction-with-image-size-1200-results
```

---

To view, we open MeshLab on our host machine. We'll need to copy these to a location available to our host machine:

```SHELL
cp ~/BundlerTools/src/bundler/examples/kermit/reconstruction-with-image-size-1200-results/option-0000.ply /vagrant/.
```

These will be in our original odm directory, e.g.

c:\Users\yourusername\Documents\GitHub\odm\option-0000.ply

---

Open MeshLab, choose File:Import Mesh 
and navigate to the directory and choose option-0000.ply

---

To halt vm:
```
exit
vagrant halt

```

---

Photos:

Use a simple point and shoot.
GoPro is a maybe (wide angle could be a problem)
Take lots of overlapping photos.
Also, consult recommendations at:
http://wedidstuff.heavyimage.com/index.php/2013/07/12/open-source-photogrammetry-workflow/

