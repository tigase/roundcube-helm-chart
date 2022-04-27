# Changelog

## unreleased

  * Improved plugin configuration rendering: Now allows for complex types such as maps and slices
  * Allow to modify resources configuration

## v1.5.0

  * Added support to automatically install plugins via composer

## v1.4.1

  * Upgraded roundcube to v1.5.2

## v1.4.0

  * Improved `NetworkPolicy` configuration
  * Disabled `NetworkPolicy` by default
  * Fixed: For `NetworkPolicy` resource, check `networkPolicy.enabled`, not `pdb.enabled`

## v1.3.1

  * Do not add roundcube-logo.png to helm chart package (smaller package file size)

## v1.3.0

  * Updated bitnami/common dependency to v1.10.3
  * Updated roundcube default image and chart version to v1.5.1

## v1.2.0

  * Added NetworkPolicy
  * Added support for custom roundcube configuration (e.g. plugins)
  * Renamed `config.php` to `config.customPhpConfig`
  * Improved plugin configuration

## v1.1.0

  * Fixed roundcube version to `1.4.11`
  * Updated `NOTES.txt`
  * Allow for additional labels and annotations per Kubernetes resource
  * Allow setting `ipFamilyPolicy` for service, defaults to `PreferDualStack`
  * Allow for custom PHP configuration
  * Improved nginx session stickyness configuration

## v1.0.1

  * Added Roundcube logo as chart icon

## v1.0.0

  * First release
