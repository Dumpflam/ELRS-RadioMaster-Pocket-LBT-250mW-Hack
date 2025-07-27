This is an ELRS firmware that allows 250mw power output while still keeping LBT functionality. Great for when you have an LBT reciever, but you are not in EU so you can use the full 250mW while still keeping LBT.

INSTRUCTIONS:
To build this, install "git" (https://git-scm.com/downloads).
Open Command Prompt and write (cd "%USERPROFILE%\Documents") [Exclude parentheses.].
Then, write (git clone https://github.com/Dumpflam/ELRS-RadioMaster-Pocket-LBT-250mW-Hack) [Exclude parentheses.].
This will clone this repository to your documents folder.
You can close Command Propmpt.
Now, install ExpressLRS Configurator (https://github.com/ExpressLRS/ExpressLRS-Configurator/releases/latest)
Launch ExpressLRS Configurator and navigate to the "Settings" tab.
Under Application Options, enable "Expert Mode".
Now, go back to the "Configurator" tab.
Select "LOCAL" from the top.
Tap "CHOOSE FOLDER" under the "Local path" text-box.
In the file picker, navigate to your Documents folder.
Find "ELRS-RadioMaster-Pocket-LBT-250mW-Hack".
Go inside that folder, then single-click the "src" folder to highlight it and select it. On the bottom right, click "Choose folder" with the "src" folder highlighted.
You should be sent back to the configurator. Under "Target", choose your device category and device.
Choose the recommended "Wifi" flashing method.
Under "Regulatory domains 2.4 GHz band" choose "2.4 GHz LBT (Listen Before Talk)".
If you desire, set up your home wifi network and/or your binding phrase.
All the way below, under "Actions", ***!!!!DO NOT CLICK "FLASH"!!!!***, instead click "BUILD".
WARNING: THIS WILL TAKE A ***LOOONG WHILE*** TO FINISH.
After it's finished, it should automatically open a File Explorer window with TWO .bin files in it. Your firmware is the one that ***ISN'T firmware.bin*** but is the one named according to your device.
To flash this firmware, if you HAVEN'T set up your home network, you can directly connect to your transmitter's wifi hotspot (activated in the lua script)and go to "http://10.0.0.1/", if you HAVE set up your home network, you can go to "http://elrs_tx.local/" and select the "UPDATE" tab to upload the firmware file and wait for it to flash.
Advice while flashing, after upload is done, do not touch the transmitter for about 2 minutes. then, restart the transmitter and check in the lua script if you have the option to go to 250mW even though it says  "100mW CE LIMIT". ***!!!AT FIRST YOU WILL SEE "ERR" OR "---" BUT IT WILL GET FIXED WHEN YOU TRY TO CHANGE IT.!!!***
That's it!
