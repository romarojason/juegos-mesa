# 🎮 Club de Juegos de Mesa - PWA

Una aplicación web progresiva completa para gestionar sesiones de juegos de mesa con ruletas de selección, registro de partidas, historial y herramientas útiles.

## 🚀 Características

- **🎯 Ruletas de Selección**: Elige juegos y jugadores aleatoriamente
- **📋 Registro de Partidas**: Documenta cada sesión de juego
- **📊 Historial**: Visualiza estadísticas de todas las partidas
- **🛠️ Herramientas**: Dado, moneda y temporizador
- **📱 PWA**: Instala como app nativa en cualquier dispositivo
- **🌐 Offline**: Funciona sin conexión a internet

## 📦 Estructura del Proyecto

```
board-game-toolkit/
├── index.html          # Aplicación principal
├── manifest.json       # Configuración PWA
├── sw.js              # Service Worker
├── netlify.toml       # Configuración Netlify
├── favicon.ico        # Icono del sitio
├── icons/             # Iconos PWA
│   ├── icon-72x72.png
│   ├── icon-96x96.png
│   ├── icon-128x128.png
│   ├── icon-144x144.png
│   ├── icon-152x152.png
│   ├── icon-192x192.png
│   ├── icon-384x384.png
│   └── icon-512x512.png
└── screenshots/       # Capturas para PWA
    ├── desktop-1.png
    └── mobile-1.png
```

## 🛠️ Configuración para GitHub + Netlify

### 1. Preparar el Repositorio

```bash
# Crear repositorio
git init
git add .
git commit -m "Initial commit: Board Game Toolkit PWA"

# Conectar con GitHub
git remote add origin https://github.com/TU-USUARIO/board-game-toolkit.git
git branch -M main
git push -u origin main
```

### 2. Generar Iconos PWA

Necesitas crear los iconos en diferentes tamaños. Puedes usar:

- **Canva**: Diseña un icono de 512x512px
- **PWA Asset Generator**: https://www.pwabuilder.com/imageGenerator
- **Favicon.io**: https://favicon.io/favicon-converter/

Iconos requeridos:

- `icons/icon-72x72.png`
- `icons/icon-96x96.png`
- `icons/icon-128x128.png`
- `icons/icon-144x144.png`
- `icons/icon-152x152.png`
- `icons/icon-192x192.png`
- `icons/icon-384x384.png`
- `icons/icon-512x512.png`
- `favicon.ico`

### 3. Configurar Netlify

1. **Conectar repositorio**:
- Ve a [Netlify](https://netlify.com)
- Click en “New site from Git”
- Conecta tu repositorio de GitHub
1. **Configuración automática**:
- Netlify detectará automáticamente `netlify.toml`
- Build command: `echo 'No build needed'`
- Publish directory: `.`
1. **Configurar dominio personalizado** (opcional):
- Ve a Site settings > Domain management
- Agrega tu dominio personalizado

### 4. Variables de Entorno (si las necesitas)

```bash
# En Netlify Dashboard > Site Settings > Environment Variables
REACT_APP_API_URL=tu-api-url
```

### 5. Despliegue Automático

Cada push a `main` desplegará automáticamente la app.

## 📱 Funcionalidades PWA

### Instalación

- Aparece automáticamente el botón “Instalar App”
- Funciona en Chrome, Safari, Firefox, Edge
- Se instala como app nativa

### Offline

- Funciona sin conexión
- Cachea recursos automáticamente
- Sincronización cuando vuelve la conexión

### Características Nativas

- Icono en home screen
- Splash screen personalizada
- Funciona a pantalla completa
- Notificaciones push (preparado)

## 🔧 Desarrollo Local

```bash
# Servir localmente
npx serve .

# O usar Python
python -m http.server 8000

# O usar Node.js
npm install -g http-server
http-server
```

## 🎯 Uso de la Aplicación

### Ruletas

1. Agrega juegos y jugadores
1. Gira las ruletas para selección aleatoria
1. Los resultados se transfieren automáticamente al registro

### Registro de Partidas

1. Completa fecha, sede y juego
1. Selecciona jugadores participantes
1. Marca el ganador
1. Guarda la partida

### Historial

- Visualiza todas las partidas registradas
- Estadísticas de juegos y ganadores
- Exportación de datos (próximamente)

### Herramientas

- **Dado**: Lanza dados de 6 caras
- **Moneda**: Cara o cruz
- **Temporizador**: Configurable con alertas

## 🌟 Próximas Funcionalidades

- [ ] Múltiples tipos de dados
- [ ] Estadísticas avanzadas
- [ ] Exportar datos a CSV
- [ ] Temas personalizables
- [ ] Notificaciones push
- [ ] Sincronización en la nube

## 🤝 Contribuir

1. Fork el proyecto
1. Crea una rama para tu feature
1. Commit tus cambios
1. Push a la rama
1. Abre un Pull Request

## 📄 Licencia

MIT License - ve el archivo LICENSE para más detalles.

## 🆘 Soporte

Si encuentras algún problema:

1. Revisa los issues existentes
1. Crea un nuevo issue con detalles
1. Incluye screenshots si es necesario

-----

**¡Disfruta jugando! 🎲🎮**
