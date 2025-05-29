<p align="center">
<img src="images/clarus-logo.png" width="15%"/> <img src="images/idsa-logo.png" width="45%"/> 
</p>

![Version Badge](https://img.shields.io/badge/Release-In%20Progress-green)

<!--the list of used link is at the bottom of the file-->

# Infrastructure MVDS Clarus Data Space
This repository contains information about the infrastructure used to install the components of the CLARUS Minimum Viable Data Space ([MVDS][mvds-link]). It is a combination of components to initiate a data space with just enough features to be usable for secure and sovereign data exchange, as specified by International Data Spaces Association ([IDSA][idsa]).

## Table of contents
* [**Architecture**](#architecture)
* [**Components**](#components)
* [**Hardware and Software Requirements**](#requirements)
* [**Architecture**](#architecture)
* [**Support Team**](#support-team)
<!--* [**License**](#license)-->
<!--* [**Endpoints**](#endpoints)-->

## Architecture

![Architecture](images/clarus-architecture.jpg)

## Components
* [Identity Provider Omejdn][omejdn] consisting of:
    * The Certificate Authority (CA) granting X.509 certificates 
    * DAPS: The Dynamic Attributes Provisioning Service to handle dynamic attributes and manage dynamic access tokens
* [Metadata Broker][metadatabroker]
* Clearing House
* Two IDS connectors (TRUE Connector Provider and Consumer)

# requirements
### Hardware Requirements

|  Name   |           Value           |
| :-----: | :-----------------------: |
|   RAM   | 4GB (8GB is reccomended)  |
| Storage |           50GB            |
|   CPU   |          6-Core           |

It is recommended to use 64bit quad core processor to provide enough processing power for all docker containers. 

### Software Requirements

|      Name      |      Version     |             Notes        |
| :------------: | :--------------: | :----------------------: |
|     Docker     |     24.0.7       | [Docker][docker]         |
| Docker-compose |     v2.21.0      | [Docker-compose][docker] |

## Support Team

| Name                        |        E-mail          |
| :-------------------------- | :--------------------: |
| [Luigi di Corrado][luigi]   | luigi.dicorrado@eng.it |
| [Gianluca Isgro'][gianluca] | gianluca.isgro@eng.it  |
| [Luca Di Lorenzo][luca]     | luca.dilorenzo@eng.it  |

<!--
## License
-->

<!--LIST OF LINKS USED-->

[mvds-link]: https://mvds-clarus.eu/

[luigi]: https://github.com/luidicorra

[gianluca]: https://github.com/gianluca-isgro

[luca]: https://github.com/ludilorenz

[mvds]: https://github.com/International-Data-Spaces-Association/IDS-testbed/blob/master/minimum-viable-data-space/MVDS.md

[idsa]: https://internationaldataspaces.org/

[true-connector]: https://github.com/Engineering-Research-and-Development/true-connector

[testbend]: https://github.com/International-Data-Spaces-Association/IDS-testbed/blob/master/InstallationGuide.md

[docker]: https://docs.docker.com/         

[omejdn]: https://github.com/International-Data-Spaces-Association/omejdn-daps

[metadatabroker]: https://github.com/International-Data-Spaces-Association/metadata-broker-open-core

[clearinghouse]: https://github.com/International-Data-Spaces-Association/ids-clearing-house-service
