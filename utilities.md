---
title: Utilities
description: Page to store and link to useful tools for DDF development/implementation
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
---
# Utilities



## DDF CPT-CLI Tool

### Summary
The DDF Initiative has developed, in collaboration with Arborsys, a Proof of Concept utility tool to show how USDM can be mapped to the TransCelerate CC&R [Common Protocol Template](https://www.transceleratebiopharmainc.com/assets/clinical-content-reuse-solutions/) format, and to additionally demonstrate the automated population of an eCPT Word document by loading a USDM file directly from the SDR.
 
### Description
The tool itself is for demonstration purposes only and is not for Production use.  It is a “command line interface” (CLI) tool that can be executed very simply from a command prompt or shell.  Specifically, it is NOT an extension to the eCPT Word “addin”. 
 
The CLI tool both directly queries the DDF SDR through a custom API endpoint to retrieve the CPT variables from a given Study Design, or it can load pre-created CPT files previously extracted from the SDR.  In both cases, the tool will automatically populate a pre-existing eCPT template with the CPT variables output from the SDR.
 
The value of the CLI tool is it’s ability to demonstrate that:
- USDM can both store and represent a large portion of CPT data
- The CPT data elements stored in USDM can be unambiguously mapped to elements in the eCPT
- The extraction of CPT data elements from a USDM compliant study definition and the population of an eCPT template can be automated, without requiring human intervention
 
### Scope
- 31 CPT variables are currently stored in USDM and all 31 can be mapped into the eCPT.  The [linked spreadsheet](documents/ddf-sdr-ri-usdm-cpt-mapping-sheet-v2.0.xlsx) summarizes the mapped variables, which were derived from ICH CORE.
- Multiple valued elements are catered for, such as Interventions, Objectives and Endpoints, and Regulatory Agency IDs, among others
- Whereas all CPT variables can be extracted and parsed by the CLI, population of the eCPT has some limitations with multi-valued variables, for example tables of Objectives and Endpoints list only the first 4
- Only one (the first) Study Design within the USDM study document will be processed
 
### Pre-requisites and Dependencies
- Familiarity with USDM and CPT is helpful, to understand what the CLI tool is accomplishing
- In order to connect, and demonstrate access, to the SDR API and retrieve Study data, the user must have an account to access the TransCelerate DDF SDR RI (access registration here)
- The CLI tool will run only in a Windows environment.
 
### Downloads and Installation:
1. Download the [zip package](documents/DDF-0.23.0802.1405.zip) - there is just one zip file!
2. Installation of the CLI tool is easy – simply unzip to any local directory
3. The zip file contents are:
    - An Executable file (EXE) (self contained, no additional dependencies, its all bundled into the exe)
    - A Settings file (JSON)
    - User Guide (PDF)
    - Sample USDM (JSON) and Sample SDR-CPT (JSON) output
4. The Mapping spreadsheet (Excel) showing the coverage of elements and how they map can be found [here](documents/ddf-sdr-ri-usdm-cpt-mapping-sheet-v2.0.xlsx) 
5. The User Guide explains all the steps to try out the CLI tool, and can be separately found [here](documents/DDF CPT CLI Tool User Guide_V1.0.pdf)
 
Please email ddf@transceleratebiopharmainc.com if you have thoughts or feedback on this tool.
 
# Disclaimer
These materials and information, as well as the underlying code/application they relate to are provided by TransCelerate Biopharma Inc. AS IS. Any party using or relying on this information and, these materials and/or the underlying code/application do so entirely at their own risk. Neither TransCelerate nor its members will bear any responsibility or liability for any harm, including indirect or consequential harm, that a user may incur from use or misuse of this information, materials, or underlying code/application.
TransCelerate does not endorse any particular software, system, or service. And the use of specific brands of products or services by TransCelerate and its collaboration partners in developing the CPT CLI Tool should not be viewed as any endorsement of such products or services. To the extent that the CPT CLI Tool incorporates or relies on any specific branded products or services, this resulted out of the practical necessities associated with making a Proof of Concept available to demonstrate the interoperability between the SDR and eCPT.