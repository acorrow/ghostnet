<picture>
  <img alt="ICARUS Terminal" src="./resources/ghostnet_logo.svg" height="100" width="auto"/>
</picture>

![GitHub Version](https://img.shields.io/github/v/release/acorrow/icarus??display_name=tag&include_prereleases&sort=semver&color=8d5cff&style=for-the-badge)
![GitHub License](https://img.shields.io/github/license/acorrow/icarus?color=8d5cff&style=for-the-badge)
![GitHub Downloads](https://img.shields.io/github/downloads/acorrow/icarus/total?color=8d5cff&style=for-the-badge)

_ICARUS Terminal is currently in early access._

## About ICARUS Terminal

_ICARUS Terminal is a free, immersive, context-sensitive companion app and second screen interface for [Elite Dangerous](https://www.elitedangerous.com/)._

You can run ICARUS Terminal in a native window, on multiple windows/displays, as an overlayed window in top of the game if playing with a VR headset or on an ultra-wide display or connect remotely in a browser from another computer/tablet/phone/other devices (e.g. Chromebook, Android Phone/Tablet, Amazon Fire Tablet); the UI is specifically designed with touch screen devices in mind and to adapt the layout of panels to both landscape and portrait displays, both large and small.

<p align="center">&nbsp;</p>

<p align="center">
  <a href="https://github.com/acorrow/icarus/releases">
    <img alt="Download" src="https://github.com/acorrow/icarus/assets/595695/ee98eb94-f293-4eb5-8230-b7a75f17ea44" height="80" width="auto"/>
  </a>
</p>

## Screenshots

<img alt="System Map" src="https://user-images.githubusercontent.com/595695/197432007-13726aea-9413-4fcf-88c6-9abc34f2d26c.png" height="auto" width="98.5%"/>

<img alt="System List" src="https://user-images.githubusercontent.com/595695/215351117-50282d37-f42f-4eb9-975b-e70d29202cdb.png" height="auto" width="49%"/> <img alt="Ship Status" src="https://user-images.githubusercontent.com/595695/215350062-0f7ad9e4-905c-43ae-b3cf-1dc7944ab744.png" height="auto" width="49%"/>
<img alt="Blueprint" src="https://user-images.githubusercontent.com/595695/192074945-b47edcbb-6aab-444d-827c-6b6255e8f932.png" height="auto" width="49%"/> <img alt="Navigation Route" src="https://user-images.githubusercontent.com/595695/215350464-88e75eb1-77d8-408c-a0ec-12fd6911e866.png" height="auto" width="49%"/>

## Requirements

The self-contained installer is around 20 MB and has no dependancies. If you are running an older but supported release of Windows, any missing dependancies will be automatically installed.

* Windows 10 or newer required.
* No dependancies are required to install the application.
* No manual configuration or setup is required, it will automatically find your game data.
* No additional diskspace is required to store game data. Recent game data is loaded in to memory when launched and streamed in real time when the game is active, it is not persisted or cached to disk.

### Notes

* This software is in early access. All releases are pre-releases and contain known defects.
* The launcher will indicate when a new release is available. Updating is optional.
* All releases are code signed and verified. If you have a conflict with your anti-virus or firewall software, please contact the vendor responsible for that software.
* The application will run against the latest version of Elite Dangerous (Odyssey) and older releases (e.g. Horizons), but it is currently explicitly designed for use with the latest versions. Changes to the game API may impact functionality when using ICARUS Terminal with older versions of the game.
* The application includes a web interface to allow access from remote devices. The web interface is enabled by default while the application is running.

The web interface relies on advanced browser functionality for rendering and works best on native Google Chrome browsers (e.g. Google Chrome for Windows, Mac, ChromeOS, Android). Other browsers (e.g. Safari, Firefox, Chromium) may use fallback rendering and/or lack required features for full compatbility / optimal user experience.

## Developer Documentation

Code contributions, pull requests and bug reports are not currently being accepted for this repository. See [CONTRIB.md](CONTRIB.md) for more information. For developer documentation see [BUILD.md](BUILD.md).

## GHOSTNET Page

ICARUS Terminal ships with a dedicated GHOSTNET page that pulls together trade, ship, mission and resource intel submitted by the GHOSTNET community. The page is accessible from the left-hand navigation inside the app (or directly at `/ghostnet` when running the web client) and currently provides:

* **Ship availability search** – find stations selling a selected ship and view enriched details (distance, services, landing pads) from ICARUS's canonical data sets.
* **Trade route scouting** – mirror GHOSTNET's public trade route search, including profit-per-trip and per-hour metrics, with an optional sandbox mode for layout testing.
* **Mining mission leads** – surface nearby mining missions and factions that have recently posted them.
* **Pristine ring finder** – highlight bodies with pristine reserves within jump range for mining expeditions.

All GHOSTNET-sourced insights are clearly labelled inside the UI so that commanders can distinguish between local ICARUS data and community-reported values. For a deep dive into how the integration works under the hood—including details on the HTTP requests, parsers and logging used to access GHOSTNET without an API key—see [GHOSTNET-README.md](GHOSTNET-README.md).

### Developer Quickstart

Looking to run ICARUS Terminal from source? The maintained setup, build, and screenshot workflow now lives in [AGENTS.md](AGENTS.md) so contributors have a single source of truth. Follow that guide for the current development checklist and environment notes.

## Legal

ICARUS Terminal is free, open-source software released under the ISC License.

ICARUS Terminal does not record Personally Identifiable Information (PII). ICARUS Terminal includes integrations with services like [EDSM](https://www.edsm.net), [EDDB](https://eddb.io/) and [GHOSTNET](https://inara.cz/). Data such as your current in-game location, cargo, etc. may be sent to them order to render information in the interface. ICARUS Terminal does not expose or send information about you or your in game character (e.g. your name, user name, commander name or ship name) but any requests made to a third party will include your IP address.

Elite Dangerous is copyright Frontier Developments plc. This software is not endorsed by nor reflects the views or opinions of Frontier Developments and no employee of Frontier Developments was involved in the making of it.

THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY
AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT,
INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM
LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR
OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR
PERFORMANCE OF THIS SOFTWARE.

## Credits

_ICARUS Terminal would not be possible without work from dozens of enthusiasts and hundreds of open source contributors._

* The name ICARUS was suggested by [SpaceNinjaBear](https://www.reddit.com/user/SpaceNinjaBear) on Reddit.
* Loading animation by [James Panter](http://codepen.io/jpanter/pen/PWWQXK).
* Includes origional icons, icons inspired by those found in Elite Dangerous and icons based on those from [edassets.org](https://edassets.org).
* Uses stellar cartography data from the wonderful [EDSM API](https://www.edsm.net).
* Includes game data collated and provided by [EDCD](https://github.com/EDCD/FDevIDs).
* The [Jura font](https://fonts.google.com/specimen/Jura#glyphs) is included under the Open Font License.
* Thank you to [Serge Zaitsev](https://github.com/zserge) for his work on the WebView library.

ICARUS Terminal uses imagery from/inspired by Elite Dangerous, which is copyright Frontier Developments plc. This software is not endorsed by nor reflects the views or opinions of Frontier Developments and no employee of Frontier Developments was involved in the making of it.

Thank you to all those who have created and supported libraries on which this software depends and to Frontier Developments plc for supporting third party tools.

## Support

People have asked if I take donations for the project - I don't donations, but 
I do appreciate the offer.

If you want to support development of ICARUS Terminal, the best way is to visit 
the [Ardent Pioneer (V9G-G7Z)](https://inara.cz/elite/station/490914/).

Selling Tritium to the carrier directly supports development as it means I can 
spend more time adding features to ICARUS Terminal and travelling the galaxy to 
test them out!

You can use Ghostnet to [find out which system the Ardent Pioneer is currently in](https://inara.cz/elite/station/490914/) and see if it's anywhere near you.

Before you visit you might want to [check out what commodities are currently 
being traded](https://inara.cz/elite/station-market/490914/). You might also
want to chat to the bartender to see what they are looking for!

