# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Proyecto

Landing page de cotización para **Aroma Center** — empresa chilena líder en aromatización profesional de espacios comerciales (+18 años, +6.000 equipos instalados). El objetivo es que clientes potenciales entiendan el servicio rápidamente y soliciten una cotización.

El sitio principal es **aromacenter.cl** (WordPress). Esta landing es un sitio **independiente**, deployable en Vercel.

## Stack

- **HTML + CSS** estático — sin frameworks, sin build step
- **Tailwind CSS** via CDN
- **Deploy:** Vercel (sitio estático)

Para previsualizar localmente:
```bash
open landing/index.html
# o con servidor local:
npx serve landing/
```

## Estructura del proyecto

```
landing/
  index.html        # Página única (toda la landing)
  assets/
    logo-color.png  # Logo azul lavanda (uso en fondos claros)
    logo-blanco.png # Logo blanco (uso en fondos oscuros)
```

## Branding

| Elemento | Valor |
|---|---|
| Color principal | `#8B91D4` — Pantone 2123 C (azul lavanda) |
| Fondo cálido | `#F0EAE0` — Pantone 11-0610 TSX "Silence" (crema) |
| Texto | `#232323` — Pantone 419 C (casi negro) |
| Tipografía | Sin definir aún — usar system-ui o Google Fonts a tono con el logo |

## Canales de contacto (hardcodeados en la landing)

- **WhatsApp (WATI):** `https://api.whatsapp.com/send/?phone=56981715598&text=Hola%20AromaCenter.%20Necesito%20m%C3%A1s%20informaci%C3%B3n.%0A%0AID%3A%20D-80216&type=phone_number&app_absent=0`
- **Formulario web:** `https://aromacenter.cl/contacto/`
- **Teléfono:** +56 2 2953 8600
- **Email:** contacto@aromacenter.cl
- **Dirección:** Tabancura 1562, Vitacura

## Información comercial

**Tarifa mensual incluye (comodato):**
1. Equipo y fragancia sin costo de compra, con reposición mensual
2. Aromatización continua hasta 10 horas diarias
3. Servicio técnico permanente

**Planes por superficie (precio base mensual):**

| Superficie | Ejemplo | Precio |
|---|---|---|
| Hasta 5 m² | Baños, ascensores | UF 0,65 + IVA |
| 5–10 m² | Oficinas pequeñas | UF 0,80 + IVA |
| 10–25 m² | Recepciones, tiendas pequeñas | UF 0,95 + IVA |
| 25–50 m² | Salas de venta, tiendas medianas | UF 1,20 + IVA |
| 50–100 m² | Grandes espacios | UF 1,50 + IVA |

- Espacios +100 m²: se evalúa instalación de más de un equipo
- Descuentos por volumen y licitaciones disponibles

**Instalación (pago único por dirección):**
- Región Metropolitana: UF 1,0 + IVA (incluye 1 equipo)
- Regiones: UF 1,5 + IVA (incluye 1 equipo)
- Equipo adicional: UF 0,2 + IVA c/u

## Sectores que atienden

Retail, hoteles, oficinas, restaurantes, centros médicos, wellness, inmobiliarias/salas de venta, centros deportivos, cafeterías, centros de atención.

## Principio de diseño

La landing debe ser **muy explicativa** — los clientes frecuentemente no entienden qué es la aromatización profesional ni cómo funciona el modelo de servicio (comodato). Priorizar claridad sobre estética.
