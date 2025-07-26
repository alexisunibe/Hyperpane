# Hyperpane
# 🚀 Hyperpane Fase 2 - Escritorio Expandido Avanzado

**Hyperpane** es una aplicación de escritorio expandido revolucionaria que transforma tu experiencia de navegación horizontal con funcionalidades avanzadas, wallpapers animados, magnetización inteligente de ventanas y un sistema completo de gestión de perfiles.

![Hyperpane Icon](Resources/hyperpane-icon-256.png)

## ✨ **Características Principales**

### 🎯 **Navegación Fluida y Física Realista**
- **Inercia y fricción** en el movimiento del escritorio
- **Animaciones suaves** con 60 FPS optimizadas
- **Gestos avanzados** del mouse y teclado
- **Navegación con rueda del mouse** y arrastre intuitivo
- **Física realista** con decaimiento de velocidad y rebote

### 🗺️ **MiniMap Inteligente**
- **Navegación visual** con vista previa del workspace
- **Marcadores personalizables** con colores y nombres
- **Zoom independiente** del minimapa
- **Modo compacto** para ahorrar espacio
- **Sincronización bidireccional** con el workspace
- **Tooltips informativos** y menú contextual
- **Configuración persistente** automática

### 🧲 **Magnetización de Ventanas**
- **Zonas magnéticas** predefinidas y personalizables
- **Detección automática** de ventanas del sistema
- **Snap inteligente** con animaciones suaves
- **Gestión de múltiples monitores**
- **Configuración de sensibilidad** ajustable

### 🎨 **Wallpapers Animados**
- **Soporte para videos** como wallpapers de fondo
- **Imágenes estáticas** con desplazamiento suave
- **Control de volumen** y reproducción en bucle
- **Múltiples formatos** soportados (MP4, AVI, MOV, etc.)
- **Optimización de memoria** automática

### 🚀 **Integración con Wallpaper Engine**
- **Detección automática** de Wallpaper Engine
- **Modo transparente** para wallpapers de Wallpaper Engine
- **Resolución extendida** simulando múltiples monitores
- **Configuración inteligente** y recomendaciones automáticas
- **Sincronización perfecta** entre Hyperpane y Wallpaper Engine

### 🔧 **Compatibilidad Universal**
- **Detección automática** de apps de terceros (Fences, Rainmeter, FancyZones, etc.)
- **Anclaje al escritorio** para coexistir sin conflictos
- **Click-through condicional** para permitir interacción con otras apps
- **Configuración dinámica** según el entorno detectado
- **Compatibilidad total** con herramientas populares de escritorio

### 📐 **Múltiples Layouts**
- **Layouts predefinidos**: Horizontal, Vertical, Grid, Freeform
- **Transiciones visuales** entre layouts
- **Configuración personalizable** por layout
- **Activación automática** según el contenido

### 👤 **Sistema de Perfiles**
- **Perfiles de usuario** con configuraciones completas
- **Guardado automático** de preferencias
- **Cambio rápido** entre perfiles
- **Sincronización** de todos los componentes

### 🎭 **Transiciones Visuales**
- **Múltiples tipos**: Fade, Slide, Zoom, Rotate
- **Duración configurable** y easing personalizable
- **Transiciones automáticas** entre layouts
- **Efectos visuales** profesionales

### ⚙️ **Panel de Configuración Completo**
- **Configuración de navegación** y física
- **Gestión de wallpapers** y layouts
- **Configuración de perfiles** y magnetización
- **Ajustes de rendimiento** y optimización
- **Interfaz intuitiva** con categorías organizadas

### 💾 **Auto-Guardado Inteligente**
- **Guardado automático** cada 30 segundos
- **Restauración de sesión** al iniciar
- **Múltiples backups** con rotación automática
- **Recuperación de errores** robusta

### 🔧 **Modo Desarrollador**
- **Información en tiempo real** de rendimiento
- **Monitoreo de memoria** y CPU
- **Logs detallados** de eventos
- **Herramientas de diagnóstico** avanzadas

## 🎮 **Controles y Navegación**

### **Mouse**
- **Clic izquierdo + arrastre**: Navegar por el workspace
- **Rueda del mouse**: Scroll horizontal
- **Shift + rueda**: Scroll horizontal preciso
- **Ctrl + rueda**: Zoom del workspace
- **Doble clic**: Centrar en posición
- **Botón medio + arrastre**: Navegación manual

### **Teclado**
- **Flechas izquierda/derecha**: Navegación paso a paso
- **Home/End**: Ir al inicio/fin del workspace
- **Espacio**: Pausar/reanudar wallpaper
- **F1**: Abrir panel de configuración
- **F2**: Activar/desactivar modo desarrollador
- **F3**: Toggle magnetización de ventanas
- **F4**: Probar transiciones

### **MiniMap**
- **Clic**: Saltar a posición
- **Arrastre del thumb**: Navegación directa
- **Ctrl + rueda**: Zoom del minimapa
- **Clic derecho**: Menú contextual
- **Botones +/-**: Control de zoom

## 🏗️ **Arquitectura del Proyecto**

```
Hyperpane/
├── Core/
│   ├── ViewportManager.cs          # Gestión de viewport con física
│   └── WorkspaceCanvas.cs          # Canvas optimizado del workspace
├── Input/
│   └── SlideController.cs          # Control de gestos y navegación
├── Logic/
│   └── WorkspaceCanvas.cs          # Lógica del workspace
├── Services/
│   ├── WallpaperManager.cs         # Gestión de wallpapers
│   ├── AutoDetectManager.cs        # Detección de Wallpaper Engine
│   ├── CompatibilityManager.cs     # Compatibilidad con apps de terceros
│   ├── WindowMagnetizer.cs         # Magnetización de ventanas
│   ├── WorkspaceLayoutManager.cs   # Gestión de layouts
│   ├── ProfileManager.cs           # Gestión de perfiles
│   ├── TransitionManager.cs        # Transiciones visuales
│   ├── AutoSaveManager.cs          # Auto-guardado
│   └── DeveloperOverlay.cs         # Modo desarrollador
├── UI/
│   ├── MiniMap.xaml               # Interfaz del minimapa
│   ├── MiniMap.xaml.cs            # Lógica del minimapa
│   └── SettingsPanel.xaml         # Panel de configuración
├── Config/
│   ├── AppSettings.cs             # Configuración de la aplicación
│   └── PerformanceConfig.cs       # Configuración de rendimiento
├── Utils/                         # Utilidades y helpers
├── Resources/                     # Iconos y recursos visuales
│   ├── hyperpane-icon.svg         # SVG original del icono
│   ├── hyperpane-icon.ico         # Icono principal de la aplicación
│   ├── IconResources.xaml         # Recursos XAML de iconos
│   └── Scripts/                   # Scripts de generación
├── MainWindow.xaml                # Ventana principal
├── MainWindow.xaml.cs             # Lógica de la ventana principal
├── App.xaml                       # Configuración de la aplicación
├── App.xaml.cs                    # Punto de entrada
└── Hyperpane.csproj               # Archivo de proyecto optimizado
```

## 🚀 **Optimizaciones de Rendimiento**

### **Optimizaciones Implementadas**
- ✅ **Gestión de memoria mejorada** con IDisposable en todos los componentes
- ✅ **Constantes optimizadas** para reducir cálculos en tiempo de ejecución
- ✅ **Detección de elementos visibles** para renderizado eficiente
- ✅ **Animaciones optimizadas** con 60 FPS exactos
- ✅ **Limpieza automática de recursos** al cerrar la aplicación
- ✅ **Configuración centralizada** de rendimiento
- ✅ **Manejo de errores robusto** con try-catch optimizados
- ✅ **Reducción de allocations** de memoria
- ✅ **Timers optimizados** para mejor rendimiento
- ✅ **Caché de imágenes** con límites de memoria

### **Configuración de Rendimiento**
- **Frame Rate**: 60 FPS constante
- **Memoria**: Límite de 100MB para caché
- **Animaciones**: Duración optimizada según modo
- **Física**: Constantes ajustadas para fluidez
- **Auto-guardado**: Cada 30 segundos sin impacto en UI

## 🛠️ **Tecnologías Utilizadas**

- **.NET 6.0** - Framework moderno y optimizado
- **WPF (Windows Presentation Foundation)** - Interfaz de usuario avanzada
- **XAML** - Diseño declarativo de UI
- **C# 10.0** - Lenguaje moderno con características avanzadas
- **System.Windows.Media** - Animaciones y efectos visuales
- **System.Windows.Threading** - Gestión de hilos y timers
- **System.Xml.Serialization** - Persistencia de configuración

## 🎨 **Sistema de Iconos**

Hyperpane incluye un sistema de iconos moderno y escalable:

### **Características del Icono**
- **Diseño vectorial** basado en SVG para escalabilidad perfecta
- **Gradiente moderno** verde-azul-morado (#4CAF50 → #2196F3 → #9C27B0)
- **Múltiples formatos** ICO, PNG en diferentes resoluciones
- **Integración nativa** con Windows y WPF

### **Generación de Iconos**
```powershell
# Generar todos los iconos desde el SVG
.\Scripts\generate-icons.ps1
```

### **Documentación Completa**
- 📖 [Guía del Sistema de Iconos](ICON_SYSTEM.md) - Documentación detallada
- 🎯 [Guía de Compatibilidad](COMPATIBILITY_GUIDE.md) - Compatibilidad con apps de terceros

## 📦 **Instalación y Uso**

### **Requisitos del Sistema**
- Windows 10/11 (64-bit)
- .NET 6.0 Runtime
- 4GB RAM mínimo (8GB recomendado)
- Tarjeta gráfica compatible con DirectX 11
- **ImageMagick** (opcional, para generar iconos)

### **Instalación**
1. Descargar la aplicación desde el repositorio
2. Ejecutar `Hyperpane.exe`
3. La aplicación se iniciará automáticamente
4. Configurar preferencias en el panel de configuración (F1)

### **Primera Configuración**
1. **Añadir wallpaper**: Arrastrar imagen/video al workspace
2. **Configurar layouts**: Seleccionar layout preferido
3. **Ajustar magnetización**: Configurar zonas magnéticas
4. **Crear perfil**: Guardar configuración personalizada
5. **Integrar Wallpaper Engine**: Configurar modo extendido (opcional)

### **Integración con Wallpaper Engine**
Para una experiencia visual completa, consulta el archivo `WALLPAPER_ENGINE_INTEGRATION.md` que incluye:
- Guía de instalación y configuración
- Solución de problemas comunes
- Casos de uso específicos
- Configuración avanzada

### **Compatibilidad Universal**
Para información detallada sobre compatibilidad con herramientas de terceros, consulta el archivo `COMPATIBILITY_GUIDE.md` que incluye:
- Compatibilidad con Fences, Rainmeter, FancyZones, etc.
- Configuración automática y manual
- Solución de problemas de compatibilidad
- Casos de uso específicos por herramienta

## 🎯 **Casos de Uso**

### **Desarrollo y Diseño**
- **Workspace expandido** para múltiples herramientas
- **Organización visual** de proyectos
- **Navegación rápida** entre aplicaciones
- **Configuración personalizada** por proyecto

### **Productividad**
- **Gestión de ventanas** automatizada
- **Acceso rápido** a aplicaciones frecuentes
- **Organización visual** del escritorio
- **Transiciones suaves** entre tareas

### **Entretenimiento**
- **Wallpapers animados** personalizados
- **Experiencia inmersiva** con navegación fluida
- **Configuración de múltiples monitores**
- **Gestión de contenido multimedia**

## ⚙️ **Configuración Avanzada**

### **Archivos de Configuración**
- `session.json` - Estado de la sesión actual
- `profiles.json` - Perfiles de usuario
- `minimap_config.xml` - Configuración del minimapa
- `appsettings.json` - Configuración general

### **Personalización**
- **Colores y temas** personalizables
- **Sensibilidad de gestos** ajustable
- **Velocidades de animación** configurables
- **Zonas magnéticas** personalizables

## 🔧 **Solución de Problemas**

### **Problemas Comunes**
1. **Rendimiento lento**: Verificar configuración de gráficos
2. **Wallpapers no cargan**: Verificar formato de archivo
3. **Magnetización no funciona**: Verificar permisos de ventana
4. **Configuración no se guarda**: Verificar permisos de escritura

### **Logs y Diagnóstico**
- **Modo desarrollador** (F2) para información detallada
- **Logs automáticos** en `logs/` directory
- **Información de rendimiento** en tiempo real
- **Diagnóstico de memoria** y CPU

## 🔮 **Próximas Mejoras**

### **Fase 3 (Planificada)**
- [ ] **Soporte para múltiples monitores** avanzado
- [ ] **Plugins y extensiones** del sistema
- [ ] **Integración con la nube** para sincronización
- [ ] **Temas personalizables** completos
- [ ] **Gestión de espacios de trabajo** virtuales
- [ ] **Integración con APIs** de terceros
- [ ] **Soporte para gestos táctiles** en pantallas táctiles
- [ ] **Optimizaciones de IA** para organización automática

### **Mejoras de Rendimiento**
- [ ] **Renderizado GPU** acelerado
- [ ] **Compresión de memoria** avanzada
- [ ] **Lazy loading** de componentes
- [ ] **Optimización de red** para wallpapers remotos

## 📄 **Licencia**

Este proyecto está bajo la Licencia MIT. Ver el archivo `LICENSE` para más detalles.

## 🤝 **Contribuciones**

Las contribuciones son bienvenidas. Por favor, lee las guías de contribución antes de enviar un pull request.

## 📞 **Soporte**

Para soporte técnico o preguntas:
- Crear un issue en el repositorio
- Consultar la documentación
- Usar el modo desarrollador para diagnóstico

---

**Hyperpane Fase 2** - Transformando la experiencia del escritorio expandido con tecnología avanzada y optimizaciones de rendimiento profesional. 🚀 
