# oci-x11-hook

A simple experiment to demonstrate how to create OCI hooks.

## Dependencies

* jq available in the host
* xauth-based X cookie

## Install

1. Copy the `oci-x11-hook` program to the host (e.g. `/usr/local/bin`)
2. Copy the `x11.json` file to a hooks directory and adjust the path to the program

## Running

    podman run --rm --hooks-dir /path/to/hooks.d --env DISPLAY --env XAUTH=$XAUTHORITY --net host gns3/xeyes
