# Curso Git

## 👩🏻‍💻 Datos de la Estudiante

_**Nombre completo:** Esther Romero Aguilar_

---

## 🔙 Deshacer Cambios

### ¿En qué casos deshacemos cambios?

- Dejó de funcionar el proyecto.
- Queremos recuperar una parte del código que eliminamos.
- Queremos recuperar archivos que eliminamos.

### Comandos destrucctivos y no destructivos

#### 🔴 Destructivos

Afectan el historial de commits realizado.

#### git reset

Posee 2 opciones:

1. soft: Mantiene los cambios que ocurrieron antes de hacer commit desde donde apuntaba.

```bash
git reset --soft <id-commit> || git reset --soft HEAD~1
```

2. hard: Descarta los cambios.

```bash
git reset --hard <id-commit>
```

#### 🟢 No destructivos

Trabajan en base al historial sin afectarlo.

#### git revert

Revierte los cambios que un commit introdujo, y crea un nuevo commit con los cambios revertidos.

```bash
git revert HEAD~5
```

para abortar cambios:

```bash
git revert --abort
```

#### git checkout

Nos permite recuperar código específico de commits.

```bash
git checkout <id-commit> <archivo>
```
