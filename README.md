# InfraLegal Pereira

Aplicación web/móvil de asesoría legal en infracciones de tránsito para Pereira, Colombia.

## 📱 Descripción

InfraLegal Pereira conecta ciudadanos con abogados especializados en infracciones de tránsito. La plataforma permite:

- 🔍 Consultar comparendos por número
- 💬 Chatear con un abogado simulado
- 🤖 Chatbot automático con palabras clave
- 📜 Historial de conversaciones
- 📂 Seguimiento del estado de casos legales

## 🛠️ Tecnologías

| Tecnología     | Propósito                     |
|----------------|-------------------------------|
| Vue.js 3       | Framework principal (CDN)     |
| Tailwind CSS   | Estilos (CDN)                 |
| Firebase       | Auth + Firestore (opcional)   |
| fetch API      | Consumo de APIs externas      |
| Font Awesome   | Íconos                        |

## 📁 Estructura del Proyecto

```
InfraLegal-Pereira/
├── index.html           # Archivo principal (HTML + Vue templates)
├── app.js               # Lógica Vue.js (setup, estado, métodos)
├── styles.css           # Estilos personalizados
├── services/
│   ├── firebase.js      # Configuración Firebase (opcional)
│   ├── api.js           # Consumo de APIs con fetch
│   └── chatbot.js       # Lógica del chatbot con palabras clave
├── components/          # Carpeta para futuros componentes
└── assets/              # Recursos estáticos
```

## 🚀 Cómo Ejecutar

### Opción 1: Sin servidor (más simple)
1. Abre la carpeta `InfraLegal-Pereira/`
2. Haz doble clic en `index.html`
3. Se abre en tu navegador

### Opción 2: Servidor local con Python
```bash
cd InfraLegal-Pereira
python -m http.server 8000
```
Abre: `http://localhost:8000`

### Opción 3: VS Code Live Server
1. Abre el proyecto en VS Code
2. Instala la extensión "Live Server"
3. Click derecho en `index.html` → "Open with Live Server"

## ⚙️ Configuración Firebase (Opcional)

La app **funciona sin Firebase** usando datos simulados.

Para activar persistencia real:
1. Crea un proyecto en [console.firebase.google.com](https://console.firebase.google.com)
2. Activa **Authentication** (Email/Password) y **Firestore Database**
3. Edita `services/firebase.js` y reemplaza las credenciales

## 📖 Funcionalidades

### 1. 📋 Consultar Comparendos
- Ingresa cualquier número y obtén datos simulados de infracción
- Muestra valor, fecha, lugar y estado

### 2. 💬 Chat con Abogado
- Mensajes en tiempo real con respuestas automáticas del "abogado"
- Historial durante la sesión

### 3. 🤖 Chatbot Inteligente
Responde por palabras clave: `multas`, `plazos`, `apelar`, `SOAT`, `licencia`, `puntos`, `urgente`, `hola`, `gracias`, `adiós`

### 4. 📜 Historial
- Lista conversaciones previas simuladas

### 5. 📂 Seguimiento de Casos
- Ingresa un ID de caso (ej: `CAS001`) y ver su timeline
- Lista de "Mis Casos" con estados

## 📄 Licencia

Proyecto con fines educativos — SENA / Tecnología en Análisis y Desarrollo de Software
