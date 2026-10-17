# Arbol_qr

Aplicación web estática que genera un código QR voxel en Three.js y alterna entre:

- **Vista QR** top-down plana y escaneable.
- **Vista diorama 3D** isométrica con árbol procedural centrado.

Árbol voxel procedural (único por URL) con sombras, base de diorama y detalles; se puede girar arrastrando. Incluye transición animada con GSAP, cambio de estaciones (Spring/Summer/Autumn) y partículas en otoño.

## Ejecutar

No requiere build tools.

1. Abre `index.html` directamente en un navegador moderno, **o** sirve la carpeta como estático.
2. Si quieres servir localmente con Python:

```bash
python -m http.server 8000
```

Luego abre `http://localhost:8000`.

## Controles

- **Input URL** (parte inferior): escribe una URL y pulsa **Enter** o **Actualizar QR** para regenerar el código.
- **Botón flotante central**:
  - `Tap to see the tree` → pasa a diorama 3D.
  - `Tap to see QR code` → vuelve a vista QR plana.
- **Estaciones**:
  - `Spring`: verdes claros y rosados.
  - `Summer`: verdes vibrantes y amarillos.
  - `Autumn`: naranjas/rojizos/marrones y partículas de hojas/lluvia.
