
# Instalar el entorno (environment) de trabajo

## ¿Qué es un ambiente virtual y qué ventajas tiene?

Un **ambiente virtual** es un entorno aislado de Python que permite gestionar dependencias específicas por proyecto sin interferir con otros entornos. Sus ventajas incluyen:
- **Aislamiento de dependencias**: Cada proyecto usa sus propias librerías y versiones.
- **Reproducibilidad**: Garantiza que el entorno funcione igual en diferentes máquinas.
- **Evita conflictos globales**: No afecta a las librerías instaladas a nivel del sistema.

## ¿Para qué sirve *Poetry*?

*Poetry* es una herramienta para gestión de dependencias y empaquetado en Python. 
Automatiza:
- Creación y gestión de entornos virtuales.
- Manejo de dependencias utilizano archivo `pyproject.toml`.
- Empaquetado y publicación de librerías.

## ¿Cómo instalar *Poetry*?

```bash
curl -sSL https://install.python-poetry.org | python3 -
```

**Nota:** Instalar software de esta manera puede ser inseguro. 
La cadena de confianza en este software está en los administradores del dominio `python-poetry.org`. 


### Verifica la instalación:
```bash
poetry --version
```

## ¿Cómo instalar nuestro ambiente de desarrollo (virtual) con *Poetry*?

El archivo `pyproject.yml` contiene la descripción y los paquetes mínimos para comenzar. 
Si se requiren otros paquetes o dependencias, estás pueden ser agregadas de la siguiente manera:

### Instalar todo el proyecto (ambiente de trabajo)
   ```bash
   poetry install
  ```



### Agregar dependencias:
   ```bash
   poetry add ipython
   ```

## Activar el ambiente de trabajo
   ```bash
   poetry shell
   ```

## Comenzamos 🚀 !
```bash
ipython
```


