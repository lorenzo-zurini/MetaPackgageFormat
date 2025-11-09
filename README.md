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

PACKAGENAME - The name of the package eg. "Age of Empires II"
PACKAGEUID - A unique identifier for this specific software. For games, using TGDBID is recommended.
PACKAGEVERSION - A package version, set by the packager eg. "v1.0"
"SUBGAMES":
    [
{
        "TITLE": "Age of Mythology",
        "PLATFORM": "Windows",
        "EXEPATH": "aom.exe",
        "EXEARGS": "xres=%ScreenWidth% yres=%ScreenHeight%",
        "WORKDIR": null,
        "GAMEUID": "7804",
        "TGDBID": "7804",
        "STEAMAPPID": null,
        "UMUID": "0",
        "GOGPRODUCTID": null,
        "COVER": "AoM_Cover.jpg",
        "RELEASEDATE": "2002-10-30",
        "EDITION": "Original Release",
        "EDITIONDATE": null,
        "DEVELOPER": "Ensemble Studios",
        "PUBLISHER": "Microsoft Studios",
        "SERIES": "Age of Empires",
        "SERIESSORTNUMBER": "6",
        "SUBSERIES": "Age of Mythology",
        "SUBSERIESSORTNUMBER": "1",
        "EDITOR": "Yes",
        "ONLINEDRM": "No",
        "NETWORKMULTIPLAYER": "Yes",
        "DIRECTCONNECT": "Yes",
        "LANMULTIPLAYER": "Yes",
        "ONLINEMULTIPLAYER": "No",
        "NETWORKCOOP": "No",
        "LOCALMULTIPLAYER": "No",
        "LOCALCOOP": "No",
        "OTHERONLINEFEATURES": "NA",
        "COMPONENT": "3"
        },
        {
        "TITLE": "Age of Mythology - The Titans",
        "PLATFORM": "Windows",
        "EXEPATH": "aomx.exe",
        "EXEARGS": "xres=%ScreenWidth% yres=%ScreenHeight%",
        "WORKDIR": null,
        "GAMEUID": "7805",
        "TGDBID": "7805",
        "STEAMAPPID": null,
        "UMUID": "0",
        "GOGPRODUCTID": null,
        "COVER": "AoM_X_Cover.jpg",
        "RELEASEDATE": "2003-09-30",
        "EDITION": "Original Release",
        "EDITIONDATE": null,
        "DEVELOPER": "Ensemble Studios",
        "PUBLISHER": "Microsoft Studios",
        "SERIES": "Age of Empires",
        "SERIESSORTNUMBER": "7",
        "SUBSERIES": "Age of Mythology",
        "SUBSERIESSORTNUMBER": "2",
        "EDITOR": "Yes",
        "ONLINEDRM": "No",
        "NETWORKMULTIPLAYER": "Yes",
        "DIRECTCONNECT": "Yes",
        "LANMULTIPLAYER": "Yes",
        "ONLINEMULTIPLAYER": "No",
        "NETWORKCOOP": "No",
        "LOCALMULTIPLAYER": "No",
        "LOCALCOOP": "No",
        "OTHERONLINEFEATURES": "NA",
        "COMPONENT": "7"
        }
    ],
    "COMPONENTS":
    [


# Components
