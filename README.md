# Diccionario-de-correccion-ortografica-Español-WPS-Office

Cuando uno descarga el diccionario español España para WPS Office desde:

http://wps-community.org/download/dicts

Nota: A esta fecha 23 de Noviembre del 2019 han retirado esa url no se porqué.

no funciona para WPS Office 2019 por estar vacío el contenido de "main.dic"(que no tenía nada) por esta razón he adaptado el paquete "hunspell-es" (el cual es el diccionario de corrección ortográfica español para LibreOffice) desde los repositorios de Ubuntu:

http://archive.ubuntu.com/ubuntu/pool/main/libr/libreoffice-dictionaries/hunspell-es_6.0.3-3_all.deb 

para que funcione como diccionario para WPS Office 2019

lo que hice fue descargarlo y extraer su contendio y lo que necesitaba estaba aquí:

usr/share/hunspell/es_ES.aff
usr/share/hunspell/es_ES.dic

y cree una carpeta llamada:

es_ES

y allí los pegué. Además pegué allí también el archivo "dict.conf" que lo saqué de la página original de los diccionarios de http://wps-community.org/download/dicts cuando estaban en línea

y al hacer esto si funciona

Detalles del contacto: 

Washington Indacochea Delgado
wachin.id@gmail.com


#Instalación General.

Esto funciona en Manjaro Linux 20.1 Gnome/KDE.


- Clonar el repositorio.
```bash
	git clone https://github.com/RiemaruKarurosu/WPS-Office-Dict-es-ES.git
```


#Instalación con script.

- En caso de que no funcione el script utilizar este comando.
```bash
	chmod 755 install.sh
```

- Instalación
```bash
	sudo ./install.sh
```

#Instalación sin script.

- Copiamos la carpeta `es_ES` al directorio de diccionarios de wps office:

```bash
	sudo cp -r es_ES /usr/lib/office6/dicts/spellcheck
```





