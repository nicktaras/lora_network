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

https://wiki.dragino.com/index.php?title=Getting_GPS_to_work_on_Raspberry_Pi_3_Model_B (GPS)

https://console.thethingsnetwork.org/gateways

https://larsimmisch.github.io/pyalsaaudio/pyalsaaudio.html

Support:

support@dragino.com

Raspberry PI

https://raspberrytips.com/add-microphone-raspberry-pi/

https://learn.adafruit.com/usb-audio-cards-with-a-raspberry-pi/figure-out-your-chipset

https://www.scipy.org/install.html

https://gist.github.com/notalentgeek/48aeab398b6b74e3a9134a61b6b79a36

https://github.com/aubio/aubio/issues/78

https://stackoverflow.com/questions/33851379/pyaudio-installation-on-mac-python-3
xcode-select --install
brew remove portaudio
brew install portaudio
pip3 install pyaudio

https://github.com/tyiannak/pyAudioAnalysis

https://github.com/aubio/aubio/blob/master/python/demos/demo_pyaudio.py

https://aubio.org/doc/latest/

https://wiki.python.org/moin/PythonInMusic

http://librosa.github.io/librosa/feature.html

Useful CLI CMDs'

- pydoc modules, check modules are correctly installed
- arecord -D plughw:1,0 test.wav (Record from default mic input - steam to output of test.wav)
- brew switch python 3.6.5_1 for pyAudio

reading: https://github.com/Adobe-Marketing-Cloud/aem-dialog-conversion/blob/master/content/jcr_root/libs/cq/dialogconversion/content/sample/classic/dialog/.content.xml
