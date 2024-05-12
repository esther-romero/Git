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
