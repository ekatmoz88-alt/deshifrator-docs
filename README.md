# Deshifrator — Desktop Application Documentation

Public technical documentation for the Deshifrator desktop application. The materials are based on available project descriptions and selected source-code excerpts; they are not a complete specification or a full source-code audit.

## Purpose

The package contains a desktop application and separate stationary and mobile modules for person and case workflows. The available configuration files show a UMMS SOAP endpoint in the mobile module and local FIAS/Elasticsearch settings in the mobile and stationary modules. The exact ownership of every integration must be verified against source code and service contracts.

## Documentation

- [Architecture and components](docs/architecture.md)
- [File exchange and MRZ](docs/data-exchange-and-mrz.md)
- [Technical risks and engineering decisions](docs/risks-and-decisions.md)\n- [Dependencies, configuration, and runtime boundaries](docs/dependencies-and-runtime.md)

## Architecture boundary

ПОСС, ПОМС, and ПОШ ВБД belong to a separate architecture. They are not part of Deshifrator and must not be added to its component diagrams, relationships, interfaces, or functional descriptions without explicit confirmation.

## Technology context

The supplied packages target .NET Framework 4.5 and include WPF components, SQLite, Tesseract OCR, Elasticsearch 1.2.1, and separate mobile/stationary modules. The mobile configuration contains the UMMS SOAP endpoint. A possible .NET 8 migration is mentioned in project materials, but its scope and completion status are unverified.

## Security and publication boundaries

The public version contains no real credentials, cryptographic key material, personal data, production service addresses, connection strings, or actual exchange files. Environment-specific endpoints are configured separately through protected configuration.

This project was documented as part of the author's work at Scientific Instruments, Inc. (2014–2016). The content describes the historical technical context and does not imply that the listed component versions are currently in use.
