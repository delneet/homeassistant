[HomeAssistant](https://home-assistant.io) version 0.58

Currently running as a manual install on a raspberry pi zero.

## To Do

- [ ] Hassbian or virtualenv install
- [ ] Ansible configuration
- [ ] Run Mosquitto externally
- [ ] Graphite database

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

