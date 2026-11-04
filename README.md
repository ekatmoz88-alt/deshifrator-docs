# Deshifrator — Desktop Application Documentation

Public technical documentation for the Deshifrator desktop application. The materials are based on available project descriptions and selected source-code excerpts; they are not a complete specification or a full source-code audit.

## Purpose

The application supports searching and processing person and case records, integration with an external system through SOAP, address lookup using FIAS/Elasticsearch, and file-based data exchange with a mobile module.

## Documentation

- [Architecture and components](docs/architecture.md)
- [File exchange and MRZ](docs/data-exchange-and-mrz.md)
- [Technical risks and engineering decisions](docs/risks-and-decisions.md)

## Architecture boundary

ПОСС, ПОМС, and ПОШ ВБД belong to a separate architecture. They are not part of Deshifrator and must not be added to its component diagrams, relationships, interfaces, or functional descriptions without explicit confirmation.

## Technology context

The materials mention .NET Framework 4.5, WPF/WinForms, SQLite, Tesseract OCR, Elasticsearch, and SOAP. A planned or partial migration of selected components to .NET 8 is also described; the migration status must be verified against the source code.

## Security and publication boundaries

The public version contains no real credentials, cryptographic key material, personal data, production service addresses, connection strings, or actual exchange files. Environment-specific endpoints are configured separately through protected configuration.

This project was documented as part of the author's work at Scientific Instruments, Inc. (2014–2016). The content describes the historical technical context and does not imply that the listed component versions are currently in use.
