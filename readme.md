# openstack-validate
## Quick Start
```
$ sudo snap install openstack-validate --channel yoga/stable

$ source admin.novarc

# Create the initialization script and feed it to bash.
# Which will:
#
# Install necessary snaps
# Initialize a tempest workspace in myworkspace directory
# Create testing resources on the cloud
# Configure tempest
$ openstack-validate myworkspace | bash
...
2023-07-04 15:43:08.086 2609465 INFO config_tempest.constants [-] Creating configuration file /home/miles/repo/snap-openstack-validate/myworkspace/etc/tempest.conf
########################################################
#
# A tempest workspace is set up at myworkspace
#
# Quick Start:
# cd myworkspace
# tempest run --load-list smoke
########################################################


# Go ahead and follow the advice
cd myworkspace
tempest run --load-list smoke
```
