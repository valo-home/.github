# Valo, a local smart home hub

**Valo is an open source, self-hosted smart home hub for Zigbee, MQTT and IP cameras.** A lightweight alternative to Home Assistant for homes built on Zigbee2MQTT: one web interface for dashboards, visual automations, camera recording with object detection, extensions and an optional AI assistant. It runs on a mini PC at home, works without the cloud and installs with one command.

> **Valo is in early development, before beta.** It runs daily on real hardware in the author's home, but there are no releases yet and things still change. Feedback, bug reports and ideas are very welcome.

<a href="https://github.com/valo-home/valo"><img src="https://raw.githubusercontent.com/valo-home/valo/main/assets/screenshots/dashboard.webp" alt="Valo smart home dashboard with lights, climate, energy and scenes"></a>

<table>
<tr>
<td width="50%"><img src="https://raw.githubusercontent.com/valo-home/valo/main/assets/screenshots/home.webp" alt="Home overview with a floor plan"><br><b>Overview.</b> Rooms on a floor plan, warnings, scenes, climate and energy</td>
<td width="50%"><img src="https://raw.githubusercontent.com/valo-home/valo/main/assets/screenshots/flow-editor.webp" alt="Visual automation editor"><br><b>Automations.</b> A visual flow editor with versions, test runs and run history</td>
</tr>
<tr>
<td width="50%"><img src="https://raw.githubusercontent.com/valo-home/valo/main/assets/screenshots/camera-timeline.webp" alt="Camera with live video and a recording timeline"><br><b>Cameras.</b> Live video, clips on events, continuous recording, detection of people and cars</td>
<td width="50%"><img src="https://raw.githubusercontent.com/valo-home/valo/main/assets/screenshots/zigbee-network.webp" alt="Zigbee network map"><br><b>Zigbee.</b> Zigbee2MQTT built in, network map, signal and firmware updates</td>
</tr>
</table>

## What Valo is for

- a home with Zigbee sensors, lights, plugs and thermostats, MQTT devices (Tasmota, ESPHome) and a few IP cameras
- people who want one compact system instead of a hub, an NVR and a pile of add-ons
- local operation: devices, video and history never leave the house
- a hub that survives power cuts and comes back by itself

If you need hundreds of integrations or a stable release today, Home Assistant is the better choice. Valo focuses on doing a smaller set of things well.

## Get started

```
curl -fsSL https://raw.githubusercontent.com/valo-home/valo/main/install.sh | sudo bash
```

On a clean Ubuntu or Debian machine this installs Docker, starts Valo and prints its address. With Docker already installed, `git clone https://github.com/valo-home/valo.git && cd valo && docker compose up -d` does the same. To look around first, run the demo with simulated devices: `MOCKS_LANG=en ./valo demo up`.

## Repositories

| Repository | What is inside |
| --- | --- |
| [valo](https://github.com/valo-home/valo) | the hub: core, web interface, official extensions, documentation, installer, screenshots |
| [extension-template](https://github.com/valo-home/extension-template) | a template for your own extension with a working example and tests |
| [app](https://github.com/valo-home/app) | the mobile app, planned |
| [.github](https://github.com/valo-home/.github) | this page, contributing guide, issue templates |

## Get involved

- try the demo and [open an issue](https://github.com/valo-home/valo/issues/new/choose) for anything that looks wrong
- write an extension for a device or a service you use, start from the [template](https://github.com/valo-home/extension-template)
- help with translations: English, Ukrainian, Russian, German, French, Spanish and Japanese
- read the [contributing guide](https://github.com/valo-home/.github/blob/main/CONTRIBUTING.md) before a pull request

Valo is open source under the Apache License 2.0. It is not affiliated with Home Assistant.
