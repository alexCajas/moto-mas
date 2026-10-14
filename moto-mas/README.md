# Moto-Mas · Maquetas de rediseño web

Tres propuestas de diseño para modernizar la web de **Moto-Mas** (Pilar de la Horadada),
tienda y taller de **bicicletas y patinetes eléctricos** desde 1980.

Contenido extraído de la web actual ([moto-mas.com](https://www.moto-mas.com/es/)) y del
servicio de alquiler ([rentbikepilar.com](http://rentbikepilar.com/)),
**eliminando todas las referencias a motos** (KYMCO, Super Dink, etc.).

## Cómo verlo

Opción 1 — abrir directamente:

```
Abre index.html en el navegador (doble clic). El selector muestra las 3 maquetas.
```

Opción 2 — servidor local (recomendado):

```bash
cd moto-mas
python3 -m http.server 8765
# Abre http://localhost:8765
```

No requiere internet ni instalación: Tailwind y las fuentes van incluidos en `assets/`.

## Las 3 maquetas

| Maqueta | Estilo | Concepto |
|---|---|---|
| `maqueta-1/` | **Electric Tech** | Dark mode, acento verde neón, glassmorphism, estética de movilidad eléctrica |
| `maqueta-2/` | **Mediterránea** | Fondo claro, azul mar + coral, cercana y familiar |
| `maqueta-3/` | **Editorial Bold** | Crema/negro/amarillo, tipografía display gigante estilo revista (incluye FAQ) |

Cada maqueta incluye 3 páginas: `index.html` (Home + Alquiler), `servicios.html` y `contacto.html`.
Todas son responsive (probadas a 1440px y 390px de ancho).

## Estructura

```
moto-mas/
├── index.html              # Selector comparador de las 3 maquetas
├── README.md
├── assets/
│   ├── css → (cada maqueta tiene el suyo en maqueta-N/css/estilos.css)
│   ├── fonts/              # Fuentes locales (woff2) + fonts.css
│   ├── img/                # Fotos de la tienda + recortes de bicis + previews
│   └── vendor/tailwind.js  # Tailwind Play CDN descargado (funciona offline)
├── maqueta-1/  (index.html, servicios.html, contacto.html, css/estilos.css)
├── maqueta-2/  (…)
└── maqueta-3/  (…)
```

## Contenido real reutilizado

- Dirección: Calle Ramón y Cajal 25, 03190 Pilar de la Horadada (Alicante)
- Teléfono: +34 96 535 27 63 · Email: info@moto-mas.com
- Historia: desde 1980, más de 45 años, 3 generaciones de clientes, servicio multimarca
- Servicios: reparación de bicicletas, mantenimiento, kits eléctricos, venta/accesorios, alquiler
- Alquiler (precios reales de rentbikepilar.com): Girl 7€/día, Boy 7€/día, Woman 8€/día, Man 8€/día
- Redes: Facebook (motomas.pilardelahoradada), Instagram y Twitter (rentbikepilar)

## Notas

- **Precios de venta de bicis**: se muestran como "Consultar" para no inventar datos.
- **Horario**: orientativo (L–V 9:30–13:30 / 17:00–20:30, Sáb 10:00–13:30); confirmar con el negocio.
- **Testimonios**: ficticios, solo para la maqueta.
- **Formularios**: visuales (no envían datos); al integrar, conectar a email/CRM.
- **Imágenes**: fotos propias del negocio (recortadas para eliminar marcas de motos) + recortes
  de producto de las bicis de alquiler.
- Los mapas usan el embed público de Google Maps (necesita internet para verse).
