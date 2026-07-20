# EDUCAP · Prototipo UX

Repositorio **exclusivo** para publicar los bocetos navegables de EDUCAP y compartirlos con el cliente para validación, **antes** de terminar el desarrollo de la plataforma real.

> No contiene código ni documentación del producto: solo las maquetas de interfaz exportadas desde la herramienta de diseño. El proyecto real vive en un repositorio aparte.

## Enlace para el cliente

Una vez desplegado, el sitio queda en:

```
https://yair0024.github.io/educap-prototipo/
```

Ese es el enlace que se le envía al cliente. Abre un índice con las tres vistas, enlazadas entre sí.

## Contenido

| Archivo | Vista |
| --- | --- |
| `index.html` | Índice / menú de los bocetos |
| `EDUCAP Landing.dc.html` | Landing (sitio público) |
| `EDUCAP Plataforma.dc.html` | Plataforma (panel administrativo) |
| `EDUCAP Guardia.dc.html` | App del guardia (móvil) |
| `support.js` | Runtime que necesitan los bocetos exportados |

## Cómo se despliega

Automático con **GitHub Pages + GitHub Actions** (`.github/workflows/deploy.yml`).
Cada `push` a `main` vuelve a publicar el sitio. También se puede lanzar a mano desde la pestaña **Actions → Desplegar prototipo → Run workflow**.

## Cómo actualizar los bocetos

1. Exporta de nuevo las maquetas desde la herramienta de diseño.
2. Reemplaza los `.dc.html` y `support.js` en la raíz (conserva los nombres exactos: los bocetos se enlazan entre sí por nombre).
3. `git commit` y `git push` a `main`. En ~1 minuto el enlace queda actualizado.

## Notas

- Es un prototipo **visual**, no funcional: algunos botones/enlaces son solo de navegación y no todos los datos son reales.
- El índice incluye `noindex` para que no lo listen los buscadores. Aun así, cualquiera con el enlace puede abrirlo.
