# Curso Git

## 👩🏻‍💻 Datos de la Estudiante

_**Nombre completo:** Esther Romero Aguilar_

---

## 🌿 Ramas

Una rama es una línea de desarrollo independiente que permite trabajar en una nueva funcionalidad sin afectar la rama principal.

Para crear una rama, se puede utilizar el siguiente comando:

```bash
git branch <nombre-rama>
```

Para eliminar una rama, se puede utilizar el siguiente comando:

```bash
git branch -D <nombre-rama>
```

Para eliminar ramas de mi repositorio remoto, se puede utilizar el siguiente comando:

```bash
git remote prune origin
```

Para ver las ramas, se puede utilizar el siguiente comando:

```bash
git branch
```

Para ver todas las ramas, se puede utilizar el siguiente comando:

```bash
git branch -a
```

Para cambiar de rama, se puede utilizar el siguiente comando:

```bash
git checkout <nombre-rama> || git switch <nombre-rama>
```

Para crear una rama y cambiar a ella, se puede utilizar el siguiente comando:

```bash
git checkout -b <nombre-rama> || git switch -c <nombre-rama>
```

### ¿Por qué al generar una nueva rama, el id del commit no cambia?

El id del commit no cambia porque el commit es un objeto inmutable. Al crear una nueva rama, se crea un nuevo puntero que apunta al mismo commit que la rama anterior.

## 🔄 Merge

Para fusionar una rama con la rama actual, se puede utilizar el siguiente comando:

```bash
git merge <nombre-rama>
```

### Merge Fast-Forward

El merge fast-forward es un tipo de merge que se realiza cuando no hay conflictos entre las ramas. Consiste en avanzar la rama actual hasta la rama que se quiere fusionar.

Para realizar un merge fast-forward, se puede utilizar el siguiente comando:

```bash
git merge <nombre-rama>  --no-ff
```
