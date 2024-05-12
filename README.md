# Curso Git

## 👩🏻‍💻 Datos de la Estudiante

_**Nombre completo:** Esther Romero Aguilar_

---

## 🚀 Git Push

Sube los cambios del repositorio local al repositorio remoto.

```bash
git push origin <nombre-rama>
```

### git push -u & git push -f

- **git push -u**: Establece la rama actual como rama por defecto.
- **git push -f**: Fuerza la subida de los cambios al repositorio remoto.

```bash
git push -u origin <nombre-rama>
```

```bash
git push -f origin <nombre-rama>
```

### eliminar rama remota

```bash
git push -d origin <nombre-rama>
```

### otros comandos relacionados

```bash
git push --all
git push --tags
```

## 📥 Git Pull

Descarga los cambios del repositorio remoto al repositorio local.

```bash
git pull origin <nombre-rama>
```

### git pull --rebase

El rebase es una técnica que permite reescribir la historia de un repositorio.

```bash
git pull --rebase origin <nombre-rama>
```

### git pull --all

Descarga todas las ramas del repositorio remoto al repositorio local.

```bash
git pull --all
```

### git pull --set-upstream

Establece la rama actual como rama por defecto.

```bash
git pull --set-upstream origin <nombre-rama>
```
