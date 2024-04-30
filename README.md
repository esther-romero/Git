# Curso Git

## Instalación de Git

Para instalar Git en Windows, macOS o Linux, se puede descargar desde la página oficial de [Git](https://git-scm.com/).

Verificar la instalación de Git con el siguiente comando:

```bash
git --version
```

## Configuración de Git

Configurar el nombre de usuario y el correo electrónico con los siguientes comandos:

```bash
git config --global user.name "Nombre Apellido"
git config --global user.email "
```

## Crear un repositorio

Para crear un repositorio, se puede utilizar el siguiente comando:

```bash
git init
```

## Estado del repositorio

Para ver el estado del repositorio, se puede utilizar el siguiente comando:

```bash
git status
```

### Tipos de estados del repositorio

- **Modified**: Archivos que han sido modificados.
- **Staged**: Archivos que están en el stage.
- **Committed**: Archivos que han sido guardados en el repositorio.

## Seguimiento de archivos

Para agregar un archivo modificado al stage, se puede utilizar el siguiente comando:

```bash
git add <archivo>
```

Para agregar todos los archivos modificados al stage, se puede utilizar el siguiente comando:

```bash
git add .
```

## Crear un commit

Para crear un commit con los archivos en el stage, se puede utilizar el siguiente comando:

```bash
git commit -m "<mensaje>"
```

### Historial de commits

Para ver el historial de commits, se puede utilizar el siguiente comando:

```bash
git log
```
