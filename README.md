# Curso Git

## 👩🏻‍💻 Datos de la Estudiante

_**Nombre completo:** Esther Romero Aguilar_

---

## 🔤 Hooks, Alias y Trucos de Git

### ¿Qué es un Hook?

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
