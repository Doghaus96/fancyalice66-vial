# fancyalice66-vial
fancyalice66 firmware I mucked with for added vial support

Spent way to much time digging through firmware and forums to not share this - going to try and clean it up eventually. 

## What you get
- fancyAlice66 firmware with support for VIAL 
  - Flash the *_vial.hex to your board for vial support
  - the rest of the qmk related files are here if you want to re-build or anything
- And im throwing in my vial key layout, 
  - adds super to the key left of the left spacebar ( I use a mac at work so CMD is helpful to have)
  - Rebinds caps lock to Control (HHKB style, I rebind all my caps lock keys like this now) 
  - Caps lock is now on layer one, so MO(1)+caps gives you caps) 
  - moved tilde key (~) to page down. I work in linux, that tilde is important. 
  - Why am I defending my keyboard layout? whats wrong with me? 
## Some notes
- I removed the encoder knob code from this because it was throwing compiler errors -- also mine doesn't have an encoder knob 
- Originally written/maintained by github user chent7 <https://github.com/chent7>
  - you can find the original via firmware on chent7's page if just need that (because you goofed and bricked your keyboard like me)
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
