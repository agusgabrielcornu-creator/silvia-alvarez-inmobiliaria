# Silvia Álvarez · Negocios Inmobiliarios — sitio web

Página web interactiva para la inmobiliaria Silvia Álvarez (Río Cuarto, Córdoba).
Propiedades, fotos y datos tomados de [@inmobiliaria.silviaalvarez](https://www.instagram.com/inmobiliaria.silviaalvarez/).

## Versiones

| Carpeta | Diseño |
|---|---|
| `index.html` | **Actual** — diseño propio basado en los globos de diálogo del logo (rojo, blanco y gris). Contacto en forma de charla. |
| `version-pelicula/index.html` | **Anterior** — estética de película: claqueta, visor de cámara, recorrido como línea de tiempo de edición, storyboard y créditos. |
| `version-clasica/index.html` | **Primera** — clásica y elegante en rojo y blanco, tipografía con serifa, recorrido horizontal y mapa. |

Las tres versiones usan las mismas fotos de la carpeta `img/`.

## Estructura

```
index.html                  versión actual
version-pelicula/index.html versión anterior (película)
version-clasica/index.html  primera versión (clásica)
img/                        fotos de las propiedades (p{id}-{n}.jpg; la 1 es la placa del post)
```

## Cómo verla

Abrí `index.html` en el navegador. Para que el mapa y las fotos carguen bien conviene servir la carpeta con un servidor local
(por ejemplo la extensión "Live Server" de VS Code).

## Cómo agregar o editar una propiedad

En cada `index.html`, buscá la lista `const P = [ ... ]` y agregá un objeto con:
`id`, `op` (venta / alquiler / terreno / comercial), `tipo`, `t` (título), `a` (dirección), `price`, `cur` (USD o $),
`d` (dormitorios), `b` (baños), `lat`, `lng`, `desc` y `f` (características).
Las fotos van en `img/p{id}-1.jpg`, `img/p{id}-2.jpg`, etc.

## Notas

- Las ubicaciones en el mapa son aproximadas.
- El contacto abre WhatsApp al 358 487-0218.
