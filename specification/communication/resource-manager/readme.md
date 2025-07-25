# vsonline

> see https://aka.ms/autorest

This is the AutoRest configuration file for Azure Communication Services.

---

## Getting Started

To build the SDKs for Azure Communication Services, simply [Install AutoRest](https://aka.ms/autorest/install) or via `npm` (`npm install -g autorest`) and in this folder run:

> `autorest`

To see additional help and options, run:

> `autorest --help`

---

## Configuration

### Basic Information

These are the global settings for the Azure Communication Services API.

``` yaml
title: CommunicationServiceManagementClient
openapi-type: arm
openapi-subtype: rpaas
tag: package-preview-2025-05-01-preview
```
### Tag: package-preview-2025-05-01-preview

These settings apply only when `--tag=package-preview-2025-05-01-preview` is specified on the command line.

```yaml $(tag) == 'package-preview-2025-05-01-preview'
input-file:
  - Microsoft.Communication/preview/2025-05-01-preview/CommunicationServices.json
  - Microsoft.Communication/preview/2025-05-01-preview/Domains.json
  - Microsoft.Communication/preview/2025-05-01-preview/EmailServices.json
  - Microsoft.Communication/preview/2025-05-01-preview/SenderUsernames.json
  - Microsoft.Communication/preview/2025-05-01-preview/SmtpUsernames.json
  - Microsoft.Communication/preview/2025-05-01-preview/SuppressionLists.json
```

### Tag: package-preview-2024-09-01

These settings apply only when `--tag=package-preview-2024-09-01` is specified on the command line.

```yaml $(tag) == 'package-preview-2024-09-01'
input-file:
  - Microsoft.Communication/preview/2024-09-01-preview/CommunicationServices.json
  - Microsoft.Communication/preview/2024-09-01-preview/Domains.json
  - Microsoft.Communication/preview/2024-09-01-preview/EmailServices.json
  - Microsoft.Communication/preview/2024-09-01-preview/SenderUsernames.json
  - Microsoft.Communication/preview/2024-09-01-preview/SmtpUsernames.json
  - Microsoft.Communication/preview/2024-09-01-preview/SuppressionLists.json
```

### Tag: package-2023-04

These settings apply only when `--tag=package-2023-04` is specified on the command line.

``` yaml $(tag) == 'package-2023-04'
input-file:
  - Microsoft.Communication/stable/2023-04-01/CommunicationServices.json
  - Microsoft.Communication/stable/2023-04-01/Domains.json
  - Microsoft.Communication/stable/2023-04-01/EmailServices.json
  - Microsoft.Communication/stable/2023-04-01/SenderUsernames.json
```
### Tag: package-preview-2023-06

These settings apply only when `--tag=package-preview-2023-06` is specified on the command line.

```yaml $(tag) == 'package-preview-2023-06'
input-file:
  - Microsoft.Communication/preview/2023-06-01-preview/CommunicationServices.json
  - Microsoft.Communication/preview/2023-06-01-preview/Domains.json
  - Microsoft.Communication/preview/2023-06-01-preview/EmailServices.json
  - Microsoft.Communication/preview/2023-06-01-preview/SenderUsernames.json
  - Microsoft.Communication/preview/2023-06-01-preview/SuppressionLists.json
```
### Tag: package-preview-2023-04

These settings apply only when `--tag=package-preview-2023-04` is specified on the command line.

``` yaml $(tag) == 'package-preview-2023-04'
input-file:
  - Microsoft.Communication/preview/2023-04-01-preview/CommunicationServices.json
  - Microsoft.Communication/preview/2023-04-01-preview/Domains.json
  - Microsoft.Communication/preview/2023-04-01-preview/EmailServices.json
  - Microsoft.Communication/preview/2023-04-01-preview/SenderUsernames.json
```

### Tag: package-2023-03

These settings apply only when `--tag=package-2023-03` is specified on the command line.

``` yaml $(tag) == 'package-2023-03'
input-file:
  - Microsoft.Communication/stable/2023-03-31/CommunicationServices.json
  - Microsoft.Communication/stable/2023-03-31/Domains.json
  - Microsoft.Communication/stable/2023-03-31/EmailServices.json
  - Microsoft.Communication/stable/2023-03-31/SenderUsernames.json
```

### Tag: package-preview-2023-03

These settings apply only when `--tag=package-preview-2023-03` is specified on the command line.

``` yaml $(tag) == 'package-preview-2023-03'
input-file:
  - Microsoft.Communication/preview/2023-03-01-preview/CommunicationServices.json
  - Microsoft.Communication/preview/2023-03-01-preview/Domains.json
  - Microsoft.Communication/preview/2023-03-01-preview/EmailServices.json
  - Microsoft.Communication/preview/2023-03-01-preview/SenderUsernames.json
```

### Tag: package-preview-2022-07

These settings apply only when `--tag=package-preview-2022-07` is specified on the command line.

``` yaml $(tag) == 'package-preview-2022-07'
input-file:
  - Microsoft.Communication/preview/2022-07-01-preview/CommunicationServices.json
  - Microsoft.Communication/preview/2022-07-01-preview/Domains.json
  - Microsoft.Communication/preview/2022-07-01-preview/EmailServices.json
```

### Tag: package-2020-08-20

These settings apply only when `--tag=package-2020-08-20` is specified on the command line.

``` yaml $(tag) == 'package-2020-08-20'
input-file:
  - Microsoft.Communication/stable/2020-08-20/CommunicationService.json
```

### Tag: package-2020-08-20-preview

These settings apply only when `--tag=package-2020-08-20-preview` is specified on the command line.

``` yaml $(tag) == 'package-2020-08-20-preview'
input-file:
  - Microsoft.Communication/preview/2020-08-20-preview/CommunicationService.json
```

### Tag: package-2021-10-01-preview

These settings apply only when `--tag=package-2021-10-01-preview` is specified on the command line.

``` yaml $(tag) == 'package-2021-10-01-preview'
input-file:
  - Microsoft.Communication/preview/2021-10-01-preview/CommunicationServices.json
  - Microsoft.Communication/preview/2021-10-01-preview/Domains.json
  - Microsoft.Communication/preview/2021-10-01-preview/EmailServices.json
```

---

# Code Generation

## Swagger to SDK

This section describes what SDK should be generated by the automatic system.
This is not used by Autorest itself.

``` yaml $(swagger-to-sdk)
swagger-to-sdk:
  - repo: azure-sdk-for-net
  - repo: azure-sdk-for-python
  - repo: azure-sdk-for-go
  - repo: azure-sdk-for-js
  - repo: azure-sdk-for-java
  - repo: azure-cli-extensions
  - repo: azure-powershell

    after_scripts:
      - bundle install && rake arm:regen_all_profiles['azure_mgmt_vsonline']
```

## CSharp

See configuration in [readme.csharp.md](./readme.csharp.md)

## Python

See configuration in [readme.python.md](./readme.python.md)

## Go

See configuration in [readme.go.md](./readme.go.md)

## Typescript

See configuration in [readme.typescript.md](./readme.typescript.md)

## Az

See configuration in [readme.az.md](./readme.az.md)

## Cli

See configuration in [readme.cli.md](./readme.cli.md)
