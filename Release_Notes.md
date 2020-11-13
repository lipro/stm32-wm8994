---
pagetitle: Release Notes for WM8994 Component Drivers
lang: en
---

::: {.row}
::: {.col-sm-12 .col-lg-4}

::: {.card .fluid}
::: {.sectione .dark}
<center>
# <small>Release Notes for</small> <mark>WM8994 Component Drivers</mark>
Copyright &copy; 2016 STMicroelectronics\
    
[![ST logo](../../../../_htmresc/st_logo.png)](https://www.st.com){.logo}
</center>
:::
:::

# License

Licensed by ST under BSD 3-Clause license (the \"License\"). You may
not use this package except in compliance with the License. You may
obtain a copy of the License at:

[https://opensource.org/licenses/BSD-3-Clause](https://opensource.org/licenses/BSD-3-Clause)

# Purpose

This directory contains the WM8994 component drivers.

:::

::: {.col-sm-12 .col-lg-8}
# Update History

::: {.collapse}
<input type="checkbox" id="collapse-section22" checked aria-hidden="true">
<label for="collapse-section22" aria-hidden="true">V2.3.1 / 03-April-2019</label>
<div>			

## Main Changes

- Update release notes format
- Reformat the BSD 3-Clause license declaration in the files header (replace license terms by a web reference to OSI website where those terms lie)

</div>
:::

::: {.collapse}
<input type="checkbox" id="collapse-section19" aria-hidden="true">
<label for="collapse-section19" aria-hidden="true">V2.3.0 / 24-January-2018</label>
<div>			

## Main Changes

- wm8994.c: fix no audio output issue

</div>
:::

::: {.collapse}
<input type="checkbox" id="collapse-section18" aria-hidden="true">
<label for="collapse-section18" aria-hidden="true">V2.2.0 / 05-June-2017</label>
<div>			

## Main Changes

- Add support of ColdStartup sequence for headphone
  - Unmute is performed in a gradual way to minimize pop noise.
  - Update wm8994_SetFrequency to support AUDIO_FREQUENCY_32K
  - Update comments to be used for PDSC generation


</div>
:::

::: {.collapse}
<input type="checkbox" id="collapse-section185" aria-hidden="true">
<label for="collapse-section185" aria-hidden="true">V2.1.0 / 22-February-2016</label>
<div>			

## Main Changes

- wm8994.c
  - Update wm8994_Init() by adding the support of analog microphone connected to INPUT LINE 1, INPUT_DEVICE_DIGITAL_MICROPHONE_1 and INPUT_DEVICE_DIGITAL_MIC1_MIC2
  - Add AUDIO_FREQUENCY_32K as possible AudioFreq value
- wm8994.h
  - Add INPUT_DEVICE_DIGITAL_MIC1_MIC2 define

</div>
:::

::: {.collapse}
<input type="checkbox" id="collapse-section17" aria-hidden="true">
<label for="collapse-section17" aria-hidden="true">V2.0.0 / 24-June-2015</label>
<div>			

## Main Changes

- wm8994.h 
  - Add codec de-initialization function: wm8994_DeInit()
  - Add Audio IO de-initialization function prototype: AUDIO_IO_DeInit()
  - Add INPUT_DEVICE_INPUT_LINE_1 and INPUT_DEVICE_INPUT_LINE_1 support for AUDIO IN
  - Add Input audio volume control support
- wm8994.c 
  - Update wm8994_Init() function to support the Audio IN
  - Update wm8994_Stop() function to only stop the codec if it was configured
  - Enable VMID_BUF_ENA bit in R57 ANTIPOP register (address 0x39) for all configurations

**[[NOTE]{style="font-size: 10pt; font-family: Verdana; color: black;"}]{.underline}**
This release must be used with BSP Common driver V4.0.0 or later.


</div>
:::

::: {.collapse}
<input type="checkbox" id="collapse-section16" aria-hidden="true">
<label for="collapse-section16" aria-hidden="true">V1.0.2 / 12-February-2015</label>
<div>			

## Main Changes

- wm8994.c: Update the wm8994_Init() function to set the volume after enabling the dynamic charge pump power control mode 


</div>
:::

::: {.collapse}
<input type="checkbox" id="collapse-section165" aria-hidden="true">
<label for="collapse-section165" aria-hidden="true">V1.0.1 / 28-November-2014</label>
<div>			

## Main Changes

- wm8994.h: change "\\" by "/" in the include path to fix compilation issue with Linux


</div>
:::

::: {.collapse}
<input type="checkbox" id="collapse-section15" aria-hidden="true">
<label for="collapse-section15" aria-hidden="true">V1.0.0 / 18-February-2014</label>
<div>			

## Main Changes

- First official release


</div>
:::

:::
:::

<footer class="sticky">
For complete documentation on <mark>STM32 Microcontrollers</mark> ,
visit: [http://www.st.com/STM32](http://www.st.com/STM32)
</footer>
