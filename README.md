# Overview

This is a Canonical juju charm used to bring up iron-io/functions, an Open
Source FaaS solution.

This is a precursor to creating a juju charm for Openstack Picasso, as it also
uses iron-functions.

# How to install/test

Currently this is not tested as per framework, it is pretty much - modify, run, debug, repeat.

This is how you can build it
```
charm build
juju bootstrap localhost
juju deploy ./trusty/iron-functions --series trusty
juju debug-log
```
After it has crashed and you know what to fix run `juju kill-controller localhost-localhost`

Remember to check the [icon guidelines][] so that your charm looks good
in the Juju GUI.

# Contact
Feel free to email me at phkaznowski ([<at<[[( gmail )]]>> Funky formatting to avoid bots

## Upstream Project Name

The functions service can be found at https://github.com/iron-io/functions

The functions website can be found at https://www.iron.io/

NOTE I am not affiliated with iron-io or functions

Issues are tracked on the github of this project https://github.com/phughk/iron-functions-juju-charm

[icon guidelines]: https://jujucharms.com/docs/stable/authors-charm-icon
