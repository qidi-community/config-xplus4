# X Plus 4 config files

WIP and very much under construction, do not install on your printer without ability to revert.

if you want to test, in the meantime, ssh into on the printer with the following:
(Extended documentation about SSH access [here](https://github.com/qidi-community/Plus4-Wiki/blob/main/content/ssh-access/README.md))
```
ssh mks@[printer's IP]
```

Password is: `makerbase`

Next, copy this, paste it and press enter.
```
cd /home/mks/printer_data/config/ && git clone https://github.com/qidi-community/config-xplus4 && sed -i '/<---------------------- SAVE_CONFIG ---------------------->/i [include config-xplus4/*.cfg]' printer.cfg
```
then do a firmware restart.

if you already installed, the current update procedure is pasting and running this line: 
```
cd /home/mks/printer_data/config/ && rm -rf ./config-xplus4/ && git clone https://github.com/qidi-community/config-xplus4 
```
then do a firmware restart. Beware that if you had done any modifications to the mods stored in the `config-xplus4` folder, they'd be erased by this action. 
