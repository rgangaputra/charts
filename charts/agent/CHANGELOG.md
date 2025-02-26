# Chart: Agent

All notable changes to this chart will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

Please note that it's automatically updated vía github actions.
Manual edits are supported only below '## Change Log' and should be used
exclusively to fix incorrect entries and not to add new ones.

## Change Log
# v1.5.58
### Bug Fixes
* **agent** [a2891bc](https://github.com/sysdiglabs/charts/commit/a2891bc82b2cfef7be5da1d22f39f8b81b05c897): Fix agent.secure.enabled flag ([#858](https://github.com/sysdiglabs/charts/issues/858))
# v1.5.57
### New Features
* **agent,node-analyzer,rapid-response** [487b421](https://github.com/sysdiglabs/charts/commit/487b421c922e097047e5ca65c01cee466664daba): add Rancher-specific tolerations ([#884](https://github.com/sysdiglabs/charts/issues/884))
# v1.5.56
### Bug Fixes
* **agent** [6dcd65e](https://github.com/sysdiglabs/charts/commit/6dcd65ed1bc02e3c6929f0925167e803e820909b): Set agent node selector os and arch by k8s version ([#859](https://github.com/sysdiglabs/charts/issues/859))
# v1.5.55
### Documentation
* **agent,node-analyzer,sysdig,sysdig-stackdriver-bridge** [da18fe5](https://github.com/sysdiglabs/charts/commit/da18fe5e7225be9bbfc484d6dcb22987d7d08066): remove references of the deprecated --purge option for 'helm delete' ([#864](https://github.com/sysdiglabs/charts/issues/864))
# v1.5.54
### Documentation
* **agent,node-analyzer,sysdig** [bd37186](https://github.com/sysdiglabs/charts/commit/bd371864313e64d7a7ac07f79fe30f296b46d540): Remove references to Get Started in the READMEs ([#819](https://github.com/sysdiglabs/charts/issues/819))
# v1.5.53
### Chores
* **agent** [60531e5](https://github.com/sysdiglabs/charts/commit/60531e52a565b8dbf85c385d401e45661cbd54a5): bump agent version to 12.10.1
# v1.5.52
### Bug Fixes
* **agent** [ea56818](https://github.com/sysdiglabs/charts/commit/ea568182894e0803d92a9051bcd500792ee6bee2): Fix agent logPriority rendering ([#824](https://github.com/sysdiglabs/charts/issues/824))
# v1.5.51
### Bug Fixes
* **agent** [751015b](https://github.com/sysdiglabs/charts/commit/751015b713b0bd3a9a738f8e47d72cfe2167e70e): fix region us3 endpoints for agent and sysdig-deploy ([#823](https://github.com/sysdiglabs/charts/issues/823))
* **sysdig,agent** [096d6e4](https://github.com/sysdiglabs/charts/commit/096d6e4d0326f36357fec6ac61342c17e73b33ab): add extra secrets and tests ([#821](https://github.com/sysdiglabs/charts/issues/821))
# v1.5.50
### New Features
* **agent** [7df93a3](https://github.com/sysdiglabs/charts/commit/7df93a38409a902fe5372115bf8c545f84f804e9): add extra secrets ([#813](https://github.com/sysdiglabs/charts/issues/813))
# v1.5.49
### Chores
* **agent** [ede1c8e](https://github.com/sysdiglabs/charts/commit/ede1c8ebcacbf315814a272eb39f68150e1cc979): bump agent version to 12.10.0 ([#815](https://github.com/sysdiglabs/charts/issues/815))
# v1.5.48
### New Features
* **agent** [3975f58](https://github.com/sysdiglabs/charts/commit/3975f58a59bbcee90ead958939fd4722a8bf6e19): Add logPriority flag to agent chart ([#804](https://github.com/sysdiglabs/charts/issues/804))
# v1.5.47
### New Features
* [f4cb189](https://github.com/sysdiglabs/charts/commit/f4cb189afba6833fd458f99dcfcc0121f9d9dfa2)]: unify changelog headers ([#787](https://github.com/sysdiglabs/charts/issues/787))


## v1.5.46
### Minor changes
* Fixed links displayed in the Notes section

## v1.5.45
### Minor changes
* Updated chart icon

## v1.5.44
### Minor changes
* Do not add psp policy to clusterrole if k8s > 1.25

## v1.5.43
### Minor changes
* Added `node-role.kubernetes.io/control-plane` toleration

## v1.5.42
### Minor changes
* Added negative test case to check incorrect sysdig region input, also added code changes to fail on wrong sysdig region input.

## v1.5.41
### Minor changes
* Updated override helm tests to include extra testcases.

## v1.5.40
### Minor changes
* Readme changes to indicate helm unit testing.

## v1.5.39
### Minor changes
* Added golden template tests
## v1.5.38
### Minor changes
* Added unit tests to check conditional flag testing

## v1.5.37
### Minor changes
* Added unit tests for testing labels

## v1.5.36
### Minor changes
* Revert changes from 1.5.35 due to breaking OKD3.

## v1.5.35
### Minor changes
* Remove 'beta' from kubernets.io/arch and kubernetes.io/os in daemonset due to deprecation

## v1.5.34
### Minor changes
* Fixed .helmignore to add chart tests back when packaging the chart

## v1.5.33
### Minor changes
* Added unit tests for testing helm install commands in readme

## v1.5.32
### Minor changes
* Added unit tests to check local overrides of global values

This file documents all notable changes to the Sysdig Agent Helm Chart. The release numbering uses [semantic versioning](http://semver.org).

## v1.5.30
### Minor changes
* Tests: Added helm unit test to check apiEndpoint value set because of different region inputs.

## v1.5.29
### Minor changes
* Usage of global tags over existing value of tags

## v1.5.28
### Minor changes
* Add aroberts87 to chart maintainers

## v1.5.27
### Minor changes
* Removed trailing spaces

## v1.5.25
### Bugfix
* Don't deploy psp policies on k8s 1.25.x

## v1.5.24
### Minor changes
* Added a global gke autopilot flag

## v1.5.23
### Minor changes
* Added certificatesigningrequests resources in agent clusterrole

## v1.5.22

### Minor changes
* Add deployment test to agent chart

## v1.5.21

### Minor changes
* Moved the clusterrole's Ingresses resource in the networking.k8s.io group

## v1.5.19

### Bugfixes
* Don't mount /etc on GKE autopilot

## v1.5.18

### Minor changes
* Added /etc to container and initContainer /host/etc volume bind

## v1.5.17

### Minor changes
* Readme fixes

## v1.5.16

### Minor changes
* Removed warning from agent chart readme

## v1.5.15

### Minor changes
* Introduced support to proxy for agent initContainer

## v1.5.14
* Documentation fix slim-agent defaults to true

## v1.5.13

### Minor changes
* Reverted change for v1.5.10 that added /etc to /host/etc volume bind.

## v1.5.11

### Minor changes
* Added helper to accomodate agent configmapname

## v1.5.10

### Minor changes
* Added /etc to container /host/etc volume bind

## v1.5.9

### Bugfix

* Fix agent container name to match previous name `sysdig`

## v1.5.8

### Bugfix

* Fixed region collector addresses for us4, au1

## v1.5.7

### Minor Changes

* Fixed README redirect

## v1.5.6

### Bugfix

* make collectorHost required when region is custom

## v1.5.5

### Bugfix

* Require collectorHost to be specified if one of the SaaS regions isn't used

## v1.4.4

### Bugfix

* fix the `agent.ebpfEnabled` helper so it doesn't always evaluate to `true`

## v1.4.3

### Minor Changes

* Strip the custom appcheck stuff out of the agent chart


## v1.1.0

### Minor Changes

* Match the sysdig charts where the agent portion was updated up to version 1.12.70 from 1.12.56

## v1.0.0

### Major Changes

* Deploy only the Sysdig Agent daemonset and associated resources
* Automatically detect COS nodes and enable eBPF
* Use global common values for access key and cluster name
