audio_hdmi_amd-nvidia
============
OS X AMD/Nvidia discrete graphics HDMI audio

PEG0/P0P2/NPE3/P0P1, etc. ???
1. [Guide]-OSX-hdmi_audio-hdef_audio-ssdt_v3, https://github.com/toleda/audio_hdmi_guides

SSDTs
A. Nvidia discrete graphics (Nvidia HDMI Audio)
1. ssdt_hdmi-nvidia-NPE3
Supports IOReg/NPEs display device name

2. ssdt_hdmi-nvidia-P0P1
Supports IOReg/P0P1 display device name

3. ssdt_hdmi-nvidia-P0P2
Supports IOReg/P0P2 display device name

4. ssdt_hdmi-nvidia-PEG0
Supports IOReg/PEG0 display device name

B. AMD discrete graphics/default framebuffer (AMD HDMI Audio)
1. ssdt_hdmi-amd_default-NPE3
Supports IOReg/NPEs display device name

2. ssdt_hdmi-amd_default-P0P1
Supports IOReg/P0P1 display device name

3. ssdt_hdmi-amd_default-P0P2
Supports IOReg/P0P2 display device name

4. ssdt_hdmi-amd_default-PEG0
Supports IOReg/PEG0 display device name

C. AMD discrete graphics/framebuffer injection (AMD HDMI Audio)
Edits required: Model/eevice)id/framebuffer/number of connectors
1. ssdt_hdmi-amd_fb_inj-NPE3
Supports IOReg/NPEs display device name

2. ssdt_hdmi-amd_fb_inj-P0P1
Supports IOReg/P0P1 display device name

3. ssdt_hdmi-amd_fb_inj-P0P2
Supports IOReg/P0P2 display device name

4. ssdt_hdmi-amd_fb_inj-PEG0
Supports IOReg/PEG0 display device name

D AMD discrete graphics/framebuffer injection/Examples (AMD HDMI Audio)
1. ssdt_hdmi-hd6670-Muskgrass-P0P1
Supports sapphire hd6670-Muskgrass-IOReg/P0P1

2. ssdt_hdmi-amd-hd6870-P0P1
Supports sapphire hd6870-Duckweed-IOReg/P0P1

3. ssdt_hdmi-amd-hd7750-PEG0
Supports sapphire hd7750-Dashimaki-IOReg/PEG0

4. ssdt_hdmi-amd-r9_380-P0P2
Supports sapphire r9_380-Greyhound-IOReg/P0P2

Nvidia HDMI Audio
1. Nvidia discrete graphics (4xx, 5xx, 6xx, 7xx, 9xx*, etc, * web driver)
2. DP/HDMI/DVI audio: native (except: 450, 550*, 550ti*, 560*, 560ti*, * fix available)

AMD HDMI Audio
1. AMD HD 5xxx/HD 6xxx/HD 7xxx/R7-R9 2xx/R7-R9 3xx
2. DP audio: not native, frame buffer specific edits
3. Note: specific manufacturer/model may make native DP audio
4. Example: Sapphire HD6870 Vapor-X/Duckweed native (2x DP, HDMI,2x DVI)*
5. HDMI audio: not native, framebuffer specific edits
6. Note: specific manufacturer/model may make native HDMI audio
7. Example: Sapphire HD 7750 Low Profile/Dashimaki with edits (DP, HDMI)*
8. TrueAudio supported in 10.10.4 and newer
9. DVI audio: not supported
* See [Case Studies]..., https://github.com/toleda/audio_hdmi_guides

Installation (included in download)
1. [Guide]-OSX_ssdt-installation

Problem Reporting
1. [Guide]-OSX-hdmi_audio-hdef_audio-ssdt_v3, https://github.com/toleda/audio_hdmi_guides
2. Post to:
   1. http://www.insanelymac.com/forum/topic/301137-yosemite-applehda-hdmi-audio/
   2. http://www.tonymacx86.com/hdmi-audio/143760-audio-hdmi-audio-applehda-guide.html#post886766

toleda
https://github.com/toleda/audio_hdmi_amd-nvidia
README.txt