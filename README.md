<!--
SPDX-FileCopyrightText: Copyright (c) 2024 Infineon Technologies AG
SPDX-License-Identifier: MIT
-->

# OPTIGA™ Authenticate NBT: Host software overview

[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](CODE_OF_CONDUCT.md)
[![REUSE Compliance Check](https://github.com/Infineon/optiga-nbt/actions/workflows/linting-test.yml/badge.svg?branch=main)](https://github.com/Infineon/optiga-nbt/actions/workflows/linting-test.yml)

This is the entry page for the host software offering of the [OPTIGA&trade; Authenticate NBT](https://www.infineon.com/OPTIGA-Authenticate-NBT).

## Overview

The software offering for the OPTIGA™ Authenticate NBT consists of host libraries for C, Java and Swift. In addition, multiple example applications consisting of embedded, mobile phone, and webserver implementations are provided.

![OPTIGA™ Authenticate NBT chip](./docs/images/optiga_nbt_chip.png)

### Features

- NFC and I2C dual-interface bridge tag
- NFC Forum Type 4 Tag certified
- ISO/IEC 14443 Type A interface
- 106 up to 848 Kbit/s contactless
- Storage capacity of 8 KB user NVM
- I2C standard mode / fast mode

### Host libraries

The following host libraries are provided as reference implementations and support the integration of the OPTIGA™ Authenticate NBT into various systems.

| Name | Platform | Status |
| ---- | -------- | ------ |
| [OPTIGA™ Authenticate NBT Host Library for C](https://github.com/Infineon/optiga-nbt-lib-c) | CMake | Active |
| [OPTIGA™ Authenticate NBT Host Library for ModusToolbox™](https://github.com/Infineon/optiga-nbt-lib-c-mtb) | ModusToolbox™ | Active |
| [OPTIGA™ Authenticate NBT Host Library for Java](https://github.com/Infineon/optiga-nbt-lib-java) | Gradle Build Tool | Active |
| [OPTIGA™ Authenticate NBT Host Library for Swift](https://github.com/Infineon/optiga-nbt-lib-swift) | Swift Package Manager | Active |

### Example applications

The following example applications are provided for the listed use cases.
Each application contains a detailed description in the linked GitHub repository.

| Name | Mobile phone | Embedded | Webserver | Status |
| ---- |--------------| -------- | --------- | ------ |
| Brand protection with offline authentication   | [Android](https://github.com/Infineon/optiga-nbt-example-bp-android), [iOS](https://github.com/Infineon/optiga-nbt-example-bp-ios) |   |   | Active |
| Brand protection with online authentication    |  |   | [python (Flask)](https://github.com/Infineon/optiga-nbt-example-cott-flask)  | Active |
| Host parameterization via async. data transfer  | [Android](https://github.com/Infineon/optiga-nbt-example-adt-android), [iOS](https://github.com/Infineon/optiga-nbt-example-adt-ios) |  [ModusToolbox™](https://github.com/Infineon/mtb-example-optiga-nbt-adt)  |   | Active |
| Host parameterization via pass-through | [Android](https://github.com/Infineon/optiga-nbt-example-pt-android), [iOS](https://github.com/Infineon/optiga-nbt-example-pt-ios) |   [ModusToolbox™](https://github.com/Infineon/mtb-example-optiga-nbt-pt) |   | Active |
| Static connection handover    |  |   [ModusToolbox™](https://github.com/Infineon/mtb-example-optiga-nbt-sch) |  | Active |
| Personalization via NFC       | [Android](https://github.com/Infineon/optiga-nbt-example-perso-android), [iOS](https://github.com/Infineon/optiga-nbt-example-perso-ios) |   |   | Active |

#### Reference hardware

Dedicated reference hardware is available to simplify the evaluation of the OPTIGA™ Authenticate NBT.

- [OPTIGA™ Authenticate NBT Development Kit](https://www.infineon.com/OPTIGA-Authenticate-NBT-Dev-Kit)
- [OPTIGA™ Authenticate NBT Development Shield](https://www.infineon.com/OPTIGA-Authenticate-NBT-Dev-Shield)

The shield consists the OPTIGA™ Authenticate NBT device, an NFC antenna, and a pin-header to connect to any custom microcontroller via I2C (for embedded applications).
The kit includes the shield and, additionally, the reference host microcontroller board ([PSoC&trade; 62S2 Wi-Fi Bluetooth&reg; Prototyping Kit](https://www.infineon.com/CY8CPROTO-062S2-43439)).

## Getting started

High-level information on how to build the OPTIGA™ Authenticate NBT close-to-code documentation from the source in this repository.

### Project layout

```text
├── .github/        # GitHub-related resources (e.g., workflows)
├── .reuse/         # Configuration files for REUSE license check
├── LICENSES/       # Licenses used in this project
├── docs/           # Documentation sources and images
└── submodules/     # OPTIGA™ Authenticate NBT host software repositories as Git submodules
```

### Setup and requirements

A Git client is needed to clone this repository and its related repositories as submodules.
For instructions to get started with the related repositories, refer to the `README.md` files in the individual submodules.

### Install

Clone the repo from GitHub and initialize the submodules:

```bash
git clone <URL_OF_THIS_REPOSITORY>
cd <repo folder>
git submodule update --init --recursive 
```

## Additional information

### Related resources

- [OPTIGA™ Authenticate NBT - product page](https://www.infineon.com/OPTIGA-Authenticate-NBT)
- [OPTIGA™ Authenticate NBT - GitHub overview](https://github.com/Infineon/optiga-nbt) - **\*this repository\***

### Contributing

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for detailed contribution instructions and refer to our [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md).

### Contact

In case of questions regarding this repository and its contents, refer to [MAINTAINERS.md](MAINTAINERS.md) for the contact details of this project's maintainers.

### Licensing

Please see our [LICENSE](LICENSE) for copyright and license information.

This project follows the [REUSE](https://reuse.software/) approach, so copyright and licensing information is available for every file (including third party components) either in the file header, an individual *.license file or the .reuse/dep5 file. All licenses can be found in the [LICENSES](LICENSES) folder.
