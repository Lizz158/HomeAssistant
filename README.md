# Home Assistant Automations for Vegetable Seedling Propagation Station

This repository contains Home Assistant automations, helpers, templates and MQTT integrations that run a modular indoor seedling propagation station for vegetable crops.
The system maintains consistent early growth conditions by monitoring and reacting to micro‑climate parameters and plant development phases.

What it does

    Phase‑based profiles (germination → early growth → fully grown seedling ready to be planted outside) with culture‑specific setpoints.
    Lighting control (photoperiod + adaptive dimming via 0–10 V).
    Heat the substrate with heating mats (hysteresis / two‑point control).
    Ventilation cycles for stem strength & moisture management.
    Soil moisture, substrate temperature, air temperature & RH monitoring (virtual VPD derivable).
    Alerting on threshold breaches (dry substrate).
    Local-first design (Home Assistant running on Raspberry Pi 3), only the Dreo vent needs the Dreo cloud, but it doesn't work great for the seedling station anyways and is only a temporary solution.
    Make cool time lapses and look at your plants growing! 

Tech stack

    Home Assistant, MQTT (publish/subscribe telemetry + commands), ESP8266 microcontroller, BH1750 (light), BME680 (air temp/RH), DS18B20 (substrate temp), Capacitive soil moisture sensor V2.0 (soil RH), 0–      10 V dimmed LED grow lights, heating mats, Wi‑Fi fan, camera. 

Goals

    Grow compact and resilient seedlings for your vegetable garden.  
    Create adjustable microclimates depending on plant culture and growth stage. 
    Low-cost, extensible and scalable architecture for small-scale seed germination and plant cultivation. 
