# Deshifrator — Desktop Application Documentation

**Published documentation:** https://ekatmoz88-alt.github.io/deshifrator-docs/

Public technical documentation for the PПО. Материалы основаны на реальных проектных описаниях и исходном коде.

## Documentation

- [Architecture and components](docs/architecture.md)
- [Application suite review: ModuleMobile, ModuleStationary, Printer / PassportPaint](docs/application-suite-review.md)
- [SQLite data-access layer review](docs/data-access-review.md)
- [Repository contents and evidence boundaries](docs/repository-completeness.md)
- [File exchange and MRZ](docs/data-exchange-and-mrz.md)
- [Technical risks and engineering decisions](docs/risks-and-decisions.md)
- [Dependencies, configuration, and runtime boundaries](docs/dependencies-and-runtime.md)

## Source code

Материалы основаны на реальных проектных описаниях и исходном коде.

## Architecture boundary

This repository documents the real **АРМ «Дешифратор»** application suite (ModuleMobile, ModuleStationary, and Printer / PassportPaint). Historical materials also use the earlier name **АРМ «Дискриптор»** for this same project; it is not a separate product. The companion repository `descriptor-arm-spec` contains complementary project-level workstation specifications, while this repository documents selected software components and source-code excerpts.

ПОСС, ПОМС, ПОШ ВБД, and the Oracle GLOBAL11 demo data model are not treated as components of the Deshifrator application in this repository. No relationship between the Oracle model and this WPF application suite is established by the available evidence.

## Technology context

The supplied packages target .NET Framework 4.5 and include WPF components, SQLite, Tesseract OCR, Elasticsearch 1.2.1, and separate mobile/stationary modules. The mobile configuration contains the UMMS SOAP endpoint. A possible .NET 8 migration is mentioned in project materials, but its scope and completion status are unverified.

## Publication

The public version must not contain credentials, cryptographic key material, personal data, production service addresses, connection strings, or actual exchange files. Environment-specific endpoints are excluded from public examples.

Материалы основаны на реальных проектных описаниях и исходном коде.


## Tags

`deshifrator` · `csharp` · `wpf` · `sqlite` · `soap` · `source-review` · `legacy-systems`
