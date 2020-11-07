# docker-rmi

Have too many docker images on your local docker daemon, and not sure which ones to delete?

Remove docker images with a prompt: Press **y** to delete, and **n** to skip deletion.

## Key Features

- Delete docker images with confirmation. Press **y** to delete, and **n** to skip.
- Images (especially the big ones) gets deleted in the background, so you don't wait, you just move onto the next selection.

## Screencast
[![asciicast](https://asciinema.org/a/371122.svg)](https://asciinema.org/a/371122)

## Wanna try it out!?

```
User: Hey! I don't feel comfortable trying it out on my laptop.
User: I fear docker-rmi will delete some images accidentally.
Me: No worries! just run "vagrant up" and it will spin up an ubuntu 18.04 VM
Me: ..and setup ~20 docker images for you to delete and try it out!
Me: Once the VM is up, just do "vagrant ssh docker-rmi" and "docker-rmi"
Me: Vagrant setup takes ~10 mins, go get a coffee :) while we set things up for you!
User: This is awesome!
```

## Installation

Make sure your **$GOPATH** is setup correctly.

```
$ mkdir -p $GOPATH/src/github.com/shishir-a412ed
$ cd $GOPATH/src/github.com/shishir-a412ed
$ git clone git@github.com:shishir-a412ed/docker-rmi.git
$ cd docker-rmi
$ sudo make install
```

## Verify

```
$ which docker-rmi
$ docker-rmi (This should start the application)
```

## Currently supported environments

macOS Catalina (Version 10.15.5), Ubuntu (>=16.04), Centos, Fedora
