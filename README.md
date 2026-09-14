# Restaurante App - Tkinter
## Datos del estudiante

**Nombre**: Bonner Javier García Guanga

---
## Descripción

Restaurante App es una aplicación desarrollada en Python utilizando Programación Orientada a Objetos (POO), persistencia de datos con archivos JSON e interfaces gráficas mediante Tkinter.

La aplicación permite gestionar información de usuarios y productos almacenados localmente. Además, incorpora un sistema de autenticación para acceder a la interfaz principal y visualizar los datos registrados.

El objetivo de esta práctica es aplicar conceptos de organización por capas, reutilización de código, persistencia de información e interfaces gráficas de usuario.

---

## Estructura del proyecto

```text
restaurante_app/
├── datos/
│   ├── productos.json
│   └── usuarios.json
├── modelos/
│   ├── __init__.py
│   ├── producto.py
│   └── usuario.py
├── servicios/
│   ├── __init__.py
│   ├── archivo_servicio.py
│   └── restaurante_servicio.py
├── ui/
│   ├── __init__.py
│   ├── login_view.py
│   └── main_view.py
└── main.py

README.md
``` 

---

## Descripción de carpetas y archivos

### datos

Contiene los archivos JSON utilizados para almacenar la información de forma persistente.

- *productos.json:* almacena los productos registrados.
- *usuarios.json:* almacena los usuarios registrados.

### modelos

Contiene las clases que representan las entidades principales del sistema.

- *producto.py:* define la clase Producto.
- *usuario.py:* define la clase Usuario.

### servicios

Contiene la lógica de negocio y el acceso a los datos.

- *archivo_servicio.py:* permite leer información desde archivos JSON.
- *restaurante_servicio.py:* administra usuarios, productos y validación de acceso.

### ui

Contiene las interfaces gráficas desarrolladas con Tkinter.

- *login_view.py:* pantalla de inicio de sesión.
- *main_view.py:* pantalla principal de la aplicación.

### main.py

Punto de entrada de la aplicación. Inicializa los servicios, carga los datos y muestra la ventana principal.

---

## Flujo de la aplicación

1. El usuario ejecuta el archivo main.py.
2. El sistema carga la información almacenada en los archivos JSON.
3. Se presenta la pantalla de inicio de sesión.
4. El usuario ingresa sus credenciales.
5. El sistema valida el acceso utilizando los usuarios registrados.
6. Si las credenciales son correctas, se muestra la interfaz principal.
7. Desde la interfaz principal es posible visualizar productos y usuarios registrados.
8. El usuario puede cerrar sesión y regresar a la pantalla de inicio.

---

## Vistas implementadas

### LoginView

Permite al usuario ingresar sus credenciales para acceder al sistema.

*Funciones principales:*

- Ingreso de usuario.
- Ingreso de contraseña.
- Validación de acceso.
- Mensajes de error cuando las credenciales son incorrectas.

### MainView

Pantalla principal de la aplicación.

*Funciones principales:*

- Visualización de productos registrados.
- Visualización de usuarios registrados.
- Barra de estado con información general.
- Opción para cerrar sesión.

---

## Requisitos

- Python 3.10 o superior.
- Tkinter (incluido en la instalación estándar de Python).

---

## Ejecución

1. Abrir una terminal en la carpeta restaurante_app.
2. Ejecutar el siguiente comando:

bash
python main.py


3. Ingresar las credenciales registradas en usuarios.json.
4. Utilizar las opciones disponibles dentro de la aplicación.

---

## Tecnologías utilizadas

- Python
- Programación Orientada a Objetos (POO)
- Tkinter
- JSON
- Git y GitHub