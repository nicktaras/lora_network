# lora_network

A short guide to set up a gateway to the lora network 

1. sudo apt-get install git
2. sudo raspi-config (turn on SPI)
3. sudo apt-get install wiringpi
4. cd /home/pi git clone https://github.com/dragino/dual_chan_pkt_fwd
5. make all (ensure you are within the correct dir)
6. sudo ./dual_chan_pkt_fwd
7. locate 'GatewayID' e.g. b827ebffff783b7f
8. sudo make install

Commands:

systemctl start dual_chan_pkt_fwd

systemctl stop dual_chan_pkt_fwd

systemctl status dual_chan_pkt_fwd

To see gateway log in real time:

sudo journalctl -f -u dual_chan_pkt_fwd

references:

http://www.dragino.com/downloads/downloads/LoRa-GPS-HAT/LoRa_GPS_HAT_UserManual_v1.0.pdf

https://github.com/Lora-net/packet_forwarder/wiki/Use-with-Raspberry-Pi

https://www.dragino.com/products/lora/item/106-lora-gps-hat.html

https://wiki.dragino.com/index.php?title=Lora/GPS_HAT

http://wiki.dragino.com/index.php?title=Use_Lora/GPS_HAT_%2B_RaspberryPi_to_set_up_a_Lora_Node

https://www.dragino.com/products/lora/item/149-lora-gps-hat.html

https://www.dragino.com/news/item/107-dragino-release-lora-gps-hat.html

http://www.iot.org.au/wp/wp-content/uploads/2016/12/IoTSpectrumFactSheet.pdf

Support:

support@dragino.com
