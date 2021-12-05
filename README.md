# perso-linux
1st linux experience on ubuntu

Liste des actons à mener pour un setup complet pour jouer la création musicale et peut être le montage vidéo

#Régler problèmes audio
https://help.ubuntu.com/community/SoundTroubleshootingProcedure
killall pulseaudio; pulseaudio -k  ; rm -r ~/.config/pulse/* ; rm -r ~/.pulse*
attendre quelques secondes
fermer discord si ouvert
pulseaudio --start
rouvrir discord et autres
si autres problèmes https://docs.google.com/document/d/1iTlJ8BfqXUjaHO__TEdlkvuqB1WLOkGaudngc5SFLMI/edit

#installer gpt3
open ai gpt3 install
check this https://jman4190.medium.com/how-to-build-a-gpt-3-chatbot-with-python-7b83e55805e6

#i2c procedure
https://stackoverflow.com/questions/42904712/i2c-not-detecting-issues-in-hardware-or-any-other

comment monter un iso sur une cl2 usb : //https://askubuntu.com/questions/995661/how-to-install-rufus-on-ubuntu-mate
sudo fdisk -l 
umount /dev/sdc1 #si sdc1 est le disque qui a été monté
sudo dd if=filename.iso of=/dev/sdc bs=4M
sync   
sudo eject /dev/sdc
