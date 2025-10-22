# ns8-unifi-network

This is the NS8 implementation of the [Unifi Network Application](https://hub.docker.com/r/linuxserver/unifi-network-application)

## Install

Instantiate the module with:

    add-module ghcr.io/mrmarkuz/unifi-network:latest 1

The output of the command will return the instance name.
Output example:

    {"module_id": "unifi-network1", "image_name": "unifi-network", "image_url": "ghcr.io/nethserver/unifi-network:latest"}

## Configure

Setup the FQDN in the NS8 app settings and browse to `http://<FQDN>`

You need to create a Unifi account to be able to login and pass a 2FA validation via mail.

## Notes

If you want to connect to your Network Application from the Unifi web page and get the message "Connecting to Site is taking longer than expected ...", check [this page](https://community.ui.com/questions/Connecting-to-site-is-taking-longer-than-expected/70b5bd50-6935-4d54-bc6a-79b744214374) for a solution.

In Chromium it worked after the message, in Firefox it didn't. The local connection always worked.

## Uninstall

To uninstall the instance:

    remove-module --no-preserve unifi-network1