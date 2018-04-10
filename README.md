# Electron

Instalar electron:

    npm install –g electron

### Generar .deb

Instalar los siguintes paquetes de manera global:

    $ npm install -g electron-installer-debian
    $ npm install -g electron-packager

Agregar plataforma Debian:

    $ electron-packager . app --platform linux --arch x64 --out dist/

Generar instalador .deb:

    $ electron-installer-debian --src dist/app-linux-x64/ --dest dist/installers/ --arch amd64

Se generará un archivo en 'dist/installers', el cuál una vez instalado estará disponible en '/usr/lib'.

---

Fuentes:

+ https://github.com/electron/electron-quick-start
+ http://photonkit.com/components/
+ https://libraries.io/bower/photon
+ https://github.com/unindented/electron-installer-debian