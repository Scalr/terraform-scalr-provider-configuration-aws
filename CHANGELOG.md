# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.1.1] - 2022-07-19

### Fixed

- Plan would fail with the error `Error retrieving environment: Environment with name '*' not found or user unauthorized` if the provider configuration had to be shared with all environments

### Required

`scalr-server` > 8.27.0

## [0.1.0] - 2022-07-15

### Added

The initial release. Added support for:

- Provider configuration with the existing AWS IAM role.

- Provider configuration with the module-created role. The role can have the following trusted entities types:

  - AWS account - Allow entities in other AWS accounts belonging to you or a 3rd party to perform actions in this account.
  - AWS service - Allow AWS services like EC2 to perform actions in this account.
  
- Custom IAM policy documents for the module-created IAM roles.

- All AWS regions (including Gov cloud and China) are supported

- Sharing a provider configuration in all or selected Scalr environments.

- Self-managed or auto-generated external identifiers for AWS account trusted entities.

### Required

`scalr-server` > 8.27.0


[Unreleased]: https://github.com/Scalr/terraform-provider-scalr/compare/v0.1.1...HEAD
[0.1.1]: https://github.com/Scalr/terraform-provider-scalr/releases/tag/v0.1.1
[0.1.0]: https://github.com/Scalr/terraform-provider-scalr/releases/tag/v0.1.0