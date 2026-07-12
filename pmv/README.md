# Suraci Consulting OS — PMV

Aplicación de una sola página (React + Tailwind vía CDN, sin paso de build) lista para desplegar como sitio estático.

## Contenido
- Landing institucional de Suraci Consulting
- Dashboard Ejecutivo con KPIs y actividad reciente
- CRM de Clientes (listado, filtros, ficha de detalle, línea de tiempo, notas)
- Diagnóstico Empresarial con cálculo automático del Índice de Franquiciabilidad (IFR)
- Portal del Cliente navegable (Resumen, Hoja de Ruta, Documentos, Mensajes)
- Centro de IA con chat de demostración
- Modo oscuro, diseño responsive y accesible (foco visible, aria-labels, roles)

## Deploy en Vercel
1. Subir esta carpeta a un repositorio (o arrastrar en vercel.com/new → "Deploy without Git").
2. Framework preset: **Other** (sitio estático).
3. No requiere build command ni variables de entorno.
4. `index.html` es el único archivo necesario.

## Notas técnicas
Por tratarse de un PMV para demo en una única sesión, la app usa React 18 y Babel Standalone vía CDN (transpilación en el navegador) en lugar de un pipeline Vite/Node. Esto permite cero configuración y despliegue inmediato. Para producción, se recomienda migrar a un proyecto Vite compilado (como el existente `dist/`) manteniendo los mismos componentes.
