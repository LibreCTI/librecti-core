
<h1 align="center">
  <a href="https://librecti.org">LibreCTI</a>
</h1>

<p align="center">
  <a href="https://github.com/LibreCTI" alt="Website"><img src="https://img.shields.io/badge/website-librecti.org-blue.svg" /></a>
  <a href="https://github.com/LibreCTI/librecti-docs" alt="Documentation"><img src="https://img.shields.io/badge/documentation-latest-orange.svg" /></a>
  <img src="https://img.shields.io/badge/version-not%20stable-red" alt="Version Status">
</p>


LibreCTI is a work-in-progress open source platform based on OpenCTI that allows organizations to manage their cyber threat intelligence knowledge and observables. It has been created in order to structure, store, organize and visualize technical and non-technical information about cyber threats.

The structuration of the data is performed using a knowledge schema based on the [STIX2 standards](https://oasis-open.github.io/cti-documentation/). It has been designed as a modern web application including a [GraphQL API](https://graphql.org) and an UX oriented frontend. Also, LibreCTI can be integrated with other tools and applications such as [MISP](https://github.com/MISP/MISP), [TheHive](https://github.com/TheHive-Project/TheHive), [MITRE ATT&CK](https://github.com/mitre/cti), etc.

![Screenshot](./.github/img/screenshot.png "Screenshot")

## Objective

The goal is to create a comprehensive tool allowing users to capitalize technical (such as TTPs and observables) and non-technical information (such as suggested attribution, victimology etc.) while linking each piece of information to its primary source (a report, a MISP event, etc.), with features such as links between each information, first and last seen dates, levels of confidence, etc. The tool is able to use the [MITRE ATT&CK framework](https://attack.mitre.org) (through a [dedicated connector](https://github.com/OpenCTI-Platform/connectors)) to help structure the data. The user can also choose to implement their own datasets.

Once data has been capitalized and processed by the analysts within LibreCTI, new relations may be inferred from existing ones to facilitate the understanding and the representation of this information. This allows the user to extract and leverage meaningful knowledge from the raw data.

LibreCTI not only allows [imports](https://docs.opencti.io/latest/usage/import-automated/) but also [exports of data](https://docs.opencti.io/latest/usage/feeds/) under different formats (CSV, STIX2 bundles, etc.). [Connectors](https://filigran.notion.site/OpenCTI-Ecosystem-868329e9fb734fca89692b2ed6087e76) are currently developed to accelerate interactions between the tool and other platforms.

## If OpenCTI exists, why LibreCTI?

LibreCTI platform is based on OpenCTI Community edition, originally based in Apache License. LibreCTI changes, however, are licensed using Affero GNU Public License to enforce that any user of the platform will have always a version of the platform.
OpenCTI ships a version of the code that includes non-free code which is removed from this version of the platform.

## Documentation and demonstration

If you want to know more on LibreCTI, you can read the [documentation GitHub](https://github.com/LibreCTI/librecti-docs). 

## Installation

Although you need to install the LibreCTI platform will be `docker`. More details on this will be released when the platform is ready.

## Community

### Status & bugs

Currently LibreCTI is not stable at all.
OpenCTI as well is under heavy development, if you wish to report bugs or ask for new features, you can directly use the [Github issues module](https://github.com/OpenCTI-Platform/opencti/issues) of OpenCTI.

## About

### Authors

LibreCTI is shipped as free software by the Community based on OpenCTI's original code.
OpenCTI is a product designed and developed by the company [Filigran](https://filigran.io).

<a href="https://filigran.io" alt="Filigran"><img src="./.github/img/logo_filigran.png" width="300" /></a>

### Data Collection

#### Usage telemetry

To improve the features and the performances of OpenCTI, the platform collects anonymous statistical data related to its usage and health.

You can find all the details on collected data and associated usage in the [usage telemetry documentation](https://docs.opencti.io/latest/reference/usage-telemetry/).

#### OpenStreetMap server

To provide OpenCTI users with cartography features, the platform uses a dedicated OpenStreetMap server (https://map.opencti.io). To monitor usage and adapt services performances, Filigran collects access log to this server (including IP addresses).

By using this server, you authorize Filigran to collect this information. Otherwise, you are free to deploy your own OpenStreetMap server and modify the platform configuration accordingly.

If you have started using the Filigran server and change your mind, you have the right to access, limit, rectify, erase and receive your data. To exercise your rights, please send your request to privacy@filigran.io.
