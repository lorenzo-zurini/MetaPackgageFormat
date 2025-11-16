# MetaPackgageFormat
A novel, all-in-one software distribution format.

MetaPackageFormat (MPF) is a new application package format that aims to provide a universal and platform-agnostic way to distribute all kinds of software, in a way that is highly modular, customizable, easy to use and easy to share.

# The Packages

A MetaPackage (.mpx), as distributed, is composed of 2 directories (METADATA and PACKAGEFILES).

## METADATA
A static directory containing display assets (appicon, appcover) and the MANIFEST.json.
The METADATA directory contains:

### appicon.png
Filename can vary - see MANIFEST.json
The application icon, in .png format, recommended size: 1024 x 1024.
		
### cover.png
Filename can vary - see MANIFEST.json
SteamGrid-like cover for the software, intended for games, so they can be displayed in launchers.
		
### MANIFEST.json
The most important file of the package, containing all the information that defines the interaction between the components contained in it.
MANIFEST.json is a JSON file with the following structure:

PACKAGENAME (string) - The name of the package eg. "Age of Mythology"
PACKAGEUID (string) - A unique identifier for this specific software. For games, using TGDBID is recommended.
PACKAGEVERSION (string) - A package version, set by the packager eg. "v1.0"
SUBGAMES" (array):
TITLE" (string) - "Age of Mythology",
PLATFORM" (string) - "Windows",
EXEPATH" (string) - "aom.exe",
EXEARGS" (string) - "xres=%ScreenWidth% yres=%ScreenHeight%",
WORKDIR" (string) - null,
GAMEUID" (string) - "7804",
TGDBID" (string) - "7804",
STEAMAPPID" (string) - null,
UMUID" (string) - "0",
GOGPRODUCTID" (string) - null,
COVER" (string) - "AoM_Cover.jpg",
RELEASEDATE" (string) - "2002-10-30",
EDITION" (string) - "Original Release",
EDITIONDATE" (string) - null,
DEVELOPER" (string) - "Ensemble Studios",
PUBLISHER" (string) - "Microsoft Studios",
SERIES" (string) - "Age of Empires",
SERIESSORTNUMBER" (string) - "6",
SUBSERIES" (string) - "Age of Mythology",
SUBSERIESSORTNUMBER" (string) - "1",
EDITOR" (string) - "Yes",
ONLINEDRM" (string) - "No",
NETWORKMULTIPLAYER" (string) - "Yes",
DIRECTCONNECT" (string) - "Yes",
LANMULTIPLAYER" (string) - "Yes",
ONLINEMULTIPLAYER" (string) - "No",
NETWORKCOOP" (string) - "No",
LOCALMULTIPLAYER" (string) - "No",
LOCALCOOP" (string) - "No",
OTHERONLINEFEATURES" (string) - "NA",
COMPONENT" (string) - "3"
COMPONENTS (array)

# Components
