# SubNetFieldKit
Open source appliance to collect basic network info on scene.

Build / Install:

Under Releases you can download the latest pre-built binary.

After downloading SubNetFieldKit_vXXX.img.xz :
xz -d SubNetFieldKit_vXXX.img.xz

Image your MicroSD card with above .img file
(on linux you could use):
sudo dd if=SubNetFieldKit_vXXX.img of=/dev/sdYOURMICROSDCARD bs=100M status=progress

After flashing install MicroSD card in Raspberry Pi 4 and enjoy

Defaults:
SSH Enabled
Default User: kali / SubNetFieldKit (Please change)

After you plug the SubNetFieldKit into a target network, connect a USB Flash drive and the power - after the activty light has stopped flashing your Report file will be written to the flash drive (if it hasn't try power cycle and give it about 4 minutes before checking the flash drive)


If you set the URL= value to a webhook you can get real-time info as the SubNetFieldKit is performing its collection.

Edit: /etc/NetworkManager/dispatcher.d/on_new_connection.sh and look for the URL="" value.

More to come!




