# yocto-docker

macOS compatible version of crops/yocto-dockerfiles. Currently only Ubuntu-22.04 image has been tested. To build the ubuntu-22.04-base and ubuntu-22.04-builder images, run the following:
```
# Export REPO name. This will be the name of the built image.
# You can use crops/yocto if you want to override it
export REPO=ejaaskel/yocto
# Export the disto to be built. This should be one of the
# versioned distros in dockerfiles-folder. Only ubuntu-22.04
# has been tested by me.
export DISTRO_TO_BUILD=ubuntu-22.04
# Run the build script for a single image
./build_container.sh
```

More information on how to use these Docker images and how to build Yocto with Apple Silicon can be found from my blog:
https://ejaaskel.dev/how-to-build-yocto-with-apple-silicon/
