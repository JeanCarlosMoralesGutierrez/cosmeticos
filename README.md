# Cosmeticos

## Instrucciones de instalación

### 1) Crear entorno virtual

Afuera del proyecto correr este comando: ` python -m venv myvenv`.

### 2) Activar el entorno virtual

Primero tenés que ingresar a la carpeta myvenv con `cd myvenv`.
Una vez ubicado aquí se corre el comando de activación endependencia del sistema operativo.

Para OS X y linux: `source bin/activate`
Para windows: `Scrpts\Activate.ps1`

Una vez activado el entorno virtual habrán unas letras en color a la izquierda de la terminal que dirán (myvenv).

### 3) Agregar .env

Se debe agregar un archivo .env en la raíz de el proyecto, y a esto agregarle:
estas variables:

```
SECRET_KEY="asdfasdf"
STRIPE_TEST_PUBLIC_KEY="asdfasfd"
STRIP_TEST_SECRET_KEY="ASDFASDF"
```

En realidad pueden ser las keys cualquier contenido random.

### 4) Ejecutar migraciones

En la raíz del proyecto ejecutar este comando: `python manage.py makemigrations`
Luego si todo funcionó correctamente este otro comando: `python manage.py migrate`

### 5) Ejecutar el programa

Para correr el programa hay que ejecutar el siguiente comando:
`python manage.py runserver`

### 6) Crear superuser

Ejecuta el siguiente comando:
`python manage.py createsuperuser`

Y luego crea un usuario admin con su nombre de usuario, correo y contraseña, el correo no es obligatorio
