# BareDev - A small, yet resourceful keyboard


An open-source, QMK-compatible, ABNT2-based 70% keyboard, focusing in a smaller footprint while retaining all the functions found on a TKL (Del and arrow keys doubling as the navigational cluster)

---

Layout:

![Keyboard Layout](./images/layout_render.png)

Links: [KLE](http://www.keyboard-layout-editor.com/#/gists/89e76130aa221e028ccd5b3f6dec0909), [JSON](https://gist.github.com/ManoShu/89e76130aa221e028ccd5b3f6dec0909), [QMK](https://github.com/qmk/qmk_firmware/tree/master/keyboards/handwired/baredev/rev1)

---

## PCB & Case
![PCB preview on KiCad](./images/pcb_preview.png)
![Prototype case](./images/proto_case.png)

Note: this photo is of an early prototype of the case. The uploaded files has been updated to require less total area and WILL look slighty different than shown (the overall dimensions remain the same).


The case and gerber files are under `production`. The had been used and confirmed to work, however use them at your own risk.

## QMK

The rev1 has been integrated in the [main QMK repository](https://github.com/qmk/qmk_firmware/tree/master/keyboards/handwired/baredev/rev1), being able to use the [online configurator](https://config.qmk.fm/#/handwired/baredev/rev1/LAYOUT_abnt2) to generate the firmware while also having the files on the `qmk` directory here in case of you don't want to update your fork (HOWEVER the files have been confirmed working on QMK 0.2.2 [check yours with `qmk --version`], previous versions might not have support for some of the tags in the` info.json` file)

## VIA / VIAL

A `via` keymap is available allowing to use VIA to change keybindings without the need to setup QMK. 
It is not integrated with the official repository yet, but the .json file required to change bindings is available on the `via` directory.

A VIAL-compatible keymap is also available. It is on the official repository, but in case you don't want to update, just drop the keyboard folder to your `vial-qmk` directory and it should also work right off the bat.