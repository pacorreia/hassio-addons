[![GitHub Repo stars](https://img.shields.io/github/stars/pacorreia/hassio-addons?style=flat)](https://github.com/pacorreia/hassio-addons/stargazers) _Thanks to everyone having starred my repo! To star it click [here](https://github.com/pacorreia/hassio-addons), then click on the star on the top right. Thanks!_

# Neolink-latest

![Supports aarch64 Architecture][aarch64-shield]
![Supports amd64 Architecture][amd64-shield]

> [!CAUTION]
> This addon is still under support, but the upstream project **Neolink** (by original author [thirtythreeforty](https://github.com/thirtythreeforty) and forked by [QuantumEntangledAndy](https://github.com/QuantumEntangledAndy)) is **abandoned**.
>
> Expect this addon to stop working at any time!

## About

This App allows you to run latest Neolink directly on your HAOS instance. If you don't know Neolink you might not need this App. Details can be found [here](https://github.com/QuantumEntangledAndy/neolink). This App uses the Neolink fork of @QuantumEntangledAndy which also supports MQTT.

## Installation & Configuration

[![Open your Home Assistant instance and show the add App repository dialog with a specific repository URL pre-filled.](https://my.home-assistant.io/badges/supervisor_add_addon_repository.svg)](https://my.home-assistant.io/redirect/supervisor_add_addon_repository/?repository_url=https%3A%2F%2Fgithub.com%2Fpacorreia%2Fhassio-addons)

1. Install this App in your HAOS instance.
2. The operating mode of Neolink defaults to `RTSP`. If you prefer `MQTT`, please change it within the App configuration. Or select `DUAL` if you want to use RTSP and MQTT in parallel.
3. Create the configuration file named `neolink.toml` in your HAOS `/addon_configs/a14d3924_neolink-latest/` folder.
   - For configuration please follow [these](https://github.com/QuantumEntangledAndy/neolink#configusage) instructions.
   - Sample config file can be found [here](https://raw.githubusercontent.com/QuantumEntangledAndy/neolink/master/sample_config.toml).
4. Start the App and check the log output.
5. The log level defaults to `INFO`. You can set it to error, warn, info, or debug. Most users can leave it at info, but debug can be helpful if you have issues.


[aarch64-shield]: https://img.shields.io/badge/aarch64-yes-green.svg?style=for-the-badge
[amd64-shield]: https://img.shields.io/badge/amd64-yes-green.svg?style=for-the-badge
