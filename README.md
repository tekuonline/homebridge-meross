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
      "channel": 0,
      "deviceUrl": "http://192.168.11.11"
    }
  ]
}
```
