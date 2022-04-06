---
title: SDR RI Codebase
description: Landing page for getting started with the SDR RI Codebase and GitHub basics
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
---
# Getting Started on Accessing the SDR RI Codebase

The Study Definitions Repository (SDR) Reference Implementation is a working model of a Study Definitions Repository that has been developed based on the **CDISC Unified Study Definitions Model (USDM)**.  

For details and documents regarding the USDM, please go to the [CDISC Digital Data Flow website](https://www.cdisc.org/ddf).

## Disclaimer

The materials shared here are intended to be used solely for understanding DDF and the SDR Reference Implementation.

These materials are not intended to guide the study definition process or configuration of clinical systems. Results of those activities are solely the responsibility of the user of the scripts and not the developers.

For more information on the DDF initiative on the TransCelerate BioPharma Inc. website, click [here](https://www.transceleratebiopharmainc.com/initiatives/digital-data-flow/).

## SDR RI Codebase & GitHub

The SDR Reference Implementation has been deployed as open-source, and is meant to be vendor agnostic.  The goal of having an open-source, vendor agnostic solution is to create a platform for both innovation and collaborative interoperability across the industry.

GitHub is the platform where the SDR RI code is published.  

**New to GitHub?** Click [Getting Started with GitHub](github-support.md) for some guidance on accessing and using GitHub.  

## DDF Open-Source Community and Participation

The DDF Community is about working together toward continuous improvement, learning from each other, and sharing information.

Please refer to the **[DDF Community Overview](community.md)** for information and expectations about:

- Community Values
- [Contributor Covenant Code of Conduct](code-of-conduct.md)
- [Contribution License Agreement](contributing.md)
- Community Meetings  

**NOTE** - It is highly recommended that all users that will be engaging with DDF read through all the DDF Community content.

## DDF GitHub Repositories

The SDR Reference Implementation codebase is separated into different repositories for ease of use.

| Repository                                                                        | Description                                                                                                                                                                                                                                                                                                                                        |
|-----------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [ddf-home](https://github.com/transcelerate/ddf-home)         | This repository holds all public facing website content for the DDF Initiative. It contains the overview of the DDF initiative, as well as the associated open source information such as Contributor License Agreement (CLA), Community Code of Conduct, contact information, and all documentation on accessing the SDR Reference Implementation. |
| [ddf-sdr-platform](https://github.com/transcelerate/ddf-sdr-platform) | This repository holds the scripts written in Terraform for provisioning the underlying cloud hosted infrastructure to run the SDR platform, initially focused on the Microsoft Azure platform.                                                                                                                                                      |
| [ddf-sdr-api](https://github.com/transcelerate/ddf-sdr-api)           | This repository holds the ASP.NET Core api layer that comprises the core of the SDR platform                                                                                                                                                                                                                                                       |
| [ddf-sdr-ui](https://github.com/transcelerate/ddf-sdr-ui)             | Several user interface features including search, view, and compare functionality was created to support the SDR.  This repository holds the ASP.NET Core user interface layer code developed for these features                                                                                                                                  |

Each repository contains supporting documentation for access and installing the code.

### How-To Videos
Several videos have been created to show steps a user would need to go through to provision a new instance of the SDR in their organization's local environment. 

NOTE: The instructions and guidance are based on deploying the code in Azure only.  

- [1. Environment Creation for SDR on Azure]()
- [2. Deploying SDR code on Azure DevOps]()
- [3. Azure PaaS Configurations]()
- [4. Application Data Setup and Smoke Test]()
- [5. SonarQube Integration with Azure]()


## Help and Support

For questions, comments, or issues regarding the code, please post to the Issues tab in the applicable GitHub repository.

- [Link to Issues](https://github.com/transcelerate/ddf-sdr-platform/issues) in Platform repository
- [Link to Issues](https://github.com/transcelerate/ddf-sdr-api/issues) in API repository
- [Link to Issues](https://github.com/transcelerate/ddf-sdr-ui/issues) in UI repository
