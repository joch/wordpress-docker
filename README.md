# WordPress Docker

WordPress Docker makes developing for WordPress easy and predictable. It
sets up everything for you, so that you can dive straight into developing
your plugins and themes without any hassle.

There in a more in-depth blog post is available called [Develop
WordPress plugins and themes using
Docker](http://johnny.chadda.se/develop-wordpress-plugins-and-themes-using-docker/).

## Getting Started

1. Clone this repostory:
    `git clone --recursive https://github.com/joch/wordpress-docker.git`
1. Copy the provided config file to the WordPress directory:
    `cp wp-config.php wordpress/`
1. Run `docker-compose up` to start the containers.
1. Browse to http://[docker ip]:8000/ and you are ready to go! (find the
   ip using `boot2docker ip`)

## Tmuxp workspace

A predefined workspace is provided to easily get going.

1. Install tmuxp (`sudo pip install tmuxp` on a Mac)
1. Run `tmuxp load tmuxp.yml` (provided that you have tmux installed)
1. A tmux session will be started with a vim window located in the
   plugins directory. The containers are started automatically in the
   second window.

## If you're new to Docker

If you are running `boot2docker`, you can easily find your Docker IP by
running `boot2docker ip`.

The easiest way to install boot2docker and fig is to use
[Homebrew](http://brew.sh) and follow these steps:

1. Install [VirtualBox](https://www.virtualbox.org).
1. Install the software: `brew install boot2docker fig`.
1. Create a virtual machine: `boot2docker init`.
1. Finally start the virtual machine: `boot2docker up`.

## Acknowledgements

The setup is based on the excellent article [Getting started with Fig
and WordPress](http://www.fig.sh/wordpress.html).
