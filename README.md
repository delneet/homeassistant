[HomeAssistant](https://home-assistant.io) version 0.58

Currently running as a manual install on a raspberry pi zero.

## To Do

- [ ] Hassbian or virtualenv install
- [ ] Ansible configuration
- [ ] Run Mosquitto externally
- [ ] Graphite database
- [x] ~Mopidy and snapcast ([link](https://home-assistant.io/blog/2016/02/18/multi-room-audio-with-snapcast/))~
- [ ] [HomeBridge](https://github.com/home-assistant/homebridge-homeassistant)

## Devices

* Chromecast 2x
* Philips Hue starter kit
* Spotify via [raspotify](https://github.com/dtcooper/raspotify) running locally

## Configurations

### External access

* DNS via DuckDNS (updates with crontab entry)
* SSL certificates via LetsEncrypt (via _dehydrated_, updates with crontab entry)

## Maintenance

#### Upgrade

`sudo pip3 install --upgrade homeassistant`

#### Restart

`sudo systemctl restart home-assistant`

#### Log

`sudo journalctl -f -u home-assistant`

## MySensors

### Gateway

MySensors gateway has been installed, to add to the boot run:
`sudo systemctl enable mysgateway.service`

To start the gateway run:
`sudo systemctl start mysgateway.service`

## Resources

* [Using a usb audio device on a raspberry-pi zero](https://raspberrytips.nl/usb-audio-gebruiken-op-een-raspberry-pi/)
