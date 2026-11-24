# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.3.0](https://github.com/sergeym/bddkit-etcd/releases/tag/v0.3.0) - 2026-11-24

### Added

- lease steps (grant, keep alive, revoke, put under a lease, and their assertions)
- resume a watch after its stream breaks
- named etcd watches with a buffer and event assertions ([#22](https://github.com/sergeym/bddkit-etcd/pull/22))
- a failover example on three real nodes that the exec plugin starts and kills
- etcd should accept / refuse steps for put, read and compaction
- steps for one node of a cluster (leader, applied revision, HashKV, serializable get)
- add key assertions ([#5](https://github.com/sergeym/bddkit-etcd/pull/5))
- key steps with failure classes and per-operation evidence
- plugin skeleton, resource config validation and live probe ([#2](https://github.com/sergeym/bddkit-etcd/pull/2))

### Fixed

- say TLS did not agree when the server closes the handshake
- let the probe's own timeout fire before the client's

### Other

- release 0.3.0
- the watch steps, their rules and the open points of watch resume
- watch examples, and a watch through a failover that kills the watched node
- layout of the watch module and its tests
- release 0.2.0
- README for the cluster and refusal steps and the failover example
- a three-node etcd cluster of real processes that tests can break
- version 0.1.0, the first release (bddkit-etcd#7)
- the plugin README, from the config keys to running in parallel
- run the example suites against two servers and a failing one
- the secure test servers, certificates and the token rule
- TLS, mutual TLS and password authentication against a real etcd
- *(tests)* move the handle helper to tests/common
- release workflow for five targets with a rebuild_tag input ([#3](https://github.com/sergeym/bddkit-etcd/pull/3))
- agent orientation for the plugin repository ([#2](https://github.com/sergeym/bddkit-etcd/pull/2))
- Initial commit
