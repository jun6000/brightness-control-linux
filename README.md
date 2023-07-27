# brightness-control-linux
## Features
- Adjust display brightness level by changing adding to value of brightness file `/sys/class/backlight/<vendor>/brightness`.
- Get current brightness level in console.
> By default, regular users are not allowed to modify the contents of the brightness file. To enable users of the group `video` to modify the brightness value, follow [these steps](https://wiki.archlinux.org/title/Backlight#:~:text=By%20default%2C%20only,can%20be%20used%3A).
## Installation
- Clone this repo, make the scripts executable and run them.

  ```
  git clone git@github.com:jun6000/brightness-control-linux.git
  cd brightness-control-linux
  chmod a+x adjust-brightness get-brightness
  ./get-brightness
  ```
## Usage
`./adjust-brightness <[-]value>` - Adjust brightness level by appending value / -value to the script.

`./get-brightness` - Get current brightness level.
