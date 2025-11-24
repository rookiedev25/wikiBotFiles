---
questions:
    - What are the two main types of localization supported in Desigo CC?
    - How many languages are supported for localization in Desigo CC?
    - What file types can be localized as resource files?
    - How many languages are currently supported for Help localization?
    - What tools are commonly used in the Help translation workflow?
    - What file format is used when ST4 generates Help files for translation?
    - What is the typical workflow for Help file translation and integration?
---

# Localization Process

Desigo CC supports localization of both resource (UI) texts and Help files.

## Resource Localization

Resource localization covers translation of the UI strings used in the Desigo CC application. Localization is supported in 32 languages.

## Supported languages for V9.0

- ar-SA
- bg-BG
- cs-CZ
- da-DK
- de-DE
- en-GB
- en-US (default)
- es-ES
- es-MX
- et-EE
- fi-FI
- fr-CA
- fr-FR
- he-IL
- hr-HR
- hu-HU
- it-IT
- ja-JP
- ko-KR
- nb-NO
- nl-NL
- pl-PL
- pt-BR
- pt-PT
- ro-RO
- ru-RU
- sk-SK
- sl-SI
- sv-SE
- tr-TR
- uk-UA
- zh-CN
- zh-TW



Supported resource file types and extensions:
- Binary resources
    - DLL
    - EXE
    - Library resources
- XML
- Special resources
    - JSON
    - PROPERTIES

## Help Localization

Help localization covers translation of Help files (Word/HTML) for the platform and extension topics. Currently supported Help translation languages: de-DE, fr-FR, fr-CA.

Typical Help translation workflow:
1. ST4 generates Help files as .XML.
2. The .XML files are sent to translators who translate them (commonly using Trados).
3. Translators return the translated .XML files.
4. Translated files are imported into the respective language aspect of the Help project in ST4.
5. Help is generated for each translated language and integrated into the language pack delivery.