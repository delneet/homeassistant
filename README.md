[HomeAssistant](https://home-assistant.io) config for version 0.106.5

Running in docker on core-os

## To Do

- [ ] Ansible configuration
- [ ] Run Mosquitto externally
- [x] ~Mopidy and snapcast ([link](https://home-assistant.io/blog/2016/02/18/multi-room-audio-with-snapcast/))~

## Devices

* Chromecast
* Philips Hue starter kit
* Spotify via [raspotify](https://github.com/dtcooper/raspotify) running on a raspi zero
* Yeelight 2x
* LG webos tv

## Configurations

### External access

* ~DNS via DuckDNS (updates with crontab entry)~
* ~SSL certificates via LetsEncrypt (via _dehydrated_, updates with crontab entry)~

## Maintenance

## MySensors

Not active at the moment

### Gateway

~MySensors gateway has been installed, to add to the boot run:~
`sudo systemctl enable mysgateway.service`

To start the gateway run:
`sudo systemctl start mysgateway.service`

## Resources

* [Using a usb audio device on a raspberry-pi zero](https://raspberrytips.nl/usb-audio-gebruiken-op-een-raspberry-pi/)

