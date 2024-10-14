# X Plus 4 config files

WIP and very much under construction, do not install on your printer without ability to revert.

if you want to test, in the meantime, here are ssh commands to install:
```
cd /home/mks/printer_data/config/
git clone https://github.com/qidi-community/config-xplus4
sed -i '/<---------------------- SAVE_CONFIG ---------------------->/i [include config-xplus4/*]' printer.cfg
```
then do a firmware restart.
