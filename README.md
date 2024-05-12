# Curso Git

## 👩🏻‍💻 Datos de la Estudiante

_**Nombre completo:** Esther Romero Aguilar_

---

## Hooks, Alias y Trucos de Git

## 🔤 Hooks

Un hook, o un punto de enganche, es la posibilidad de ejecutar una accion o script cada vez que ocurre un evento en git.

#### Hooks del lado del cliente

Solo afectan al repositorio local que los contiene.

- **pre-commit**:

  - Podrias comprobar si se esta intentando hacer un commit de demasiados archivos.
  - Puede ser un buen sitio para ejecutar el linter sobre los archivos que han sido modificados

- **prepare-commit-msg**:
  - Para modificar el mensaje del commit o añadir cualquier información extra.
- **commit-msg**:

  - Es el sitio perfecto para hacer todas las comprobaciones pertinentes al mensaje.

- **post-commit**:
  - Su uso principal es la de notificar por Slack.
- **pre-push**:

  - Para ejecutar una bateria de tests.

- **post-checkout y post-merge**:
  - Permite limpiar el directorio de trabajo, tras realizar un checkout, o el de limpiar las ramas que ya no se usan tras realizar un merge.

### Desventajas de los Hooks del lado del cliente

Los hooks no se comparten con el repositorio, por lo que si alguien clona el repositorio no tendrá los hooks.

#### Hooks del lado del servidor

Es interesante conocerlos ya que páginas como GitHub o GitLab lo usan intesamente a la hora de construir.

- **pre-receive**:

  - Para comprobar que los commits que se quieren guardar están bien formados.
  - Verificar que el usuario que intenta grabar los commits tiene permisos necesarios para hacerlo.

- **update**:

  - Puedes evitar de una forma granular cada actualización.

- **post-receive**:
  - Enviar un correo a todos los usuarios del repositorio que se han grabado nuevos cambios en el repositorio remoto.
  - Reflejar en una UI las nuevas referencias, ramas o commits disponibles.

### Crear Hook

Para crear un hook, simplemente debemos crear un archivo en la carpeta `.git/hooks` con el nombre del hook que queremos crear.

## 🎭 Alias

Los alias permiten definir una serie de comandos que pueden ser usados en lugar de los nombres completos.

```bash
git co -> git commit
git st -> git status
```

#### ¿Por qué origin es un alias?

Porque origin es el nombre por defecto que se le da al repositorio remoto.

#### Crear Alias

```bash
git config --global alias.co commit
```

```bash
git config --global alias.wo "log --oneline"
```

#### Borrar Alias

```bash
git config --global --unset alias.co
```

## 🎩 Trucos en Git

### Guarda cambios temporalmente

```bash
git stash
git stash -u
git stash pop
```

### Aplicar cambios de commits en específico

```bash
git cherry-pick <commit>
```

### Detectar que commit es el que ha introducido un gub

```bash
git bisect
git bisect start
git bisect bad
git bisect good <commit>
git bisect reset
```

### Cambiar el nombre de un commit

```bash
git commit --amend -m <descripcion>
```

### Recuperar un archivo en concreto de otra rama o commit

```bash
git checkout <SHA> <archivo>
```
