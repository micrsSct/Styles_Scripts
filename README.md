# Estilos y Scripts

Repositorio destinado al almacenamiento de **estilos CSS** y **scripts JS** que no pueden ser agregados directamente en Joomla debido a las limitaciones del soporte y filtros de texto de la plataforma.

## ¿Por qué este repositorio?

Joomla no deja agregar archivos css y js en multimedia ya que no los soporta, lo que impide personalizar el sitio desde el panel de administración sin permisos avanzados. Este repositorio sirve como **fuente externa** desde donde se invocan los estilos y scripts mediante:

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/tuusuario/tu-repo/archivo.css">
```

```html
<script src="https://cdn.jsdelivr.net/gh/tuusuario/tu-repo/archivo.js"></script>
```

## Estructura

```
/
├── css/
│   └── styles-sidebar.css       # Estilos del sidebar derecho
├── js/
│   └── scripts.js               # Scripts personalizados
└── README.md
```

## ¿Cómo usar un archivo desde Joomla?

1. Sube o edita el archivo `.css` o `.js` en este repositorio
2. Copia la URL de **jsDelivr** del archivo:
   ```
   https://cdn.jsdelivr.net/gh/micrsSCT/Estilos_y_Scripts/css/archivo.css
   https://cdn.jsdelivr.net/gh/micrsSCT/Estilos_y_Scripts/js/archivo.js
   ```
3. Pega el `<link>` o `<script>` en el editor HTML del artículo de Joomla

## Notas

- Usar **jsDelivr** como CDN garantiza que el `Content-Type` sea correcto para CSS y JS
- Los cambios en GitHub pueden tardar unos minutos en reflejarse en jsDelivr
- Para forzar la actualización del caché de jsDelivr: `https://purge.jsdelivr.net/gh/tuusuario/tu-repo/archivo.css`
