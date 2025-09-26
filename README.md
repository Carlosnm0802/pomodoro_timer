# 🍅 Pomodoro Timer con Alarma Visual

Un timer Pomodoro moderno y funcional con sistema de alarmas visuales, sonoras y notificaciones del sistema.

![Pomodoro Timer](https://img.shields.io/badge/Status-Completed-brightgreen)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)

## ✨ Características

### 🎯 Funcionalidades Principales
- **Timer Pomodoro clásico** (25/5/15 minutos)
- **Múltiples presets** (Clásico, Corto, Largo, Personalizado)
- **Sesiones automáticas** con ciclos de trabajo y descanso
- **Estadísticas en tiempo real** (sesiones completadas, ciclos)

### 🔔 Sistema de Alarmas Avanzado
- **Modal de alarma visual** con animaciones llamativas
- **Notificaciones del sistema** nativas del navegador
- **Sonido de alarma** con secuencia de beeps
- **Efectos visuales**: parpadeo, vibración, rebote
- **Título de ventana parpadeante** para mayor visibilidad

### ⚙️ Configuración Flexible
- **Presets predefinidos**: Clásico, Corto, Largo
- **Configuración personalizada** de tiempos
- **Persistencia de configuración** en localStorage
- **Interfaz responsive** para móviles y escritorio

### 🎨 Diseño Moderno
- **Interfaz glassmorphism** con efectos de cristal
- **Gradientes dinámicos** según el tipo de sesión
- **Animaciones CSS** suaves y profesionales
- **Tema adaptativo** (rojo para trabajo, azul para descanso)

## 🚀 Cómo Usar

### Instalación
1. **Clona el repositorio**:
   ```bash
   git clone https://github.com/tu-usuario/pomodoro-timer.git
   cd pomodoro-timer
   ```

2. **Abre el archivo**:
   - Abre `index.html` en tu navegador
   - O usa un servidor local: `python -m http.server 8000`

### Configuración de Notificaciones
1. **Haz clic en "⚙️ Solicitar Permisos"**
2. **Permite las notificaciones** cuando el navegador lo solicite
3. **Prueba con "🔔 Probar Notificación"**
4. **Verifica el estado** en el indicador inferior

### Uso del Timer
1. **Selecciona un preset** o configura tiempos personalizados
2. **Haz clic en "Iniciar"** para comenzar
3. **El timer cambiará automáticamente** entre trabajo y descanso
4. **Recibirás alarmas visuales y sonoras** al completar cada sesión

## 🎛️ Controles

| Botón | Función |
|-------|---------|
| **Iniciar** | Comienza o continúa el timer |
| **Pausar** | Pausa el timer actual |
| **Reiniciar** | Reinicia el timer actual |
| **⚙️ Configuración** | Abre panel de configuración |
| **🔔 Probar** | Prueba las notificaciones |
| **⚙️ Permisos** | Solicita permisos de notificación |

## 📱 Responsive Design

- **Escritorio**: Interfaz completa con todos los controles
- **Móvil**: Diseño adaptado con controles optimizados
- **Tablet**: Experiencia híbrida con controles táctiles

## 🔧 Tecnologías Utilizadas

- **HTML5**: Estructura semántica
- **CSS3**: Animaciones, gradientes, glassmorphism
- **JavaScript ES6+**: Lógica del timer y notificaciones
- **Web APIs**: Notifications API, AudioContext
- **LocalStorage**: Persistencia de configuración

## 🎨 Personalización

### Cambiar Colores
Edita las variables CSS en el archivo `index.html`:
```css
.timer-circle.work {
    border-color: #ff6b6b; /* Color de trabajo */
}
.timer-circle.break {
    border-color: #4ecdc4; /* Color de descanso */
}
```

### Agregar Sonidos Personalizados
Modifica la función `playAlarmSound()` para usar archivos de audio:
```javascript
// Reemplaza la generación de sonidos con:
const audio = new Audio('alarm.mp3');
audio.play();
```

## 🐛 Solución de Problemas

### Las notificaciones no funcionan
1. **Verifica permisos**: El estado debe mostrar "✅ Permitidas"
2. **Navegador compatible**: Usa Chrome, Firefox, Edge o Safari
3. **No modo incógnito**: Las notificaciones no funcionan en modo privado
4. **Configuración del navegador**: Revisa la configuración de notificaciones

### El sonido no se reproduce
1. **Volumen del navegador**: Verifica que no esté silenciado
2. **Permisos de audio**: Algunos navegadores requieren interacción del usuario
3. **Navegador actualizado**: Usa la versión más reciente

## 📈 Próximas Mejoras

- [ ] **Temas personalizables** (oscuro, claro, colores)
- [ ] **Sonidos personalizados** (subir archivos de audio)
- [ ] **Estadísticas avanzadas** (gráficos, reportes)
- [ ] **Modo offline** (PWA)
- [ ] **Integración con calendarios**
- [ ] **Sincronización entre dispositivos**

## 🤝 Contribuciones

¡Las contribuciones son bienvenidas! Si tienes ideas para mejorar el proyecto:

1. **Fork** el repositorio
2. **Crea una rama** para tu feature (`git checkout -b feature/nueva-funcionalidad`)
3. **Commit** tus cambios (`git commit -m 'Agregar nueva funcionalidad'`)
4. **Push** a la rama (`git push origin feature/nueva-funcionalidad`)
5. **Abre un Pull Request**

## 📄 Licencia

Este proyecto está bajo la Licencia MIT. Ver el archivo `LICENSE` para más detalles.

## 👨‍💻 Autor

**Tu Nombre**
- GitHub: [@tu-usuario](https://github.com/tu-usuario)
- Email: tu-email@ejemplo.com

## 🙏 Agradecimientos

- **Técnica Pomodoro** por Francesco Cirillo
- **Comunidad de desarrolladores** por las ideas y feedback
- **Contribuidores** que han ayudado a mejorar el proyecto

---

⭐ **¡Si te gusta este proyecto, dale una estrella en GitHub!** ⭐