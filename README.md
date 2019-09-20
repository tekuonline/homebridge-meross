# Homebridge Meross

## Setup

Assuming you have a working homebridge setup, this is how you add the
meross plugin:

- `npm i -g homebridge-meross-plug` (You may need `sudo` depending on
  your homebridge setup)
- Edit your `config.json` to include the plug `name`, `channel`, &
  `deviceUrl`.

If you're setting this plug up fresh, make sure you go through the
typical meross app for initial setup. You will need to know what the
plugs IP address is on your network & the channel that plug is running on.

``` json
{
  "accessories": [
    {
	      "accessory": "Meross",
	      "name": "Bedroom lamp",
	      "deviceUrl": "http://192.168.1.5",
	      "hardwareVersion": 1,
	      "channel": 0,
        "username":"test@gmail.com"
        "password":"xxxxx"
	      "deviceUrl": "http://192.168.11.11"
	      "messageId": "ea3a20d62868f6c709b6e1b8aeab1ecc",
	      "timestamp": 1550640748,
	      "sign": "9430a84459d15a522a8cb91c93f63b45"
	    }
  ]
}
```
