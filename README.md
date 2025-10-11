# Home Care Instalaciones - Sitio Web Estático

Sitio web estático de Home Care Instalaciones, migrado desde WordPress para despliegue en Vercel.

## 📋 Descripción

Este es un sitio web completamente estático generado desde WordPress usando el tema Divi. El sitio ofrece servicios de instalaciones y aplicaciones para el hogar y oficina en el área metropolitana de Guadalajara.

## 🚀 Despliegue en Vercel

> Actualización 2024-10-10: se agregó este bloque para forzar un nuevo build desde GitHub y verificar la integración con Vercel.

### Opción 1: Despliegue desde CLI

1. Instala Vercel CLI (si no lo tienes):
```bash
npm install -g vercel
```

2. Despliega el sitio:
```bash
cd /path/to/web-homecare
vercel
```

3. Sigue las instrucciones en pantalla para vincular tu proyecto.

### Opción 2: Despliegue desde GitHub

1. Sube el proyecto a GitHub:
```bash
git init
git add .
git commit -m "Initial commit - sitio estático Home Care"
git branch -M main
git remote add origin https://github.com/tu-usuario/tu-repo.git
git push -u origin main
```

2. Conecta tu repositorio en [vercel.com](https://vercel.com):
   - Haz clic en "New Project"
   - Importa tu repositorio de GitHub
   - Vercel detectará automáticamente la configuración de `vercel.json`
   - Haz clic en "Deploy"

## 📁 Estructura del Proyecto

```
web-homecare/
├── index.html              # Página principal
├── vercel.json             # Configuración de Vercel
├── .gitignore              # Archivos ignorados por Git
├── README.md               # Este archivo
├── wp-content/             # Recursos de WordPress
│   ├── uploads/            # Imágenes y media
│   │   └── 2024/06/        # Imágenes del sitio
│   ├── themes/             # Tema Divi
│   │   └── Divi/
│   │       ├── js/         # JavaScript del tema
│   │       └── images/     # Imágenes del tema
│   ├── plugins/            # Plugins de WordPress
│   └── et-cache/           # Caché de estilos
├── wp-includes/            # Core de WordPress
│   └── js/                 # jQuery y librerías
└── author/                 # Páginas de autor
```

## 🔧 Cambios Realizados en la Migración

1. ✅ **Corrección de imagen faltante**: Reemplazada `green-energy-icon-18-2.png` por `green-energy-14.png`
2. ✅ **Configuración de Vercel**: Creado `vercel.json` con headers de cache optimizados
3. ✅ **Git ignore**: Creado `.gitignore` para excluir archivos innecesarios
4. ✅ **Rutas verificadas**: Todas las rutas de recursos son relativas y funcionan correctamente

## 📊 Estado de los Recursos

### ✅ Recursos Completos
- **Imágenes**: 37/38 (97.4%)
- **JavaScript**: 9/9 archivos (100%)
- **Logos y favicons**: Todos presentes
- **Iconos de servicios**: Todos presentes

### ⚠️ Recursos con Advertencias
- **CSS de caché de Divi**: 2 archivos faltantes (no críticos, hay CSS inline)
  - `/wp-content/et-cache/8/et-divi-dynamic-tb-59-tb-104-8.css`
  - `/wp-content/et-cache/8/et-core-unified-8.min.css`

  **Nota**: Estos archivos no afectan la funcionalidad porque todo el CSS necesario está embebido en el HTML.

## 🌐 Enlaces Externos

El sitio mantiene estos enlaces externos:
- **Catálogo de productos**: https://homecare.spread.name/
- **Google Fonts**: Poppins, Montserrat, Work Sans
- **Créditos**: https://soymercatonic.com/

## 🎨 Tecnologías Utilizadas

- HTML5
- CSS3 (inline, desde Divi)
- JavaScript (jQuery + Divi)
- Google Fonts
- WhatsApp integration
- Tema Divi de Elegant Themes

## 📱 Características del Sitio

- ✨ Diseño responsive (móvil, tablet, desktop)
- 🎨 Animaciones y efectos visuales
- 📞 Integración con WhatsApp
- 🔍 SEO optimizado con Yoast
- ⚡ Carga optimizada de imágenes (lazy loading)
- 🎯 Múltiples secciones de servicios

## 🔄 Actualizaciones Futuras Recomendadas

1. **Optimización de Performance**:
   - Localizar Google Fonts para mejor rendimiento
   - Extraer CSS inline a archivos externos
   - Minificar HTML (actualmente ~220KB)
   - Implementar WebP para imágenes

2. **Mejoras de SEO**:
   - Añadir meta descriptions personalizadas
   - Optimizar títulos de imágenes y alt tags
   - Implementar schema markup adicional

3. **Funcionalidades**:
   - Formulario de contacto funcional (requiere backend)
   - Analytics (Google Analytics o similar)
   - Chat en vivo

## 📞 Soporte

Para preguntas o soporte, contacta al equipo de desarrollo.

## 📄 Licencia

Este sitio web es propiedad de Home Care Instalaciones. Todos los derechos reservados.

---

**Generado el**: Octubre 2025
**Sitio original**: https://homecareinstalaciones.com/
**Tema**: Divi v4.27.4 by Elegant Themes
