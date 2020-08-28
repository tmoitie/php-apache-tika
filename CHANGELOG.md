# Changelog

## v1.0.0

### Added
* Type declarations and return types

### Removed
* Support for PHP 5
* Support for Apache Tika 1.14 and lower

### Changed
* `$client->getRecursiveMetadata()` returns an array as expected
* `Client::getSupportedVersions()` and `Client::isVersionSupported()` methods cannot be called statically
* `Client::getAvailableDetectors()` and `Client::getAvailableParsers()` returns an array with new format

## v0.9.3

### Added
* Recursive metadata in command line mode

## v0.9.2

### Changed
* Tested up to Apache Tika 1.24.1

## v0.9.1

### Changed
* Tested up to Apache Tika 1.24

## v0.9.0

### Added
* `Client::setEncoding()` to avoid encoding problems using app mode
* _Troubleshooting_ section to the README.md

## v0.8.0

### Added
* Option to disable append on `Client::setCallback()` to save memory

## v0.7.2

### Changed
 * Tested up to Apache Tika 1.23
 * Spawn scripts 'autodetects' if module java.se.ee is required

## v0.7.1

### Changed
* Tested up to version 1.21

## v0.7.0

### Added
* Recursive metadata support (thanks to @svaningelgem)
* Encoding to `DocumentMetadata` (thanks to @svaningelgem)

### Changed
* Improve web client extensibility
* Abstracted cache layer
* Tested up to version 1.21

### Fixed
* Compatibility with Windows on command line mode (thanks to @GAMESTER90)

## v0.6.0

### Added
* `Client::prepare()` to avoid checks, saving HTTP calls and filesystem accesses
* Support to set host and port using an URL (thanks to @mpdude)

### Changed
* Reduced memory usage (thanks to @JBleijenberg)
* Tested up to Apache Tika 1.20

## v0.5.1

### Changed
* Tested up to Apache Tika 1.19.1
* Tested up to PHP 7.3

## v0.5.0

### Added
* `Client::isVersionSupported()` method
* `Client::getSupportedMIMETypes()` method
* `Client::getAvailableDetectors()` method
* `Client::getAvailableParsers()` method
* `Client::getOption()` and `Client::getOptions()` methods to web client
* `Client::getTimeout()` and `Client::getTimeout()` methods to web client

### Changed
* Enhanced spawn.sh script