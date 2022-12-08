# scaling-rust-buildpack

Please use multi-buildpack because we need APT to make this work

## Configure your app with multi buildpacks:
```
scalingo env-set BUILDPACK_URL=https://github.com/Scalingo/multi-buildpack
```
## Example of .buildpacks file:
```
https://github.com/Scalingo/apt-buildpack
https://github.com/alaborderie/scalingo-rust-buildpack
```
Note that the order of the buildpacks in the .buildpacks file matters.
