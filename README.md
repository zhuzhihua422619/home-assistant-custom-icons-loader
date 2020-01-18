# Custom Icon Loader - [Home Assistant](https://www.home-assistant.io/) integration

Allow you to use your own icons in Home Assistant. No more static images ! Using svg icons allows for them to dynamically react to the state of your entities, like the brightness or the color of a light.

![A svg icon allow it to be dynamic](https://raw.githubusercontent.com/Armaell/home-assistant-custom-icons-loader/master/img/with-without.png)

## Installation
You need to add in your `configuration.yaml` the following line :  
`custom_icons:`  
Then use one of the following methods :

### With [![hacs_badge](https://img.shields.io/badge/HACS-Custom-orange.svg?style=for-the-badge)](https://github.com/custom-components/hacs)
If you use HACS, you can add this repository as a custom one. Go to the settings, and fill as following :
- Custom repository : 'armaell/home-assistant-custom-icons-loader'
- Category : Integration


### Manual Installation

Copy the folder `custom_components` of this repository into the `custom_components` inside your Home Assistant folder.

## Usage

### Create a icon file
Go to [Fontello](http://fontello.com/).  
Select icons you wish to use and/or add your own svg icons. Then download your archive.  
Move the archive to the `custom_icons` folder.

- The `custom_icons` folder will be created at the root of your Home Assistant folder, or create it yourself.  
- You can add as many files as you want.

### Use your icon
Once the file placed, reload Home Assistant.  
You can now use your new icons in a similar fashion than stock mdi icons, but with `custom:` prefix. By example, if you added 'git' icon :  
  
![How to use your icon](https://raw.githubusercontent.com/Armaell/home-assistant-custom-icons-loader/master/img/use-icon-in-lovelave.png)

### Alternative prefixes
You can use other prefixes than `custom:` by creating a subfolder inside the `custom_icons` folder. By example `custom_icons/room` will make the icons inside this folder available with the `room:` prefix.

## Credits
The icon used in the example has been made by [Pixel perfect](https://www.flaticon.com)  
The code from `template.js` and `custom_component_server.py` are from [thomasloven](https://github.com/thomasloven/hass-fontawesome)