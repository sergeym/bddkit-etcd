# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.3.1](https://github.com/sergeym/bddkit-etcd/compare/v0.3.0...v0.3.1) - 2026-11-24

### Added

- commit a transaction written in the etcdctl txn format and assert which branch ran

### Other

- README for the lease and transaction steps
- lease and transaction examples, a lease kept alive through the death of the leader
- let the verdict on a refusal serve operations other than the accept / refuse steps
