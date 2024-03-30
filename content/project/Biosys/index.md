---
title: Microfluidic biochips synthesis system control program based on STM32
summary: Supervised by Prof. Zhengchun Liu at CSU. (Key Support Project of Hunan Province College Innovation and Entrepreneurship)
tags:
  - Demo
date: '2021-04-27T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: Photo by rawpixel on Unsplash
  focal_point: Smart

url_code: 'https://github.com/Han-0107/BioSys_STM32'
url_pdf: ''
url_slides: ''
url_video: ''

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# slides: example
---

## Overview

The project enables the delivery of various reagents such as cleaning agents and de-protective agents to the reaction tank. Then STM32 is used to control the modular transport of reagents, shorten the transport process of reagents, and reduce the consumption of reaction reagents. A precision injection pump is used to deliver the reagent to the microfluidic chip for pre-activation, and then the steering command is sent to the six-way valve through RS485 bus to realize the switch between the reagents. The STM32 collects data from external sensors and monitors the entire process via an LCD touch screen. Finally, each sub-module is optimized and improved, and then these sub-modules are combined into a complete system, so that this system can realize the synthesis of biochips under the control of STM32.

Starting from the science and technology of preparing peptide nucleic acid biochips, this project aims to build an in situ synthesis system of biochips based on STM32 control, explore scientific issues such as six-way solenoid valve and liquid inlet pump cooperative transport of reagents, STM32 automation control, and carry out research in the following aspects: (1) Research on fluid transport system of reaction reagents; (2) Research on STM32 electronic control system.

## Embedded control system

The STM32 internal program is used to control the running state of the precision liquid inlet pump and the switching valve to achieve the purpose of controlling the whole system. Send a high level command to the pump connected to the cleaning agent, and then send the cleaning port steering command to the six-way valve to realize the delivery of the cleaning agent to the reaction pool. Send switching instructions to the switching valve between cleaning agents to realize switching between cleaning agents. The vent valve is normally open. When the STM32 sends the command to turn to the drying port to the six-way solenoid valve, the inert gas enters the reaction pool directly through the six-way valve to realize the drying step. When the upper computer simultaneously delivers the reagent and activator pump high power level, the reagent will enter the microfluidic chip for real-time activation. 

STM32 can activate different reagents separately by controlling the switching valve of the activator. The de-protected reagent is separately controlled by a pump, separated from the activated reagent through a switch valve in front of the reaction tank, and directly enters the reaction tank. The whole system is powered by a multilevel switching power supply, and the relay is used to connect the pump and valve to realize the purpose of developing the board pin low level control high level device. The six-way valve communicates with the development board through RS485, and the STM32 sends the hexadecimal steering command to the six-way valve to turn to 64 bits at a specific time, thus controlling the switching between various reagents.

An LCD touch screen is designed on the STM32 development board to monitor the system process through data acquisition card and sensor. Keil software was used to carry out embedded development of STM32, designed the running code of each sub-module, including cleaning, drying, de-protection, pre-activation and other modules, and then carried out hardware testing and program optimization for each module. Finally, each module is formed into a complete system, which is tested and optimized on the built hardware system.
