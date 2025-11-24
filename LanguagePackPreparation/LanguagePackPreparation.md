---
questions:
    - What are the three phases of Language Pack Preparation?
    - What is the purpose of Import Data Preparation?
    - Where is Help Preparation performed?
    - What batch scripts are run during Help Preparation?
    - What two sources of input do Language Builds use?
    - What does CLP stand for and what is its purpose?
    - What is BQT and when is it performed?
    - How are Language Packs prepared for delivery?
---

# Language Pack Preparation Process

This process is divided into three phases:

- **Input**
        - Import data preparation
        - Help preparation
- **Processing**
        - Language builds
- **Output**
        - Translation Rounds
        - Preparing CLP

## Input Phase

### Import Data Preparation

Import data preparation is the first step in the Language Pack Preparation process.

#### Activities

- Extract resource files from installed DCC based on the latest Weekly Global build (Import data).
- Copy prepared Import data to the Distribution share for processing.

#### Important Notes

- This step contains information with the latest string updates from the Weekly Global Build.
- The development team and EM team must update the [Sharepoint for EM/Platform Sheets](https://siemens.sharepoint.com/teams/AutonomousBuildingART/PNB/Forms/All%20Compact.aspx?id=%2Fteams%2FAutonomousBuildingART%2FPNB%2FDevelopment%2FDesign%2FTranslation&sortField=Modified&isAscending=true&viewid=05b4b9c4%2D3b1b%2D48f9%2D9bdd%2Dc60682cb7add) if there are any changes, feature updates, or file deletions for particular EMs or platforms.
- Notify the Language Pack team about these updates.
- Language pack delivery includes the required string updates only if the above notifications are completed. Otherwise, the delivery contains strings without the latest updates.

### Help Preparation

Help preparation is the second step in the Language Pack Preparation process. This step is performed on the ST4 Cloud Machine.

#### Activities

- Generate ST4 Help production based on the latest Weekly Global build.
- Run batch scripts to:
        - Remove redundant images
        - Update look and feel (CSS file changes)
        - Create zip files
- Create Help zips: EngineeringHelp and OperatingHelp.
- Copy created zips to the Distribution share.

## Processing Phase

### Language Builds

Language builds use two sources of input:

- Import data
- Build configs and Local Sandbox TTKs

Language builds are executed on Build machines using scripts from Alchemy Catalyst, producing TTKs and translated resource files in respective folders in the GMS Distribution share.

## Output Phase

### Language Pack Creation

Language pack preparation (CLP) combines the build output from the Processing phase with the copied Help zips to create a CLP for BQT.

BQT is a series of test cases that are verified after installation and before Language Pack delivery. After completion and report generation, the Language Pack is ready for delivery.
