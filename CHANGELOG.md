# Change Log

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/).

## 1.202101.2

### Changed

- Default value on createModule command changed to HANA Cloud
- Remove postinstall build script from HANA Cloud option - only needed in SAP Web IDE
  
## 1.202101.1

### Fixed

- Update *@sap/hana-client* to v2.7.16, *@sap/cds* to 4.4.7 and *sap-hdbext-promisfied* to 2.202101
- Correct dump if you run *hana-cli* with no commmand, no defaults to *help* command
- Correct error when using .env for connections and there are multiple HANA and User Provided Services both in the configuration
- Correct openDBX command in Business Application Studio when using .env for connections

### Added

- Node.js 14.x support
- New command copy2DefaultEnv - which copies a .env file to default-env.json and reformats the content. Designed for Business Application Studio and the HANA tooling where a .env file is generated by a binding but CAP still requires a default-env.json for testing
