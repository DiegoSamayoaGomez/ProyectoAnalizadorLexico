# Proyecto-Final-Analizador-Lexico

## Descripción
Este es un programa en python para ser un pequeño analizador léxico creado como proyecto de diseño de compiladores.
Se busca alcanzar el soporte de varios conceptos fundamentales de programación, como declaración de variables, funciones, condicionales, operaciones básicas y ciclos.
La sintaxis pretende estar basada en el lenguaje BASIC para ser legible y simple. 


El programa fue desarrollado en ```Python 3.9```.

## Archivos necesarios
- Python 3.6 o superior: [Descargar Python](https://www.python.org/downloads/)

Versiones anteriores no funcionarán
- Tkinter: Se selecciona durante la instalación de Python
- Librería SLY: ```pip3 install sly```

## Posibles problemas
Debe de estar seguro de tener todos los archivos instalados correctamente y que la versión de Python sea ```Python 3.6``` o superior.

Es posible que obtenga un error de 'comando no encontrado' en Windows, lo que significa que python no está en su ruta estándar.

Comprueba cómo añadir python a tu ruta aquí: [Configurar ruta de instalación en Python](http://superuser.com/questions/143119/how-to-add-python-to-the-windows-path).

## Arranque
Puede utilizar la interfaz de usuario WINDOW creada con la ayuda de la libreria Tkinter: ```WINDOW.py```.

## Uso
Luego de abrir ```WINDOW.py```, ejecute el archivo en la terminal y se abrirá la interfaz de usuario. Cuando la interfaz esté abierta podrá ingresar sus cadenas de prueba y observar el funcionamiento de programa

## Reglas para el análisis 
-	Las palabras reservadas están creadas en español.
-	Las palabras reservadas deben ser declaradas en  MAYÚSCULAS, por ejemplo: ```SI, SINO, ENTONCES```.
-	La declaración de variables o cadenas de texto serán declaradas en MINÚSCULAS, por ejemplo: ```auto, hola mundo```
-	El programa detectará caracteres no válidos y los reportará.

## Manejo de errores
Si se encuentra un carácter incorrecto durante el análisis, la tokenización continuará. Sin embargo, para manejar los errores de análisis léxico que se producen cuando se detectan caracteres ilegales, el método de ```error()``` recibe un Token en el que la cadena de texto separada en toknes contiene todo el texto restante sin errores. Es decir, este manejador de errores mira este texto y podrá saltarlo sin detener la ejecución.
