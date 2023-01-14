# fancyalice66-vial
fancyalice66 firmware I mucked with for added vial support

Spent way to much time digging through firmware and forums to not share this - going to try and clean it up eventually. 

## What you get
- fancyAlice66 firmware with support for VIAL 
  - Flash the *_vial.hex to your board for vial support
  - the rest of the qmk related files are here if you want to re-build or anything
## Some notes
- I removed the encoder knob code from this because it was throwing compiler errors -- also mine doesn't have an encoder knob 
- Originally written/maintained by github user chent7 <https://github.com/chent7>
## Things to fix if I get to it
- re-add encoder support 
- add secure unlock combo, as of now VIAL_INSECURE is set to yes.
- fix keymapping, removed encoder code bits but didn't mess with the keymapping as it seemed to be ok.
- Several features are disabled as of now to save on firmware size, right now it's 26028/28672 (90%, 2644 bytes free) not sure if being that close to full is ok but may try to reduce other ways
### things that are disabled to save space: 
- QMK_SETTINGS
- TAP_DANCE_ENABLE
- COMBO_ENABLE
- KEY_OVERRIDE_ENABLE
