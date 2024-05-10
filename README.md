<!--
SPDX-FileCopyrightText: Copyright (c) 2024 Infineon Technologies AG
SPDX-License-Identifier: MIT
-->

# OPTIGA™ Authenticate NBT: Host software overview

[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](CODE_OF_CONDUCT.md)
[![REUSE Compliance Check](https://github.com/Infineon/optiga-nbt/actions/workflows/linting-test.yml/badge.svg?branch=main)](https://github.com/Infineon/optiga-nbt/actions/workflows/linting-test.yml)

This is the entry page for the host software offering of the [OPTIGA&trade; Authenticate NBT](https://www.infineon.com/OPTIGA-Authenticate-NBT).

## Overview

The software offering for the OPTIGA™ Authenticate NBT consists of host libraries for C, Java and Swift. In addition, multiple example applications consisting of embedded, mobile phone, and web server implementations are provided.

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
| -----| ---------| ------ |
| [OPTIGA™ Authenticate NBT Host Library for C](https://github.com/Infineon/optiga-nbt-lib-c) | CMake | Active |
| [OPTIGA™ Authenticate NBT Host Library for Java](https://github.com/Infineon/optiga-nbt-lib-java) | Gradle Build Tool | Active |
| [OPTIGA™ Authenticate NBT Host Library for Swift](https://github.com/Infineon/optiga-nbt-lib-swift) | Swift Package Manager | Active |

### Example applications

> **coming soon..**

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
