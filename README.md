# local_manifests

To build SlimKAT for the Samsung S3 mini (golden) device,
follow the steps below:

## Setup build tree
Create the directory, which should hold your build tree, 'cd' into it
and run the following commands:
```Shell session
repo init -u https://github.com/SlimRomsSecurity/platform_manifest.git -b kk4.4
cd .repo
git clone https://github.com/MSe1969/local_manifests
cd local_manifests
git checkout kk4.4
cd ../..
repo sync
```

## Start the build
From the 'top directory' of your build tree, execute the following commands:
```Shell session
source build/envsetup.sh
brunch golden
```
