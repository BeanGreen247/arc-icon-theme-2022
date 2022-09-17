# Arc Icon Theme

Notes added by BeanGreen247
* This project may or may not contain new items or elements. It is mainly created to keep the arc theme project alive and have yet another source for it.

**Note:** This is still unfinished. It may not work as expected in some cases.

At the moment this theme mainly includes icons for folders and mimetypes.

### Requirements

This theme doesn't provide application icons, it needs another icon theme to inherit them.
By default this theme will look for the [Moka icon theme](https://snwh.org/moka) to get the missing icons. If Moka is not installed it will use the Gnome icon theme as fallback.
To change the application icons, edit `Arc/index.theme` and replace `Moka` with the name of your preferred icon theme

For example, if you like the Faenza icon theme, change

    [Icon Theme]
    Name=Arc
    Inherits=Moka,Adwaita,gnome,hicolor
    Comment=Arc Icon theme

to

    [Icon Theme]
    Name=Arc
    Inherits=Faenza,Adwaita,gnome,hicolor
    Comment=Arc Icon theme

### Installation

Installation via autotools:

    git clone https://github.com/BeanGreen247/arc-icon-theme-2022 --depth 1 && cd arc-icon-theme-2022
    ./autogen.sh --prefix=/usr
    sudo make install

Alternatively you may copy the `Arc` folder to `~/.icons` or to `/usr/share/icons` for system-wide use.

### Uninstall

Run

    sudo make uninstall

from the same directory as this README resides in, or

    sudo rm -rf /usr/share/icons/Arc

### Preview
![Preview](/img/yCO1aeP.png)

License: GPLv3
