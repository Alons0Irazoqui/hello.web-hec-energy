# HECNERGY — Landing Page | Informe para el Desarrollador

Este documento es el **brief oficial del proyecto**. Contiene toda la información de negocio, branding, requerimientos de diseño y flujo de trabajo necesarios para construir la landing page de **HECNERGY**, empresa dedicada exclusivamente a la **venta de proyectos de paneles solares**.

El desarrollo se hará sobre una **plantilla base HTML** ya existente, la cual se irá iterando y adaptando a las necesidades de este negocio. **El desarrollador trabajará junto con Claude (Claude Code)**, dándole instrucciones directas para modificar la plantilla hasta alcanzar el resultado final. Este README debe usarse como contexto inicial para Claude y como referencia constante durante todo el proyecto.

---

## 1. Sobre el negocio

| Campo | Dato |
|---|---|
| **Nombre del negocio** | HECNERGY |
| **Eslogan / actividad** | Proyectos de Energía Solar |
| **Rubro** | Venta e instalación de proyectos de paneles solares (energía solar fotovoltaica) |
| **Teléfono / WhatsApp** | 871 476 667 |

### ⚠️ Importante: fuente de información del negocio

El cliente **no proporcionó un dossier de marca, textos, ni fotografías propias del negocio**. La única información entregada es:

1. El logo (carpeta `imagenes/`, archivo `LOGO.png`).
2. El número de teléfono/WhatsApp: **871 476 667**.
3. Sus redes sociales, detalladas abajo.

Por lo tanto, **toda la información adicional necesaria para construir la landing page (fotos de instalaciones/proyectos realizados, testimonios, descripción de servicios, ubicación, horarios, publicaciones, tono de comunicación, etc.) debe obtenerse directamente de las redes sociales del negocio.** Es responsabilidad del desarrollador (o de las instrucciones que le dé a Claude) revisar estas redes y extraer contenido real y coherente con la marca — no se debe inventar información de negocio ni usar contenido genérico de relleno tipo "lorem ipsum" si se puede reemplazar por algo real extraído de estas fuentes.

**Redes sociales oficiales de HECNERGY:**

- Facebook: https://www.facebook.com/share/19223hihhp/
- TikTok: https://www.tiktok.com/@hecnergy?_r=1&_t=ZS-985bFGPy7CS
- Instagram: https://www.instagram.com/hecn.ergy?igsh=MXd1dWxrd3N1Z3R0OQ==

De estas redes se debe intentar obtener, como mínimo:
- Fotografías reales de proyectos/instalaciones de paneles solares.
- Descripción de servicios ofrecidos (venta, instalación, mantenimiento, tipos de proyectos, etc.).
- Zona/ciudad de operación si está disponible.
- Cualquier testimonio, publicación destacada o dato de contacto adicional (email, dirección) que ayude a completar la landing page.

---

## 2. Recursos entregados

Carpeta `imagenes/` — actualmente contiene **únicamente el logo**:

```
imagenes/
└── LOGO.png
```

### ⚠️ El logo necesita edición antes de usarse

El archivo `LOGO.png` **no tiene el fondo transparente** (viene con fondo sólido). Antes de integrarlo en la landing page, el desarrollador debe **quitarle el fondo** (dejarlo en PNG transparente) para que se pueda usar correctamente sobre distintos fondos de la web (header, footer, loading screen, favicon, etc.). Se recomienda generar además una versión del logo optimizada/comprimida para web.

---

## 3. Identidad de marca — Paleta de colores

La paleta de colores fue extraída directamente del logo oficial y **debe ser la base del diseño de toda la landing page**. Colores de referencia (aproximados, ajustar con pipeta de color directamente sobre el `LOGO.png` para obtener el HEX exacto):

| Color | Uso en el logo | HEX aproximado |
|---|---|---|
| 🔵 Azul corporativo | Palabra "HEC", panel solar, texto del eslogan | `#1B5C94` |
| 🟢 Verde | Palabra "NERGY", anillo circular del isotipo | `#3FA746` |
| 🟡 Amarillo / dorado | Rayos del sol | `#FDC221` |
| 🔷 Azul oscuro | Sombra/detalle de los paneles solares | `#123A5E` |
| ⚫ Negro / gris oscuro | Para textos secundarios, fondos oscuros tipo "dark mode" corporativo | `#0D0D0D` – `#1A1A1A` |
| ⚪ Blanco / gris claro | Fondos limpios, espacios en blanco, contraste | `#FFFFFF` – `#F5F7FA` |

**Concepto visual:** azul y verde como colores primarios (tecnología + sostenibilidad/energía limpia), amarillo como color de acento para CTAs, íconos o detalles que evoquen el sol/energía. El negro/gris oscuro se usa para lograr el look premium/high-tech en secciones de alto impacto (hero, fondos con contraste).

---

## 4. Estilo de diseño requerido

La landing page debe transmitir un posicionamiento **premium, corporativo y de alta tecnología**. Dirección de diseño:

- **Premium / Enterprise / Corporativo**: se debe sentir como la web de una empresa grande y confiable, no como una landing genérica de plantilla.
- **High-tech y elegante**: uso de gradientes sutiles, tipografías modernas, espaciados amplios, iconografía limpia.
- **Minimalista**: evitar saturar de elementos. Priorizar jerarquía visual clara, mucho espacio en blanco/negativo, contenido bien organizado.
- Coherencia total con la paleta de colores del logo (azul, verde, amarillo, negro/blanco).

Este estilo (premium + high-tech + minimalista + corporativo) es la dirección general que Claude debe mantener en **todas** las iteraciones del proyecto, sin desviarse hacia diseños genéricos o recargados.

---

## 5. Efectos visuales y animaciones (obligatorio)

La landing page debe incluir los siguientes efectos, ya que son parte central de la experiencia premium que se busca:

1. **Pantalla de carga (loading screen)**
   - Debe aparecer al cargar la página.
   - Debe mostrar un **spinner de carga** junto con el **logo del negocio** (el logo sin fondo).
   - Transición suave hacia el contenido de la página una vez cargada.

2. **Animaciones de scroll**
   - Los elementos/secciones deben animarse (fade in, slide up, etc.) a medida que el usuario hace scroll y van entrando en el viewport.

3. **Efectos en el título del Hero (sección principal)**
   - Efecto tipo **máquina de escribir (typewriter)** en el título principal.
   - Efecto de **cambio de color en las letras** del título (animación de color, tipo gradiente animado o transición de color por letra/palabra).
   - Estos efectos deben verse elegantes y sutiles, coherentes con el estilo premium/high-tech, sin resultar exagerados o "cargados".

---

## 6. Flujo de trabajo — Iteración con Claude

- El desarrollo se basa en una **plantilla HTML base**, sobre la cual ya se aplicó un prompt inicial para adaptarla al negocio.
- El desarrollador **debe seguir iterando con Claude** (dándole instrucciones, ajustes y correcciones) **hasta lograr el resultado final deseado**. No es un proceso de una sola pasada: se espera iteración continua sobre diseño, contenido, animaciones y responsividad hasta cerrar el proyecto.
- Este README debe entregarse a Claude como contexto de negocio al iniciar/continuar el proyecto, para que las decisiones de diseño y contenido estén siempre alineadas con la marca HECNERGY.

---

## 7. Checklist de entregables

- [ ] Logo (`LOGO.png`) sin fondo, optimizado para web.
- [ ] Contenido e imágenes reales del negocio extraídos de Facebook, Instagram y TikTok.
- [ ] Paleta de colores aplicada de forma consistente en toda la landing.
- [ ] Estilo premium / corporativo / high-tech / minimalista aplicado en todas las secciones.
- [ ] Pantalla de carga con spinner + logo.
- [ ] Animaciones de scroll en las distintas secciones.
- [ ] Efecto typewriter en el título del Hero.
- [ ] Efecto de cambio de color en las letras del título del Hero.
- [ ] Número de teléfono/WhatsApp (871 476 667) visible e integrado (botón de contacto directo/WhatsApp).
- [ ] Enlaces a redes sociales (Facebook, Instagram, TikTok) integrados en la web.
- [ ] Landing page responsiva (mobile, tablet, desktop).
