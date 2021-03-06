# Change Log
All notable changes to this project will be documented in this file.
This project adheres to [Semantic Versioning](http://semver.org/).

## [Unreleased][unreleased]
### Added
- Figure out a way to duplicate sqlsrv_field_metadata().
- Figure out a way to duplicate sqlsrv_cancel() ```$stmt = null```?

### Changed
- Make client_info() more reliable.
- Figure out how/why sqlsrv's PHPTYPE_STR(EAM|ING) function return values are randomly wrong. When wrong, they are always the same wrong values.

## [0.0.4] -
### Added
- option parsing for prepare()
- connection ref variable.

### Removed
- has_rows() and num_rows() were assumed to be working, but do not. no longer pretending.

### Fixed
- bug improperly handling invalid parameters.


## [0.0.3] - 2015-06-17
### Added
- Worked out some ugly logic for SQLTYPE_(DECIMAL|NUMERIC) functions.

### Changed
- Improved and optimized SQLTYPE functions. Reduced repeated code.

## [0.0.2] - 2015-06-09
### Added
- Logic to a few more functions.

### Changed
- Renamed class constants (removed SQLSRV_ prefixes.)
- Improved (I think) error logging function.

### Fixed
- A glaring bug where the fetch functions return false instead of null when there are no records to fetch.

## [0.0.1] - 2015-05-28
### Added
- First alpha release.

[unreleased]: https://github.com/radsectors/sqlshim/compare/v0.0.3...HEAD
[0.0.3]: https://github.com/radsectors/sqlshim/compare/v0.0.2...v0.0.3
[0.0.2]: https://github.com/radsectors/sqlshim/compare/v0.0.1...v0.0.2