---
title: SDR RI Codebase
description: Landing page for getting started with the SDR RI Codebase and GitHub basics
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
---
# *Disclaimer*

<em>The materials shared here are intended to be used solely for understanding DDF and the SDR Reference Implementation.</em>

<em>These materials are not intended to guide the study definition process or configuration of clinical systems. Results of those activities are solely the responsibility of the user of the scripts and not the developers. </em>

<em>For more information on the DDF initiative on the TransCelerate BioPharma Inc. website, click [here](https://www.transceleratebiopharmainc.com/initiatives/digital-data-flow/).</em>

## Getting Started: SDR RI Codebase

The Study Definitions Repository (SDR) Reference Implementation is a working instance of a Study Definitions Repository that has been developed based on the **CDISC Reference Architecture (RA)** which is part of the **Unified Study Definitions Model (USDM)**.  

For details and documents regarding the RA and USDM, please go to the [CDISC Digital Data Flow website](https://www.cdisc.org/ddf).

TransCelerate’s intent is to facilitate the development of open-source, vendor-agnostic solutions to facilitate digital data flow (“DDF”).  Accordingly, while the SDR is currently developed with Microsoft Azure, the intent is for users to be able to implement the elements of DDF in any environment or system.  

### SDR RI Releases


| Version                                                                                                                                                                                               | Date                                                                                                                                                                                                                                                                                                                                                                                                                                                                         | Release Notes                                                                                                                 |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------|
| R1.0 ([USDM 1.0 Draft](https://github.com/transcelerate/ddf-home/blob/main/documents/USDM/USDM_RA_v1.0_(Draft).zip)) <br> (previously described as MVP)| April 2022 | - Automated data flow from study builder applications of protocol data to the SDR-RI <br> - Automated data flow from SDR-RI to other applications, such as Electronic Data Capture (EDC) applications <br> - User interface to review study information stored in the SDR-RI
| R1.0.1 ([USDM 1.0 Provisional](https://github.com/transcelerate/ddf-home/blob/main/documents/USDM/USDM_RA_v1.0_(Provisional).zip)) <br> (previously described as v0.5)| Sept 2022 | - Updates to support updates from USDM v1.0 to USDM v1.0 Provisional |
| R2.0.0 ([USDM 2.0 Draft](https://github.com/transcelerate/ddf-home/blob/main/documents/USDM/USDM_RA_v2.0_(Draft).zip)) | March 2023 | Summary is provided below with detailed Release Notes available [here](https://github.com/transcelerate/ddf-sdr-support/tree/main/documents) <br> **SDR Data Model** <br> -Biomedical Concepts <br> -Complex Time Relationships <br> -Stores Study Versions <br> **SDR User Interface** <br> -Dashboard of landing page <br> -View Study Data <br> -Search & Filter <br> -Study Comparison <br> -Study Version Comparision <br> -Admin Only: Change Audit <br> -Revision History <br> -Conformance Rules Validation <br> -System Usage Report (Admin-only) <br> **SDR APIs** <br> -Upstream APIs extended <br> -Downstream APIs extended <br> -API for eCPT Export <br> **Security** <br> -Certificate-based Authentication <br> -Token-based Authentication for API <br> -Data Segmentation, Group Management, and User Management |



## SDR RI Codebase as Open Source & GitHub

The SDR Reference Implementation has been designed and deployed to be open-source and vendor agnostic.  The goal of having an open-source, vendor agnostic solution is to create a platform for both innovation and collaborative interoperability across the industry.

GitHub is the platform where the SDR RI code is published.  

**New to GitHub?** Click [Getting Started with GitHub](github-support.md) for some guidance on accessing and using GitHub.  

## DDF Community and Participation

The DDF Community is about working together under an open-source framework toward continuous improvement, learning from each other, and sharing information.

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
| [ddf-home](https://github.com/transcelerate/ddf-home)         | This repository holds all public facing website content for the DDF Initiative. It contains the overview of the DDF initiative, as well as the associated open-source information such as Contributor License Agreement (CLA), Community Code of Conduct, contact information, and all documentation on accessing the SDR Reference Implementation. |
| [ddf-sdr-platform](https://github.com/transcelerate/ddf-sdr-platform) | This repository holds the scripts written in Terraform for provisioning the underlying cloud hosted infrastructure to run the SDR platform, initially focused on the Microsoft Azure platform.                                                                                                                                                      |
| [ddf-sdr-api](https://github.com/transcelerate/ddf-sdr-api)           | This repository holds the ASP.NET Core API layer that comprises the core of the SDR platform                                                                                                                                                                                                                                                       |
| [ddf-sdr-ui](https://github.com/transcelerate/ddf-sdr-ui)             | Several user interface features including search, view, and compare functionality was created to support the SDR.  This repository holds the ASP.NET Core user interface layer code developed for these features                                                                                                                                  |
| [ddf-sdr-support](https://github.com/transcelerate/ddf-sdr-support)             | Core documentation to help new users get started with the DDF SDR system.                                                                                                                                                     |

Each repository contains supporting documentation for access and installing the code.

<!--- ### How-To Videos >
<!--- Several videos have been created to show steps a user would need to go through to provision a new instance of the SDR in their organization's local environment. >

<!--- NOTE: The instructions and guidance are based on deploying the code in Azure only. >

<!--- 1. [Environment Creation for SDR on Azure](https://www.youtube.com/watch?v=8k_fdwMNafY&list=PLMXS-Xt7Ou1KNUF-HQKQRRzqfPQEXWb1u&index=1)>
<!--- 2. [Deploying SDR code on Azure DevOps](https://www.youtube.com/watch?v=yulXnWUPbp8&list=PLMXS-Xt7Ou1KNUF-HQKQRRzqfPQEXWb1u&index=2)>
<!--- 3. [Azure PaaS Configurations](https://www.youtube.com/watch?v=MXLUbjDAqgs&list=PLMXS-Xt7Ou1KNUF-HQKQRRzqfPQEXWb1u&index=3)>
<!--- 4. [Application Data Setup and Smoke Test](https://www.youtube.com/watch?v=KQ7PPmGOz7A&list=PLMXS-Xt7Ou1KNUF-HQKQRRzqfPQEXWb1u&index=4)>
<!--- 5. [SonarQube Integration with Azure](https://www.youtube.com/watch?v=w11p7R10L2w&list=PLMXS-Xt7Ou1KNUF-HQKQRRzqfPQEXWb1u&index=5)>
<!--- 6. [SDR RI API Demo](https://www.youtube.com/watch?v=s9Qnzxy7HME&list=PLMXS-Xt7Ou1KNUF-HQKQRRzqfPQEXWb1u&index=7)>
<!--- 7. [SDR RI UI Demo](https://www.youtube.com/watch?v=223OgGvERRw&list=PLMXS-Xt7Ou1KNUF-HQKQRRzqfPQEXWb1u&index=6)>