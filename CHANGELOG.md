## 1.1.0 (Unreleased)

NEW FEATURES:

* lang/funcs: add a new `type()` function, only available in `terraform console` [GH-28501]

ENHANCEMENTS:

* configs: Terraform now checks the syntax of and normalizes module source addresses (the `source` argument in `module` blocks) during configuration decoding rather than only at module installation time. This is largely just an internal refactoring, but a visible benefit of this change is that the `terraform init` messages about module downloading will now show the canonical module package address Terraform is downloading from, after interpreting the special shorthands for common cases like GitHub URLs. [GH-28854]
* command/show: The -json output now indicates which state values are sensitive. [GH-28889]

BUG FIXES:

* command/show: Fix an issue where the json configuration representation was missing fully-unwrapped references. [GH-28884]

## Previous Releases

For information on prior major and minor releases, see their changelogs:

* [v1.0](https://github.com/hashicorp/terraform/blob/v1.0/CHANGELOG.md)
* [v0.15](https://github.com/hashicorp/terraform/blob/v0.15/CHANGELOG.md)
* [v0.14](https://github.com/hashicorp/terraform/blob/v0.14/CHANGELOG.md)
* [v0.13](https://github.com/hashicorp/terraform/blob/v0.13/CHANGELOG.md)
* [v0.12](https://github.com/hashicorp/terraform/blob/v0.12/CHANGELOG.md)
* [v0.11 and earlier](https://github.com/hashicorp/terraform/blob/v0.11/CHANGELOG.md)
