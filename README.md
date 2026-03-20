# 🎯 LifeAdmin

**Tu asistente personal inteligente** — Un prototipo funcional de aplicación móvil que combina capacidades de asistente digital y humano para ayudar a los usuarios a gestionar tareas diarias, citas, pagos y encargos.

---

## 📱 Vista General

LifeAdmin es una aplicación móvil (prototipo en HTML/CSS/JS) diseñada como interfaz de smartphone. Permite gestionar la vida cotidiana desde una sola app, con un asistente IA integrado para automatizar acciones comunes.

---

## ✨ Funcionalidades Actuales

### 🔐 Login
- Pantalla de inicio de sesión con email y contraseña
- Credenciales de prueba pre-rellenadas: `maria@example.com` / `password123`
- Validación básica de campos

### 🏠 Dashboard (Inicio)
- Saludo personalizado con fecha actual
- Tarjetas de estadísticas: tareas pendientes y citas
- Vista previa de las próximas tareas
- Navegación rápida a otras secciones

### ✅ Tareas
- Lista de tareas pendientes y completadas (con tabs)
- Marcar/desmarcar tareas como completadas
- Prioridades: Alta, Media, Baja
- Actualización en tiempo real del contador en el dashboard

### 💬 Chat IA
- Interfaz de conversación con asistente IA
- Acciones rápidas: Crear tarea, Agendar cita, Pagar factura, Hacer compra
- Historial de mensajes en sesión

---

## 🛠️ Tecnologías

| Tecnología | Uso |
|---|---|
| HTML5 | Estructura de la app |
| CSS3 | Estilos, animaciones, layout responsivo |
| JavaScript (Vanilla) | Lógica de estado, navegación, renderizado |

> Sin dependencias externas. Un solo archivo `.html` autocontenido.

---

## 🎨 Sistema de Diseño

| Variable | Color | Uso |
|---|---|---|
| `--primary` | `#6366f1` (Indigo) | Acciones principales, navegación activa |
| `--secondary` | `#10b981` (Emerald) | Tareas completadas, confirmaciones |
| `--accent` | `#f59e0b` (Amber) | Prioridad media, alertas |
| `--danger` | `#ef4444` (Rojo) | Prioridad alta, errores |

**Iconos:** SVG con `stroke="currentColor"`, `stroke-width="1.5"`, `fill="none"`, `stroke-linecap="round"`

---

## 📐 Layout

- **Móvil:** `100vw × 100vh`, sin bordes redondeados ni sombras
- **Desktop (>450px):** Contenedor de `414px × 896px` centrado, con esquinas redondeadas y sombra
- **Ratio de aspecto:** `9 / 19.5` (simulación de pantalla de 6.9")

---

## 🚀 Cómo Usar

1. Descarga el archivo `lifeadmin_v4_FUNCIONANDO.html`
2. Ábrelo directamente en cualquier navegador moderno
3. Inicia sesión con las credenciales de prueba:
   - **Email:** `maria@example.com`
   - **Contraseña:** `password123`
4. Explora las secciones desde la barra de navegación inferior

> ⚠️ **Nota:** Si el login no responde en producción/CDN, puede deberse a que Cloudflare inyecta `email-decode.min.js` fusionado al script de la app, bloqueando la ejecución de JavaScript. En ese caso, servir el archivo desde un servidor local o hosting estático sin proxies agresivos.

---

## 📁 Estructura del Proyecto

```
lifeadmin/
├── lifeadmin_v4_FUNCIONANDO.html   # App completa (único archivo)
└── README.md                        # Este archivo
```

---

## 🗺️ Roadmap

- [ ] Pantalla de Perfil con selector de plan de suscripción
- [ ] Gestión de tarjetas de pago (agregar, eliminar, establecer predeterminada)
- [ ] Recordatorios como tarjeta en el dashboard
- [ ] Integración real con API de IA
- [ ] Autenticación real (Firebase / Supabase)
- [ ] Notificaciones push
- [ ] Modo oscuro
- [ ] Soporte multiusuario

---

## 🤝 Contribuciones

Este proyecto está en fase de prototipo activo. Si quieres contribuir:

1. Haz fork del repositorio
2. Crea una rama para tu feature: `git checkout -b feature/nueva-funcionalidad`
3. Haz commit de tus cambios: `git commit -m 'feat: descripción del cambio'`
4. Push a tu rama: `git push origin feature/nueva-funcionalidad`
5. Abre un Pull Request

---

## ⚙️ Principios de Desarrollo

- **Inserciones quirúrgicas:** nunca eliminar ni reestructurar código funcional al agregar features
- **Integridad del login:** verificar siempre el flujo de login tras cambios en JavaScript
- **Sin regresiones:** cada entrega debe tener cero errores en consola del navegador
- **Estado global:** toda la lógica de estado vive en `appState`

---

## 📄 Licencia

MIT License — libre para usar, modificar y distribuir.

---

*Desarrollado como prototipo funcional de concepto de producto.*
