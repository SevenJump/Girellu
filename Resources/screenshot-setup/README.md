# Start-up Guide for Screenshotting
This document will set up Assetto Corsa for making screenshots.

## Additional Installation (CM, CSP, Sol, filters)

### Installing Content Manager (CM)
Download [Content Manager][1] through the GitHub source (This is where CM is developed and updated). Click on the *Latest release* and download the ZIP file. The ZIP file should be unzipped at a location where it has read and write permission, such as the download folder.

<!-- github screenshot -->
### Installing Custom Shaders Patch (CSP)
Download Custom Shaders Patch through Content Manager. CM initially downloads the *recommended* version, which is typically outdated. Click the most recent version to update CSP. Disregard flags next to the version numbers, as they are inaccurate for describing CSP version stability. 

>Ask in the [CSP Discord server][2] whether a CSP version is suitable for making screenshots.

<!-- csp screenshot -->
### Installing Sol WeatherFX

Download [Sol][3] through RaceDepartment. Sol supports drag and drop installation with Content Manager. Use Sol *Install Guide* PDF to set up Sol.

>For Sol troubleshooting, seek assistance in the [Sol Discord server][4]. The Sol Discord server does have experimental versions, which are not released on RaceDepartment. Using an experimental Sol version will not negatively impact filter functionality.

### Installing Filters
Most filters have support for drag and drop installation with Content Manager. For manual installation, go to Assetto Corsa's Steam file directory (not the document directory), and drag the following files into their respective location:

For the filter `.INI` files 

	\assettocorsa\system\cfg\ppfilters

For the `.LUA` files that may come with a filter package 

	\assettocorsa\system\cfg\ppfilters\sol_custom_configs

Video Settings shared as `.cmpreset` belong in

	%localappdata%\AcTools Content Manager\Presets\Video Settings

CSP Settings shared as `.INI` belong in

	%localappdata%\AcTools Content Manager\Presets\Custom Shaders Patch Presets

WeatherFX Scripts shared as `.ZIP` packages containing folders and `.LUA` belong in

	\assettocorsa\extension\weather

___
## File Setup

| ![](src/config.png "\SteamLibrary\steamapps\common\assettocorsa\system\cfg\assetto_corsa.ini") |
|:---:|
| Tick "Allow free camera", untick "Orbit mode for F5 Camera", and select PNG in "Screenshots format" |

"assettocorsa.ini" must be prepared to keep the game working consistently. 
1. Navigate to `\assettocorsa\system\cfg` (The game file directory not the document directory).
2. Open "assettocorsa.ini"
3. Change the following parameters:

Original | Modified
---|---
[SCREENSHOT]<br>FORMAT=JPG | [SCREENSHOT]<br>FORMAT=PNG
[CAMERA]<br>ALLOW FREE CAMERA=0 | [CAMERA]<br>ALLOW FREE CAMERA=1

| ![](src/properties.png) |
|:---:|
| Right click on "assettocorsa.ini" then click on *Properties*. Check the *Read-only* box and click *Apply*. This will ensure the file retains its modified parameters. |

### Game Settings (Video & CSP preset)

Video presets change Assetto Corsa video settings. CSP presets change Custom Shaders Patch settings. It is highly recommended having two CSP and Video presets for high performance and high graphics.

>For optimal filter performance: Consult the filter's author for video and CSP presets.

<!-- ## Links -->
[1]: https://github.com/gro-ove/actools/releases "GitHub Repository"
[2]: https://discord.gg/SWryb5V "CSP Discord Invite"
[3]: https://www.racedepartment.com/downloads/sol.24914/ "Sol Download"
[4]: https://discord.gg/7YVrS4ydaA "Sol Discord Invite"