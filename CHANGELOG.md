## WLED changelog

### Development versions after 0.10.0 release

#### Build 2005100

-   Update to Espalexa v2.4.6 (+1.6kB free heap memory)
-   Added `m5atom` PlatformIO environment

#### Build 2005090

-   Default to ESP8266 Arduino core v2.7.1 in PlatformIO
-   Fixed Preset Slot 16 always indicating as empty (#891)
-   Disabled Alexa emulation by default (causes bootloop for some users)
-   Added BWLT11 and SHOJO_PCB defines to NpbWrapper
-   Merged pull request #898 adding Solid Glitter effect

### WLED version 0.10.0

#### Build 2005030

-   DMX Single RGW and Single DRGB modes now support an additional white channel
-   Improved palettes derived from set colors and changed their names

### Development versions between 0.9.1 and 0.10.0 release

#### Build 2005020

-   Added ACST and ACST/ACDT timezones

#### Build 2005010

-   Added module info page to web UI
-   Added realtime override functionality to web UI
-   Added individial segment power and brightness to web UI
-   Added feature to one-click select single segment only by tapping segment name
-   Removed palette jumping to default if color is changed

#### Build 2004300

-   Added realtime override option and `lor` JSON property
-   Added `lm` (live mode) and `lip` (live IP) properties to info in JSON API
-   Added reset commands to APIs
-   Added `json/si`, returning state and info, but no FX or Palette lists
-   Added rollover detection to millis(). Can track uptimes longer than 49 days
-   Attempted to fix Wifi issues with Unifi brand APs

#### Build 2004230

-   Added brightness and power for individual segments
-   Added `on` and `bri` properties to Segment object in JSON API
-   Added `C3` an `SB` commands to HTTP get API
-   Merged pull request #865 for 5CH_Shojo_PCB environment

#### Build 2004220

-   Added Candle Multi effect
-   Added Palette capability to Pacifica effect

#### Build 2004190

-   Added TM1814 type LED defines

#### Build 2004120

-   Added Art-Net support
-   Added OTA platform to platformio.ini

#### Build 2004100

-   Fixed DMX output compilation
-   Added DMX start LED setting

#### Build 2004061

-   Fixed RBG and BGR getPixelColor (#825)
-   Improved formatting

#### Build 2004060

-   Consolidated global variables in wled.h

#### Build 2003300

-   Major change of project structure from .ino to .cpp and func_declare.h

#### Build 2003262

-   Fixed compilation for Analog LEDs
-   Fixed sync settings network port fields too small

#### Build 2003261

-   Fixed live preview not displaying whole light if over 255 LEDs

#### Build 2003251

-   Added Pacifica effect (tentative, doesn't yet support other colors)
-   Added Atlantica palette
-   Fixed ESP32 build of Espalexa

#### Build 2003222

-   Fixed Alexa Whites on non-RGBW lights (bump Espalexa to 2.4.5)

#### Build 2003262

  - Fixed compilation for Analog LEDs
  - Fixed sync settings network port fields too small

#### Build 2003261

  - Fixed live preview not displaying whole light if over 255 LEDs

#### Build 2003251

  - Added Pacifica effect (tentative, doesn't yet support other colors)
  - Added Atlantica palette
  - Fixed ESP32 build of Espalexa

#### Build 2003222

  - Fixed Alexa Whites on non-RGBW lights (bump Espalexa to 2.4.5)

#### Build 2003221

-   Moved Cronixie driver from FX library to drawOverlay handler

#### Build 2003211

-   Added custom mapping compile define to FX_fcn.h
-   Merged pull request #784 by @TravisDean: Fixed initialization bug when toggling skip first
-   Added link to youtube videos by Room31 to readme

#### Build 2003141

-   Fixed color of main segment returned in JSON API during transition not being target color (closes #765)
-   Fixed arlsLock() being called after pixels set in E1.31 (closes #772)
-   Fixed HTTP API calls not having an effect if no segment selected (now applies to main segment)

#### Build 2003121

-   Created changelog.md - make tracking changes to code easier
-   Merged pull request #766 by @pille: Fix E1.31 out-of sequence detection

