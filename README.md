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
