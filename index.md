---
title: Digital Data Flow (DDF) Overview
description: Landing page for the DDF reference implementation and related information
layout: home
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
---
## Draft / Beta Status

While this repository and the associated code repositories (see [Getting Started on DDF](#getting-started-on-ddf)) below) are public, this is a soft launch, and the Digital Data Flow (DDF) reference implementation and this document repository should be considered in a beta/draft state.

## Introduction

The Digital Data Flow (DDF) initiative aims to modernize clinical trials by enabling a digital workflow that allows for automated creation of study content and configuration of study systems to support clinical trial execution. It provides basic mechanisms for deployment, maintenance, and scaling of applications. See the section [What is DDF?](#what-is-ddf) in this document for more information on the objective and benefits of DDF.

## What is DDF?

**What is the Digital Data Flow initiative?**

The Digital Data Flow (DDF) initiative aims to modernize clinical trials by enabling a digital workflow that allows for automated creation of study content and configuration of study systems to support clinical trial execution. This initiative will establish a foundation for a future state of automated and dynamic readiness that can transform the drug development process.

**What is the objective of the DDF initiative?**

The objective of DDF is to automate and expedite the Study Start-Up process by revolutionizing how data flows across clinical trial systems, beginning with upstream (e.g., study builder) and downstream (e.g., electronic data capturing/EDC, clinical trial management system/CTMS) clinical systems. TransCelerate will collaborate on the development of an open-source, vendor agnostic, study definition repository (SDR) reference implementation.   The SDR reference implementation will enable the format of information from a digitized protocol and other sources to be standardized, which then allows the information to be passed to systems through application programming interfaces (APIs) that are used for study execution and data collection and reused throughout the clinical development lifecycle.  In summary, DDF will combine data standards and a new technology to enable the flow of data across all systems involved in the design and execution of a clinical trial.  

**What are the benefits of the DDF initiative?**

Utilizing a standards-based study definition repository (SDR) reference implementation may facilitate an end-to-end digital data flow across clinical systems used to design and execute a trial according to the protocol. Currently, this process is largely manual and document based.  Digital Data Flow (DDF) benefits include:  

- Minimized process hand-offs, data re-entry, and data format inconsistencies across Study Start-Up and execution  
- A foundation for data exchange and interoperability between clinical technology systems, leading to greater compatibility among systems, flexibility to sponsors, and improved clinical trial efficiencies
- A more seamless flow of data leading to accelerated Study Start-Up, and further enabling trials automation for sponsors and research partners
- Harmonization of the data format that can support greater interoperability and spark innovation within the R&D ecosystem and across the clinical trial solutions landscape

**Who does the initiative help?**

This initiative will assist many organizations, including pharmaceutical companies, CROs, standards organizations, upstream and downstream clinical vendors, sites, regulatory agencies, technology companies, and the open-source pharmaceutical and IT communities. With DDF, organizations across the R&D ecosystem will be able to leverage the open-source code of the SDR reference implementation and develop a framework to deploy their own SDR implementations.

## Disclaimer

The materials shared in this repository are intended to be used solely for understanding the DDF reference implementation and assisting the deployment of the reference implementation either locally or on Microsoft Azure. Future cloud providers are being considered but not yet on a roadmap.

Nothing in these materials is intended to guide the study definition process or configuration of clinical systems. Results of those activities are solely the responsibility of the user of the scripts and not the developers.

For more information on the DDF initiative on the TransCelerate BioPharma Inc. website, click [here](https://www.transceleratebiopharmainc.com/initiatives/digital-data-flow/).

## Getting Started on DDF

Documentation for getting started is in the list of GitHub repositories below, all in the TransCelerate BioPharma Inc. organization.

- [ddf-sdr-platform](https://github.com/transceleratebiopharmainc/ddf-sdr-platform) - TerraForm code for setting up the Azure infrastructure to deploy the DDF solution
- [ddf-sdr-api](https://github.com/transceleratebiopharmainc/ddf-sdr-api) - the ASP.NET Core api layer that comprises the core of the DDF platform
- [ddf-sdr-ui](https://github.com/transceleratebiopharmainc/ddf-sdr-ui) - the ASP.NET Core user interface layer

## Other Resources

Looking for more? Check out these links

- [Digital Data Flow Initiative on the main TransCelerate BioPharma, Inc. Website](https://www.transceleratebiopharmainc.com/initiatives/digital-data-flow/)
- [Events search for "Digital Data Flow"](https://www.transceleratebiopharmainc.com/?s=digital%20data%20flow&submit=submit)
- [YouTube Channel for TransCelerate BioPharma, Inc.](https://www.youtube.com/channel/UC9S20EmzIBGJJ70utCrtNBQ/videos)
- [Twitter account for TransCelerate BioPharma, Inc.](https://twitter.com/transcelerate)

## Help and Support

todo:where to go for support?
