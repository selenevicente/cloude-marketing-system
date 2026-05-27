# Panel Digital Riel Americano · Mockup en planta industrial
> Cómo generar la foto del panel **instalado en una fábrica real** con Gemini / Imagen / Midjourney.

---

## PASO 1 · Capturar el panel como PNG

1. Abrí `panel-planta-v2-grande.html` en Chrome o Edge.
2. Hacé la ventana lo más ancha posible (full screen).
3. Apretá **F12** → tab "Device toolbar" (Ctrl+Shift+M).
4. Arriba a la derecha del DevTools → **⋮ → Capture screenshot** (o `Capture full size screenshot`).
5. Guardás como `panel-riel.png`.

> Alternativa rápida: Cmd+Shift+4 (Mac) o Win+Shift+S (Windows) y hacés crop manual del panel sin la bezel.

---

## PASO 2 · Prompt para Gemini / Google AI Studio

### Prompt principal (con foto de referencia adjunta)

> Subís el `panel-riel.png` como imagen de referencia + este prompt:

```
Photorealistic editorial photograph of a large 55-inch landscape Smart TV 
mounted on the wall of a contemporary Argentinian textile manufacturing 
factory. The TV displays exactly the dashboard interface from the 
reference image — preserve all content, layout, typography and colors 
of the reference panel without alterations.

Environment: industrial curtain manufacturing plant in San Martín, 
Buenos Aires. Exposed concrete walls in a soft warm gray tone, exposed 
steel beams and ducts overhead, polished concrete floor with subtle 
reflections. To the right of the frame, large industrial windows let 
in soft natural afternoon daylight. To the left, partially visible, 
modern industrial sewing machines and rolls of white curtain fabric, 
slightly out of focus.

Foreground (lower third, soft bokeh): a clean industrial cafeteria 
setup with simple wooden tables and stools. Two factory workers in 
gray Riel Americano work shirts visible from the back, sitting at a 
table having coffee, completely out of focus and unidentifiable.

Lighting: balanced — cool fluorescent overhead lighting + warm daylight 
spilling from the right windows. The TV screen emits its own light, 
slightly illuminating the wall around it. No glare or reflections on 
the screen itself.

Camera: full-frame, 35mm lens, eye-level shot from approximately 5 
meters away, aperture f/4, ISO 200, sharp focus on the TV screen. 
The TV occupies roughly 40% of the frame, positioned slightly off-center 
following rule of thirds.

Style: editorial corporate photography, similar to an Apple annual 
report or Bosch industrial brochure. Photorealistic, no artistic 
filters, no HDR overprocessing. Slight film grain. Color grade: 
desaturated industrial palette with the TV being the brightest, most 
saturated element in the composition.

Quality: 4K, photorealistic, hyperdetailed.
```

### Prompt para Midjourney (estilo MJ)

```
photorealistic editorial photograph, contemporary Argentinian textile 
factory interior, large 55-inch landscape Smart TV mounted on exposed 
concrete wall displaying industrial dashboard with red accents and 
white numbers, soft warm afternoon daylight from right side windows, 
out-of-focus industrial sewing machines and white curtain fabric rolls 
in background, foreground bokeh of simple cafeteria tables, two 
unrecognizable workers in gray shirts in soft focus, 35mm lens, f/4, 
eye-level shot, Apple annual report aesthetic, desaturated industrial 
palette, photorealistic, no HDR, slight film grain --ar 16:9 --v 6 --style raw
```

### Prompt para Kling.ai (image-to-video, si quisieras animarlo)

```
Static editorial wide shot of a 55-inch Smart TV mounted on the wall 
of an industrial textile factory in Argentina, displaying a dashboard 
interface. Subtle movement: a worker walks slowly across the background 
right to left, out of focus. The dashboard content stays static and 
sharp. Soft afternoon light shifts slightly. 5 seconds, 4K, vertical 
or horizontal 16:9. Photorealistic editorial style.
```

---

## PASO 3 · Variaciones de ambiente

Si querés probar distintos lugares dentro de la planta:

### Variación A · Comedor de planta
> Cambiá la primera parte del prompt por:
> "The TV is mounted high on the wall of an industrial cafeteria with 
> long wooden tables and bench seating, served lunch trays in the 
> foreground, soft natural light from skylights overhead."

### Variación B · Entrada al sector productivo
> "The TV is mounted next to the safety-equipment lockers at the 
> entrance of the production floor. Workers visible passing through 
> safety doors in the soft background. Yellow safety floor markings 
> visible. Cool industrial lighting."

### Variación C · Sala de control / supervisión
> "The TV is one of three displays in an industrial control room, 
> with engineering desks visible in the foreground holding laptops 
> and technical drawings. Cooler, more sterile lighting."

---

## PASO 4 · Editar en Canva

Una vez que tengas la foto del mockup en planta (de Gemini):

1. **Canva → Crear diseño → Tamaño personalizado** → 1920×1080 o 16:9.
2. **Subir imagen** → arrastrá la foto del mockup que generó Gemini.
3. La imagen se convierte en fondo editable.
4. Para reemplazar el logo del panel:
   - Tapás el círculo rojo del logo con un **rectángulo blanco** o con tu **logo PNG real**.
   - Lo ubicás encima del logo placeholder.
5. Para editar textos sobre el panel:
   - Insertás **cuadros de texto** en Canva.
   - Los posicionás encima del texto del panel que quieras tapar.
   - Usás fuente **Manrope** (está en Canva).
6. Exportás como PNG o JPG.

---

## ALTERNATIVA · Subí el panel directo a Canva (sin mockup)

Si querés editar **el panel sin mockup de planta**:

1. Sacás screenshot del HTML (Paso 1).
2. Canva → Subir el PNG.
3. Lo usás como base, agregás texto y logo encima.
4. Tamaño: 1920×1080 (16:9).

---

## RECOMENDACIONES FINALES

- Las **dimensiones reales** del panel son 1920×1080 — generá el mockup en 16:9.
- El panel está **diseñado para verse a 2-4 metros**, así que la tipografía es grande a propósito.
- Si lo querés instalar de verdad en una Smart TV: subís el HTML a la TV (Samsung Tizen / LG WebOS tienen browser, o conectás una Raspberry Pi por HDMI en modo kiosco).
- Para que el reloj funcione en tiempo real en la TV real: el v2 actual tiene el reloj fijo en 14:32 para que el mockup salga limpio. Si querés versión live, te paso un toggle.
