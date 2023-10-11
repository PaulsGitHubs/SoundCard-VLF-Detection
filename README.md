# SoundCard-VLF-Detection
Use your computers sound card to detect radio frequencies within the VLF range

*Sample visualization of VLF signals captured using a sound card.*
![Screenshot 2023-10-11 024638](https://github.com/PaulsGitHubs/SoundCard-VLF-Detection/assets/102178068/7bec3ec5-15d8-4b82-95b2-60b376215035)
![Screenshot 2023-10-11 024618](https://github.com/PaulsGitHubs/SoundCard-VLF-Detection/assets/102178068/d7c10560-1385-4b3a-b716-e44614cd9f5e)

## Table of Contents

- [Introduction](#introduction)
- [Prerequisites](#prerequisites)
- [Setup Guide](#setup-guide)
- [Python Scripts](#python-scripts)
- [Contributing](#contributing)
- [License](#license)

## Introduction

The VLF range is a fascinating portion of the RF spectrum, encompassing frequencies from 3 kHz to 30 kHz. While typically explored using specialized equipment, this project seeks to experiment with standard computer sound cards for VLF signal capture and analysis.

## Prerequisites

- Download RelWithDebInfo.zip off Osmocom.org and set the directory for /x64 or /x32 to path in system variables on windows https://osmocom.org/attachments/2242
- A computer with a microphone or line-in jack. Soundcard should at least be able to operate within 48khz.
- [Spectrum Lab Software](https://www.qsl.net/dl4yhf/spectra1.html)
- Python 3.x
- Required Python Libraries: pyrtlsdr==0.2.91, numpy, matplotlib, scipy

## Setup Guide

1. **Antenna Creation**:  
   Create a loop antenna using any available wire and connect it to the microphone or line-in jack of your computer.

2. **Spectrum Lab Configuration**:  
   - Configure Spectrum Lab to capture audio from the connected sound card input.
   - Adjust the frequency range to focus on the VLF band.
   - [More detailed steps here.](./docs/spectrum_lab_setup.md)

3. **Python Script Execution**:  
   - Use the provided Python scripts to analyze captured signals, extract features, and visualize the VLF range.
   - [More on Python scripts usage here.](./docs/python_scripts_guide.md)
