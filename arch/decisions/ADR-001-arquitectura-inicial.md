---
id: ADR-001
titulo: Arquitectura inicial de una-web-para-vender-ropa
estado: propuesto
fecha: 2026-08-03
owner: arquitectura
---

# ADR-001 · Arquitectura inicial de una-web-para-vender-ropa

## Contexto

Una web para vender ropa

Usuarios: Personas comunes sin conocimiento tecnico.
Entornos: todos.

### En alcance
- solo una web

### Fuera de alcance
- el app movil

## Decisión

Se adopta una arquitectura **monolito** con topología
**mono-repo**.

### Corte por servicios
- N/A (mono-repo)

## Consecuencias

- El stack declarado pasa a ser allowlist `STK-*`: una dependencia fuera de esa lista bloquea en G6.
- Las áreas quedan registradas en `project.yaml`; un `REQ` con área no registrada bloquea en G12.
- Cambiar esta decisión exige un ADR que la marque `superseded`, no editarla en sitio.

> Generado por la entrevista de New Project. Requiere aprobación de arquitectura
> antes de pasar a `aceptado`.
