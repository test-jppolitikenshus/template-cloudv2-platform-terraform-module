# Contribution guidelines

When contributing to this repository, please first discuss the change you wish to make via issue, slack, or any other method with the owners of this repository before making a change.

Our primary slack channel for contributors who wish to get in touch is #ask-cloudv2-platform.

## Contributing

If you’ve got an idea or suggestion you can:

- [Contact the Cloudv2 Platform Team](https://teams.microsoft.com/l/channel/19%3AcH_4ca6aDoLPRoafFgQGycECu9rQctj_IVzVnnhW_WM1%40thread.tacv2/General?groupId=8660c61c-7766-4c28-8170-3212e5f9fbe6&tenantId=52623290-e56a-493b-8588-8c5caf95279d)
- [Create a GitHub issue](https://github.com/jppolitikenshus/cloudv2-platform/issues)

## Raising bugs

When raising bugs, please explain the issue in reasonable detail and provide a guide on how to replicate it.

When describing the bug, it's useful to follow the format:

- What you did
- What you expected to happen
- What happened

We have a [standard template](https://github.com/jppolitikenshus/cloudv2-platform/issues/new?assignees=&labels=bug&projects=&template=bug-template.md) for raising bugs.

## Suggesting features

Please [raise feature requests as issues](https://github.com/jppolitikenshus/cloudv2-platform/issues/new?assignees=&labels=&projects=&template=story-template.md) before contributing any code.

Raising an issue ensures they are openly discussed and before spending any time on them.

## Security vulnerabilities

Please contact us through [Teams](https://teams.microsoft.com/l/channel/19%3AcH_4ca6aDoLPRoafFgQGycECu9rQctj_IVzVnnhW_WM1%40thread.tacv2/General?groupId=8660c61c-7766-4c28-8170-3212e5f9fbe6&tenantId=52623290-e56a-493b-8588-8c5caf95279d) to discuss the vulnerability first, before [raising an issue](https://github.com/jppolitikenshus/cloudv2-platform/security/advisories/new).

## Contributing code

### Terraform Versions

We use Hashicorp [Terraform](https://www.terraform.io/) to deliver Infrastructure-as-Code.

We stay up-to-date with the latest versions of Terraform, but with Terraform Providers the Platform Team control the version in use.

### Tests

Our versioned Terraform modules have unit tests; these are written using [Terratest](https://pkg.go.dev/github.com/gruntwork-io/terratest#section-readme) and Google Go.

Your branch should ensure that changes you have made are reflected in the tests, and that these unit tests pass before raising a Pull Request.

A GitHub Action will automatically run tests against your Pull Request once you have raised it.

### Versioning

Where appropriate, versioning is based on your commit messages by using [Semantic Versioning](https://semver.org/).

Our [Cloudv2 Platform](https://github.com/jppolitikenshus/cloudv2-platform/) and [Cloudv2 Platform Environments](https://github.com/jppolitikenshus/cloudv2-platform-environments/) repositories are deployed with CI/CD from the _main_ branch, and thus are not versioned.

Terraform modules which are used by the [Cloudv2 Platform](https://github.com/jppolitikenshus/cloudv2-platform/) and [Cloudv2 Platform Environments](https://github.com/jppolitikenshus/cloudv2-platform-environments/) repositories
are versioned using GitHub Tags and Releases following Semantic Versioning.

When you come to raise a pull request, please explain the context for your pull request so that your changes are easier to understand.

### Release

Releases are actioned by the Cloudv2 Platform team.
