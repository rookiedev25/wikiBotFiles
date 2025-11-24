---
questions:
    - What is the purpose of the Sharepoint for EM/Platform Sheets?
    - When should the Excel sheet be updated by developers or GTLs?
    - How is the Language Definition determined for translations?
    - Where is the Distribution Share located and what does it host?
    - What is the GMS Translation Share used for and where is it located?
    - How often are new sheets created on the Language SharePoint?
    - What actions require updating the Excel sheet for resource files?
---

# Overview

This section provides links to important references related to the Language Pack and Translation Management process.

## Important links


### [Sharepoint for EM/Platform Sheets](https://siemens.sharepoint.com/teams/AutonomousBuildingART/PNB/Forms/All%20Compact.aspx?id=%2Fteams%2FAutonomousBuildingART%2FPNB%2FDevelopment%2FDesign%2FTranslation&sortField=Modified&isAscending=true&viewid=05b4b9c4%2D3b1b%2D48f9%2D9bdd%2Dc60682cb7add)

#### NOTE: Use above link to update the Excel sheet for your extension. For each version a new sheet is created and must be updated by GTLs/Developers whenever you:

- Add a new resource file
- Delete an existing resource file
- Rename an existing resource file
- Move a resource file from platform to extension
- Move a resource file from EM1 to EM2
Always update the Excel sheet when any of the above actions occur.

### Language SharePoint

In the Language file on the Language SharePoint, list the exact languages you want the resources translated into — this is the Language Definition. This is a draft for RCs; RCs will decide which EMs to translate.

Consult product managers to identify the exact languages. Do not use vague entries such as "All Languages".

### Distribution Share

Distribution share (internal path):
`\\ad001.siemens.net\dfs001\File\CH\GMS_Distribution`

This location hosts language packs for internal Desigo CC use (weekly packs, Field Test Deliveries, Release Candidates).

### GMS Translation Share for RCs

Upload and download translation ttk files at:
`\\ad001.siemens.net\dfs001\File\CH\GMS_Distribution\GMS_Translations`

RCs use this share to exchange ttk translation files that are then added into the language build.