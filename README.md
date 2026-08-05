![bedjet logo](https://brands.home-assistant.io/bedjet/logo.png)

# BedJet for Home Assistant

This project provides various entities to allow control of a [BedJet V2 or BedJet 3](https://bedjet.com) device.

> 🙏 **Credits**
>
> This is a fork of [natekspencer/ha-bedjet](https://github.com/natekspencer/ha-bedjet), the original BedJet integration for Home Assistant. All credit for the core integration goes to [@natekspencer](https://github.com/natekspencer); this fork builds on that work. Please consider [sponsoring](https://github.com/sponsors/natekspencer) or [buying him a coffee](https://ko-fi.com/natekspencer) if you find this integration useful.

> ⚠️ **Important**
>
> BedJet devices only allow **one active Bluetooth connection at a time**. If the BedJet mobile app is open (or running in the background) and connected to the device, Home Assistant will not be able to connect to it. The BedJet remote is not affected by this limitation, as it uses RF rather than Bluetooth.
>
> Before proceeding, **make sure the BedJet app is fully closed**. If you need to use the app (for example, to adjust biorhythm programs), temporarily disable the Home Assistant integration.

## ⬇️ Installation

### HACS (custom repository)

[![Add Repository to HACS](https://my.home-assistant.io/badges/hacs_repository.svg)](https://my.home-assistant.io/redirect/hacs_repository/?owner=Melhiser-Olson-Home&repository=ha-bedjet-enhanced&category=integration)

This is a fork, so it isn't in the default HACS store. Add it as a custom repository instead:

1. Use the **My Home Assistant** badge above, or from within Home Assistant: HACS → the three-dot menu (top right) → **Custom repositories**
2. Add `https://github.com/Melhiser-Olson-Home/ha-bedjet-enhanced`, category **Integration**
3. Search for `BedJet` in HACS and click **DOWNLOAD**
4. Restart Home Assistant

> ⚠️ If you already have the original [natekspencer/ha-bedjet](https://github.com/natekspencer/ha-bedjet) installed via HACS, remove it first — both use the `bedjet` domain and can't be installed side by side.

### Manual

If you prefer manual installation:

1. Download or clone this repository
2. Copy the `custom_components/bedjet` folder to your Home Assistant `custom_components` directory. If this is your first custom component, you may need to create the directory.  
   Example paths:
   - Hassio: `/config/custom_components`
   - Hassbian: `/home/homeassistant/.homeassistant/custom_components`
3. Restart Home Assistant

> ⚠️ Manual installation will not provide automatic update notifications. HACS installation is recommended unless you have a specific need.

## ➕ Setup

Once installed, you can set up the integration by clicking on the following badge:

[![Open your Home Assistant instance and start setting up a new integration.](https://my.home-assistant.io/badges/config_flow_start.svg)](https://my.home-assistant.io/redirect/config_flow_start/?domain=bedjet)

Alternatively:

1. Go to [Settings > Devices & services](https://my.home-assistant.io/redirect/integrations/)
2. In the bottom-right corner, select **Add integration**
3. Type `BedJet` and select the **BedJet** integration
4. Follow the instructions to add the integration to your Home Assistant

## Screenshot

![screenshot](images/BedJet3-HA.png)
