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
