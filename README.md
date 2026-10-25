# La Espiga · Panadería de barrio

> **Proyecto de demostración.** La Espiga es un negocio ficticio. Hice este sitio
> como ejemplo de mi trabajo de diseño y desarrollo web. Conocé más en
> [michasevich.com](https://michasevich.com).

Sitio completo pensado para vecinos, familias y gente mayor de un barrio de Montevideo. Funciona como una página real: se puede
navegar, armar pedidos y guardar datos, pero no cobra nada ni envía
información a ningún servidor.

**Versión publicada:** [laespiga.michasevich.com](https://laespiga.michasevich.com)

## Tecnologías

- [Next.js 16](https://nextjs.org) con App Router
- React 19 y TypeScript
- Tailwind CSS 4 y componentes de Radix
- Efectos 3D hechos con CSS, sin librerías pesadas
- `localStorage` para guardar el carrito, los datos y los pedidos en el navegador del visitante
- Publicado en [Netlify](https://www.netlify.com)

## Estilo

Papel crema, kraft, pizarra con tiza y sello rojo. Fuentes Young Serif, Kalam y Atkinson Hyperlegible Next, pensada para baja visión. Texto grande, contraste alto y un botón de "Letra grande".

## Funcionalidades principales

- **Abierto ahora:** el estado del local con la hora real de Montevideo.
- **Carta tipo pizarra** por pestañas, con fotos, filtros por alérgeno y ficha de cada producto.
- **Vitrina 3D**, horno de ladrillo que se abre y sello que se da vuelta.
- **Torta configurable en 3D** para encargos, con precio y porciones en vivo.
- **Promos del día**, desayunos para regalar, pan de la semana y tarjeta de sellos.
- **Pedido por WhatsApp:** bolsa con retiro o envío y hora, Mis datos y Mis pedidos.
- **Accesible:** letra grande, alto contraste y navegación con teclado.

## Cómo correrlo en local

Necesitás [Node.js](https://nodejs.org) 20.9 o más nuevo. Recomiendo la versión 22.

```bash
git clone https://github.com/maximichasevich/demo-la-espiga.git
cd demo-la-espiga
npm install
npm run dev        # http://localhost:3000
```

No hace falta configurar nada. Otros comandos:

```bash
npm run build && npm start   # versión optimizada
npm run lint                 # revisión de código
npm run typecheck            # revisión de tipos
```

## Configuración

`config/sitio.ts` tiene el nombre del negocio, la dirección de esta demo, la
del portfolio y el WhatsApp del botón "¿Querés una página así?". Las
direcciones también se pueden definir con las variables de `.env.example`.

## Estructura

```
app/layout.tsx          Base del sitio: fuentes, estilos globales y botón de WhatsApp
app/(sitio)/            Diseño, estilos y páginas de la demo
components/demos/       Secciones, componentes, aviso "Demo" y créditos de fotos
config/                 Nombre y direcciones
public/demos/           Fotos
```

## Créditos

Las fotos son de [Wikimedia Commons](https://commons.wikimedia.org) con
licencias libres. Cada foto muestra su autor y licencia dentro del sitio.

## Autor

Diseñado y desarrollado por Maximiliano Michasevich.
[michasevich.com](https://michasevich.com) · contacto@michasevich.com

---

## English

**La Espiga is a demo project for a fictional business.** A neighborhood bakery website designed for families and older adults, with large type and high contrast. It was built by
Maximiliano Michasevich, a web designer and developer based in Montevideo,
Uruguay, as a portfolio sample. See more at [michasevich.com](https://michasevich.com).

- **Live demo:** [laespiga.michasevich.com](https://laespiga.michasevich.com)
- **Stack:** Next.js 16, React 19, TypeScript, Tailwind CSS 4, Netlify.
- **Highlights:** chalkboard menu with photos and allergen filters, 3D display case and cake builder, live "open now" status, and ordering through WhatsApp.
- **Run locally:** `npm install`, then `npm run dev`.
