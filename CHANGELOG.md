## [1.3.3](https://github.com/de-it-krachten/ansible-role-firewall/compare/v1.3.2...v1.3.3) (2023-05-06)


### Bug Fixes

* Support service facts w/ '.service' ([6dbc3b5](https://github.com/de-it-krachten/ansible-role-firewall/commit/6dbc3b50b6a2129657f8b72b9f4d79dcaf169ae6))

## [1.3.2](https://github.com/de-it-krachten/ansible-role-firewall/compare/v1.3.1...v1.3.2) (2023-05-06)


### Bug Fixes

* Switch to service_facts module ([9e78c38](https://github.com/de-it-krachten/ansible-role-firewall/commit/9e78c3809115def50026c787f11fc3ece059507e))

## [1.3.1](https://github.com/de-it-krachten/ansible-role-firewall/compare/v1.3.0...v1.3.1) (2022-11-27)


### Bug Fixes

* Fix missing external role dependencies ([8f83bad](https://github.com/de-it-krachten/ansible-role-firewall/commit/8f83bad01e5abe7892e20079ddfc5729fe3b2550))

# [1.3.0](https://github.com/de-it-krachten/ansible-role-firewall/compare/v1.2.0...v1.3.0) (2022-10-12)


### Features

* Move to FQCN ([a452227](https://github.com/de-it-krachten/ansible-role-firewall/commit/a452227a84ce6a6b068b2996125d1bf62118eab2))
* Update CI to latest standards ([080dcbf](https://github.com/de-it-krachten/ansible-role-firewall/commit/080dcbf68b6af2f5fa7e39aadb49a5719acb3d42))

# [1.2.0](https://github.com/de-it-krachten/ansible-role-firewall/compare/v1.1.1...v1.2.0) (2022-07-28)


### Features

* Implement ansible-lint v6 support ([f67e8f3](https://github.com/de-it-krachten/ansible-role-firewall/commit/f67e8f314960e6972b36292c36be76ae8be4eed7))

## [1.1.1](https://github.com/de-it-krachten/ansible-role-firewall/compare/v1.1.0...v1.1.1) (2022-05-30)


### Bug Fixes

* implement check on functioning of iptables ([5d92962](https://github.com/de-it-krachten/ansible-role-firewall/commit/5d9296237fbe0d74339ea236a21902bfa0b83751))

# [1.1.0](https://github.com/de-it-krachten/ansible-role-firewall/compare/v1.0.5...v1.1.0) (2022-05-10)


### Bug Fixes

* remove obsolete roles from meta/requirements.yml ([07e7116](https://github.com/de-it-krachten/ansible-role-firewall/commit/07e7116b3b52436d488c80086642e892a6d17297))


### Features

* add support for Ubuntu 22.04 ([b10e711](https://github.com/de-it-krachten/ansible-role-firewall/commit/b10e7113f13b764137c672c66f06a0085c2f4e36))

## [1.0.5](https://github.com/de-it-krachten/ansible-role-firewall/compare/v1.0.4...v1.0.5) (2022-05-08)


### Bug Fixes

* identification no longer fails if no iptables is found ([7ffa2c8](https://github.com/de-it-krachten/ansible-role-firewall/commit/7ffa2c855a18dd7f5580e00d32d17eb7da4fcdfb))

## [1.0.4](https://github.com/de-it-krachten/ansible-role-firewall/compare/v1.0.3...v1.0.4) (2022-05-06)


### Bug Fixes

* extend iptables executable search paths ([86dd8ef](https://github.com/de-it-krachten/ansible-role-firewall/commit/86dd8ef83c0ce8219dc4ba473aea25e2a1dc98b1))

## [1.0.3](https://github.com/de-it-krachten/ansible-role-firewall/compare/v1.0.2...v1.0.3) (2022-04-02)


### Bug Fixes

* no longer assume iptables if no other fw found ([8d6ec01](https://github.com/de-it-krachten/ansible-role-firewall/commit/8d6ec019433a8352b2a536c9e4d5895e10484547))

## [1.0.2](https://github.com/de-it-krachten/ansible-role-firewall/compare/v1.0.1...v1.0.2) (2022-03-06)


### Bug Fixes

* replace 'service_facts' by 'service' results due to false status ([0528d8e](https://github.com/de-it-krachten/ansible-role-firewall/commit/0528d8ecbf4956e7b5a815aa5c65cd0c690bfba1))

## [1.0.1](https://github.com/de-it-krachten/ansible-role-firewall/compare/v1.0.0...v1.0.1) (2022-02-26)


### Bug Fixes

* convert port defined as integer into string ([58cb0fe](https://github.com/de-it-krachten/ansible-role-firewall/commit/58cb0fe497f1b491a5ecc00a902fa6aec5b64f32))

# 1.0.0 (2022-01-16)


### Features

* initial release ([c4c25d0](https://github.com/de-it-krachten/ansible-role-firewall/commit/c4c25d0ee57c21f38853fdacb9261c4f53189793))
