# Chart: Rapid Response

All notable changes to this chart will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

Please note that it's automatically updated vía github actions.
Manual edits are supported only below '## Change Log' and should be used
exclusively to fix incorrect entries and not to add new ones.

## Change Log
# v0.4.5
### Bug Fixes
* **rapid-response** [ad996c4](https://github.com/sysdiglabs/charts/commit/ad996c432eca3c68ad41e2d41566c513919259db): update chart version ([#909](https://github.com/sysdiglabs/charts/issues/909))
## v0.4.5
### Minor changes
* bump image tag to 0.3.8
# v0.4.4
### New Features
* **rapid-response,sysdig-deploy** [6158dda](https://github.com/sysdiglabs/charts/commit/6158dda036e90e8493d002b3501479ade32b48c1): Verify that image.tag is a string ([#894](https://github.com/sysdiglabs/charts/issues/894))
# v0.4.3
### New Features
* **agent,node-analyzer,rapid-response** [487b421](https://github.com/sysdiglabs/charts/commit/487b421c922e097047e5ca65c01cee466664daba): add Rancher-specific tolerations ([#884](https://github.com/sysdiglabs/charts/issues/884))
# v0.4.2
### Documentation
* **rapid-response** [02e4b0e](https://github.com/sysdiglabs/charts/commit/02e4b0eefc19767ffc4bdfcaad6724a602c2ba37): Removed extra ']' ([#881](https://github.com/sysdiglabs/charts/issues/881))
# v0.4.1
### Documentation
* **rapid-response** [2056b2b](https://github.com/sysdiglabs/charts/commit/2056b2b7678d178c9adf04e138cdd44e1bd6af87): Added some examples ([#880](https://github.com/sysdiglabs/charts/issues/880))
# v0.4.0
### New Features
* **rapid-response** [eb1d4c8](https://github.com/sysdiglabs/charts/commit/eb1d4c8442834e99984e397e3f93caf641c88816): Introduced the possibility of specifying a Service Account ([#879](https://github.com/sysdiglabs/charts/issues/879))
# v0.3.6
### Documentation
* **rapid-response** [21d07d8](https://github.com/sysdiglabs/charts/commit/21d07d8c09b38f9033891ba1d02ce59ae5fde8e6): Updated Rapid Response ([#878](https://github.com/sysdiglabs/charts/issues/878))
# v0.3.5
### Documentation
* **rapid-response,sysdig-deploy** [9b7cb32](https://github.com/sysdiglabs/charts/commit/9b7cb32e2c51141d74a05f2aa9bfd03babb782c4): Updated rapid-response doc ([#865](https://github.com/sysdiglabs/charts/issues/865))
# v0.3.4
### New Features
* [f4cb189](https://github.com/sysdiglabs/charts/commit/f4cb189afba6833fd458f99dcfcc0121f9d9dfa2)]: unify changelog headers ([#787](https://github.com/sysdiglabs/charts/issues/787))

## v0.3.3
### Minor changes
* Add deployment test to rapid response chart

## v0.3.2
### Minor changes
* Updated chart icon

## v0.3.1
### Minor changes
* Added `node-role.kubernetes.io/control-plane` toleration

## v0.3.0
### Major changes
* Added support to custom CA certificates
### Bugfix
* Fixed missing tolerations, this was preventing Rapid Response to be deployed on control plane nodes

## v0.2.10
### Minor changes
* Updated override helm tests to include extra testcases.

## v0.2.9
### Minor changes
* Readme changes to indicate helm unit testing.

## v0.2.8
### Minor changes
* Added golden template tests

## v0.2.7
### Minor changes
* Added unit tests for testing labels

## v0.2.6
### Minor changes
* bump image tag to 0.3.6

## v0.2.5
* Added unit tests to check local overrides of global values

## v0.2.4
### Minor changes
* bump image tag to 0.3.5

## v0.2.3
### Minor changes
* Add aroberts87 to chart maintainers

## v0.2.2
### Minor changes
* bump image tag to 0.3.4

## v0.2.1

### Minor changes

* Removed trailing spaces

## v0.2.0

### Major change

* Deprecated the usage of `skipTlsVerifyCertificate`, for enabling/disabling the certificate verification use `sslVerifyCertificate` instead
For compatibility purposes `skipTlsVerifyCertificate` is still available in this release

## v0.1.1

### Bugfix

* Fixed an issue that was causing k8s secrets to get generated with uppercase characters

## v0.1.0

### First release

* Deploy only Sysdig Rapid Response daemonset and associated resources
* Use global common values for access key
