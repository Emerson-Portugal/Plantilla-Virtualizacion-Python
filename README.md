# Virtualizacion en Python
Con estos comandos podras crear un entorno vitual de python en los sistemas operativos de linux y windows

## Requisitos
Requisitos previos, para la creacion de un entorno virtual en python

### Windows
- virtualenv
```
pip install virtualenv
```

### Ubuntu/Debian
- pip3
```
sudo apt install python3-pip
```

- virtualenv
```
pip3 install virtualenv
```

Creacion del entorno virtual en los sistemas operativos:

### Ubuntu/Debian
- Creacion del entorno virual `venv`
```
virtualenv venv -p python3
```
- Activacion del entorno virtual `venv`
```
source venv/bin/activate
```
- Desactivacion del entorno virtual `venv`
```
deactivate
```

### Windows
- Creacion del entorno virual `venv`
```
python -m virtualenv venv
```
- Activacion del entorno virtual `venv`
```
.\venv\Scripts\activate
```
- Desactivacion del entorno virtual `venv`
```
deactivate
```

## Creacion del `requirements.txt`

- Listar las librerias del entorno virtual `venv`
```
pip list
```
- Crear el archivo `requirements.txt` del entorno virtual `venv`
```
pip freeze > "requirements.txt"
```
- Instalacion el archivo `requirements.txt` en un entorno virtual
```
pip install -r ".\requirements.txt"
```

## Plantillas para el script en Python

### Linux

- Sin entorno Virtual
```
#!/usr/bin/python3
# -*- coding: utf-8 -*-
# Autor:
```

- Con entorno Virtual
```
#!/usr/bin/env python3
# -*- coding: utf-8 -*-
# Autor:
```

