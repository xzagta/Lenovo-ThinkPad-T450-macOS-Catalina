#
# Installing Lenovo T440 TrackPad Files

Files can be found in 
* "/Volumes/ESP/EFI/CLOVER/utilities/TrackPad/T440_One_Button_ClickPad/"

or

* "/Volumes/ESP/EFI/CLOVER/kexts/TrackPad/T440_One_Button_ClickPad/"

Be sure to do the following:

- Run my ".command" located in "/Volumes/ESP/EFI/CLOVER/kexts/TrackPad/T440_One_Button_ClickPad" folder and all required changes will be made automatically. 

*** (MAKE SURE EFI PARTITION THAT CONTAINS CLOVER IS MOUNTED BEFORE RUNNING MY ".command" FILE) ***

If the .command script doesn't work then do the following:

Replace the SSDT-VPS2.aml file in:
* "/Volumes/ESP/EFI/CLOVER/ACPI/patched/"

with SSDT-ASTP.aml file in: 
* "/Volumes/ESP/EFI/CLOVER/kexts/TrackPad/T440_One_Button_ClickPad/"

Replace VoodooPS2controller.kext in the following 3 folders: 
* "/Library/Extensions/" *** (if you installed it there or ran my script to install system kexts) ***
* "/Volumes/ESP/EFI/CLOVER/kexts/Other/"
* "/Volumes/ESP/EFI/CLOVER/kexts/System/" 

with ApplePS2SmartTouchpad.kext that can be found in: 
* "/Volumes/ESP/EFI/CLOVER/kexts/TrackPad/T440_One_Button_ClickPad/"