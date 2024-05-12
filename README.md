# Curso Git

## 👩🏻‍💻 Datos de la Estudiante

_**Nombre completo:** Esther Romero Aguilar_

---

## 🏆 Buenas Prácticas

### ¿Para qué sirven las buenas prácticas?

- Es un estandar manejado en la mayoría de equipos de desarrollo.
- Resolver conflictos o problemas drante el desarrollo es más sencillo.
- Tu historial de commits es más limpio y fácil de leer.

### ¿Cada cuánto tiempo debería hacer commits?

**A MENUDO**

Es mejor hacer commits pequeños, agrupando pequeñas mejoras o acciones, que un commit con todo lo que se quiere hacer.

Hacer commit a menudo no significa que debas hacer commits sin sentido.

### Escribir buenos mensajes de commit

- Usar el verbo imperativo.
  - [ADD], [FIX], [UPDATE], [REMOVE], [REFACTOR], [CHANGE]
- No usar puntos final ni puntos suspensivos en los mensajes (a lo más usa la coma)
- Usar como máximo 50 caracteres para el mensaje.
- Añadir todo el contexto que sea necesario en el cuerpo del commit (con reglas de puntuación)
- Considerar usar utilidades para hacer commit
- Usar un prefijo para los commits, cuyo fin sea hacerlos más eficientes.
  ```xml
  <tipo-de-commit> [scope] : <descripción>
  ```
  ejemplo:

```xml
  feat: add new search feature
```

### Prefijos para commits

- **feat**: Nueva funcionalidad.
- **fix**: Corrección de errores.
- **perf**: Mejora del rendimiento.
- **build**: Cambios que afectan el sistema de compilación.
- **ci**: Cambios en la integración continua.
- **docs**: Documentación.
- **refactor**: Refactorización del código.
- **style**: Cambios que no afectan el código.
- **test**: Añadir o modificar pruebas.

Ejemplo:

```xml
feat(backend): add filter for cars
fix(web): remove wrong color
```

### Escribir buenos nombres de ramas

- Ser consistente al nombrar las ramas.
- Usar el nombre de la accion que se realiza en la rama

  - bug/avoid-creating-lead-twice
