# ns8-unifi-network

This is the NS8 implementation of the [Unifi Network Application](https://hub.docker.com/r/linuxserver/unifi-network-application)

## Install

Instantiate the module with:

    add-module ghcr.io/mrmarkuz/unifi-network:latest 1

The output of the command will return the instance name.
Output example:

    {"module_id": "unifi-network1", "image_name": "unifi-network", "image_url": "ghcr.io/nethserver/unifi-network:latest"}

## Configure

Enter the FQDN and browse to `http://<FQDN>`

## Uninstall

To uninstall the instance:

    remove-module --no-preserve unifi-network1