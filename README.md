# drone-config
Configuration files and templates for initial Drone server setup

## Setup

First, pull the relevant docker images.
```docker pull drone/drone-runner-docker:1```
```docker pull drone/drone:1```

Then, copy `env.txt.template` and remove the `.template` from the name.
Given this tutorial: https://docs.drone.io/server/provider/github/ add the relevant values to the env.txt file. Copy the export statements from that file
into your bash_profile (or environment profile file of your choice) and source them into your command line. There are also aliased commands included in the
template, however you have to be in the same directory as your `docker-compose.yml` file for the `start` commands to function properly.

Now, if you are in the same directory as `docker-compose.yml`, you should be able to run `start_drone_server` and `start_drone_runner` and have your drone server
up and running.

