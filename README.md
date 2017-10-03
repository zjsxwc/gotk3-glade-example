# Go GTK3 Glade Example

[![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)
[![goreportcard](https://goreportcard.com/badge/github.com/mrccnt/gotk3-glade-example)](https://goreportcard.com/report/github.com/mrccnt/gotk3-glade-example)

Experimenting with go and gtk using [gotk3](https://github.com/gotk3/gotk3) and [glade](https://glade.gnome.org/).

![screenshot](screenshot.png)

## Prerequisites

```bash
    # Install dev dependencies for gtk, cairo and glib
    #
    sudo apt-get install libgtk-3-dev libcairo2-dev libglib2.0-dev
```

## Environment

    Ubuntu 16.04 LTS
    Go 1.8.3
    GTK 3.18

The `install.sh` script makes use of the corresponding gtk build tags.

## Dependencies

We also need to install [glide](https://glide.sh) as package manager.

Install on a per project base:

```bash
    # Make glide available in ./bin directory
    #
    curl https://glide.sh/get | sh
```

Or install via PPA:

```bash
    # Make glide globally available
    #
    sudo add-apt-repository ppa:masterminds/glide
    sudo apt-get update
    sudo apt-get install glide
```
Now install the dependencies:

```bash
    
    # Install dependencies in ./vendor directory
    #
    glide install
    
    # Link dependecies in ./src directory
    # 
    ./link.sh
```

## Run / Build
    
```bash
       
    # Install
    #
    ./install.sh

    
    # Run
    #
    gotk3-glade-example
```
