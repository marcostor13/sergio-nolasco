# Sergio Nolasco - Frontend

Frontend desarrollado con Astro 5.x, Tailwind CSS y SSR para la plataforma "Formando Empresarios con Propósito".

## 🚀 Características

- ✅ Server-Side Rendering (SSR) con Astro
- ✅ Diseño Mobile First con Tailwind CSS
- ✅ Línea gráfica personalizada (Verde Lima #70BE46 sobre fondo oscuro #0E0B16)
- ✅ Autenticación persistente con cookies HttpOnly
- ✅ Componentes UI reutilizables
- ✅ Formularios de registro, login y recuperación de contraseña

## 📋 Requisitos Previos

- Node.js 20.x o superior
- npm o yarn

## 🔧 Instalación

1. Instala las dependencias:

```bash
npm install
```

2. Copia el archivo `.env.example` a `.env` y configura las variables:

```bash
cp .env.example .env
```

3. Configura la URL de la API en `.env`:

```env
PUBLIC_API_URL=http://localhost:3000
```

## 🏃 Ejecutar la aplicación

### Desarrollo

```bash
npm run dev
```

La aplicación estará disponible en `http://localhost:4321`

### Producción

```bash
npm run build
npm run preview
```

## 📄 Páginas Disponibles

- `/` - Redirección automática (login o dashboard según autenticación)
- `/login` - Página de inicio de sesión
- `/register` - Página de registro
- `/forgot-password` - Recuperación de contraseña
- `/reset-password` - Restablecer contraseña (requiere token)
- `/verify-email` - Verificación de email (requiere token)
- `/dashboard` - Panel principal (requiere autenticación)
- `/logout` - Cerrar sesión

## 🎨 Línea Gráfica

### Colores

- **Primario (Acento):** `#70BE46` (Verde Lima Vibrante)
- **Fondo:** `#0E0B16` (Negro Oscuro con tinte azulado)
- **Fondo Secundario:** `#0A080F` (Negro Más Oscuro)

### Tipografía

- Fuente principal: Sans-serif moderna y limpia
- Estilo: Minimalista y profesional

## 🏗️ Estructura del Proyecto

```
src/
├── components/        # Componentes Astro
│   └── ui/           # Componentes UI reutilizables
├── layouts/          # Layouts de página
├── pages/            # Páginas/rutas
└── styles/           # Estilos globales
```

## 🔐 Autenticación

La autenticación se maneja mediante cookies HttpOnly enviadas por el backend. Las cookies se incluyen automáticamente en las solicitudes gracias a `credentials: 'include'` en las peticiones fetch.

## 📝 Licencia

UNLICENSED
