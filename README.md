# audible-at-speed
Play Audible speed fast than default by downloading the books then modifying cozy to play them faster than cozy defaults. This is on the arch based system useing nvidia gpu. And it is a guide.

## Get distrobox

install distrobox with 

``sudo pacman -Syu distrobox``

https://distrobox.it/ 

next install podman

``sudo pacman -Syu podman``

## download books

Run to make a distrobox to run Libation in. I couldent get it to work with yay straght in arch

``distrobox-create --nvidia -n Libation-dowload-books --image debian:latest``
``distrobox enter Libation-dowload-books``


To install libation in the distrobox by you need to cahngeing "xx" to the lated verion and running 

``wget -O libation.deb https://github.com/rmcrackan/Libation/releases/download/vX.X.X/Libation.X.X.X-linux-chardonnay.deb && sudo apt install ./libation.deb``

### or 

or dowload** from https://github.com/rmcrackan/Libation/releases/ and then cd to that derctory. and run 

``sudo apt install ./libation.deb``

next use the ui to dowload the books

to make the app acceibu to you with out using distrobox run 

``distrobox-export -a libation``



apt-get install desktop-file-utils

pip3 install PyGObject



https://github.com/rmcrackan/Libation
