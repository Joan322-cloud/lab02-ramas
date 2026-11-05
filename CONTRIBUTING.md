# Guia de contribucion

Gracias por querer mejorar **lab02-ramas**. Este documento explica cómo reportar un error, cómo proponer una mejora y qué revisar antes de enviar un Pull Request.

## Como reportar un error

Abre un **Issue** en este repositorio y responde estas cuatro preguntas:

| Pregunta | Ejemplo |
| :--- | :--- |
| Qué esperabas | El título debería verse en azul institucional |
| Qué ocurre | El título se ve en negro |
| Dónde | estilos.css, regla `h1` |
| Cómo reproducirlo | Abrir index.html en el navegador |

Usa un título que diga el problema, por ejemplo: *El título no toma el color de estilos.css*.

## Como proponer una mejora

1. Haz un **fork** del repositorio y clona tu fork.
2. Vuelve a main y actualízala antes de empezar:

```bash
git switch main
git pull
```

3. Crea una rama con un nombre que diga qué cambias:

```bash
git checkout -b mejora/enlaces-menu
```

4. Haz tus cambios, pruébalos en el navegador y revisa con `git diff`.
5. Haz commit y sube la rama a tu fork con `git push origin mejora/enlaces-menu`.
6. Abre un **Pull Request** hacia la rama main de este repositorio.

## Reglas para ramas y commits

- Nombra las ramas con un prefijo: `mejora/` para algo nuevo y `fix/` para un error.
- Escribe mensajes de commit en presente y que expliquen el cambio: *Agrega enlaces reales al menu*.
- Un Pull Request resuelve **una sola cosa**.
- Si tu cambio cierra un Issue, escribe `Closes #numero` en la descripción del Pull Request.

## Checklist antes de enviar tu Pull Request

- [ ] Creé mi rama desde main actualizada
- [ ] Probé los cambios en el navegador con Ctrl + F5
- [ ] Revisé con `git diff` que no quedaran líneas de prueba
- [ ] No quedan marcas de conflicto (`<<<<<<<`, `=======`, `>>>>>>>`)
- [ ] El mensaje del commit explica qué cambié
- [ ] La pestaña Files changed muestra solo los archivos que modifiqué

## Dudas

Si tienes una pregunta, abre un Issue con la etiqueta **question** o vuelve al [README](README.md).