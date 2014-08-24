docker-compass
==============

A simple docker running Compass inside it. Using  sass='3.4.1', compass='1.0.0.alpha.20' and  susy='2.1.3'


Usage
-----

First build the image:

    docker build -t compass_image github.com/arruda/docker-compass

Then run it:

    docker run -d -v my_compass_project_folder:/home/compass/project compass_image

This will make `compass watch` the folder `my_compass_project_folder`.


### Need to run a compass command?
Then just use it like this:

    docker run -d -v my_compass_project_folder:/home/compass/project compass_image compass <any_command_here>

LICENSE
=============
This software is distributed using MIT license, see LICENSE file for more details.
