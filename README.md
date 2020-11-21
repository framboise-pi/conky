
<code>sudo apt install fonts-font-awesome</code>
* https://linuxpedia.fr/doku.php/personaliser/conky/fonctions
* https://fontawesome.com/v4.7.0/cheatsheet/


# Conky Boot
  Créer le fichier conky.sh
    sudo nano /usr/bin/conky.sh
 
      #!/bin/sh
      (sleep 4s && conky) &
      exit 0

  Créer le fichier conky.desktop
    sudo nano /etc/xdg/autostart/conky.desktop

      [Desktop Entry]
      Name=conky
      Type=Application
      Exec=sh /usr/bin/conky.sh
      Terminal=false
      Comment=system monitoring tool.
      Categories=Utility;
