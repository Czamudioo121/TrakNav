# 🚀 TrakNav - Aplicación de Navegación y Seguimiento GPS

TrakNav es una aplicación móvil desarrollada en Flutter que combina navegación GPS inteligente con planificación de viajes avanzada. La aplicación está diseñada para fomentar el turismo mediante recomendaciones contextuales y una experiencia de viaje simple e intuitiva.

## 🎯 Objetivo del Proyecto

El objetivo es crear una aplicación móvil que ofrezca información relevante y recomendaciones de sitios cercanos, con funcionalidades de:
- Geolocalización en tiempo real
- Búsqueda de sitios y catálogo por categorías  
- Recomendaciones personalizadas según preferencias e historial
- Gestión de favoritos y soporte multiusuario
- Itinerarios con planificación diaria y guía de trayecto óptimo

## 📱 Características Principales

### 🗺️ Navegación y Mapas
- **Google Maps Integration** - Mapas interactivos con navegación en tiempo real
- **Seguimiento GPS** - Monitoreo preciso de ubicación en tiempo real
- **Planificación de Rutas** - Creación y gestión de rutas personalizadas
- **Múltiples medios de transporte** - A pie, bicicleta, auto y transporte público

### 👥 Gestión de Usuarios
- **Autenticación Firebase** - Sistema de registro e inicio de sesión seguro
- **Multi-usuario** - Soporte para múltiples perfiles de usuario
- **Sincronización en la nube** - Datos respaldados con Cloud Firestore
- **Recuperación de contraseña** - Sistema de seguridad integrado

### 🌟 Funcionalidades Adicionales
- **Planes de Viaje** - Crear, editar y gestionar itinerarios de hasta 7 días
- **Lugares Favoritos** - Guarda y gestiona ubicaciones importantes
- **Información Climática** - Datos meteorológicos integrados por ubicación
- **FAQs Integradas** - Centro de ayuda dentro de la aplicación
- **Modo Oscuro** - Interfaz adaptable para mejor experiencia
- **Interfaz Multiidioma** - Soporte para localización

## 🛠️ Stack Tecnológico

### **Frontend**
- **Flutter** (SDK >=3.0.0) - Framework de desarrollo multiplataforma
- **Dart** - Lenguaje de programación principal

### **Backend & Servicios**
- **Firebase Core** - Plataforma de desarrollo backend
- **Firebase Auth** - Autenticación de usuarios
- **Cloud Firestore** - Base de datos NoSQL en tiempo real

### **Mapas y Ubicación**
- **Google Maps Flutter** - Integración de mapas
- **Google Places** - API de lugares y búsqueda
- **Location Services** - Servicios de geolocalización
- **Permission Handler** - Gestión de permisos del dispositivo

### **Arquitectura y Estado**
- **Flutter BLoC** - Gestión de estado reactiva
- **Auto Route** - Navegación declarativa
- **Freezed** - Generación de código inmutable
- **JSON Serializable** - Serialización de datos

## 🚀 Instalación y Configuración

### Prerrequisitos
```bash
# Verificar instalación de Flutter
flutter --version

# Verificar dispositivos disponibles
flutter devices
```

### Configuración del Proyecto

1. **Clonar el repositorio**
```bash
git clone https://github.com/Czamudioo121/TrakNav.git
cd TrakNav
```

2. **Instalar dependencias**
```bash
flutter pub get
```

3. **Generar archivos de configuración**
```bash
flutter packages pub run build_runner build --delete-conflicting-outputs
```

4. **Configurar Firebase**
   - Crear proyecto en Firebase Console
   - Descargar `google-services.json` (Android) 
   - Configurar `GoogleService-Info.plist` (iOS)
   - Habilitar Authentication y Firestore
   - Configurar reglas de seguridad en Firestore

5. **Configurar Google Maps API**
   - Obtener API Key de Google Cloud Console
   - Configurar en `android/app/src/main/AndroidManifest.xml`
   - Configurar en `ios/Runner/AppDelegate.swift`

### Ejecutar la Aplicación

```bash
# Modo debug
flutter run

# Modo release
flutter run --release

# Para dispositivo específico
flutter run -d <device-id>
```

## 📂 Estructura del Proyecto

```
TrakNav/
├── lib/
│   ├── core/           # Configuración base, constantes, servicios
│   ├── features/       # Módulos: auth, home, map, travel_plan, favorites
│   ├── shared/         # Widgets, temas, utilidades, localización
│   ├── router/         # Rutas (auto_route)
│   ├── blocs/          # BLoCs/Cubits por feature
│   ├── models/         # Modelos (freezed, json_serializable)
│   └── main.dart       # Punto de entrada
├── assets/
│   ├── signin/         # Recursos de autenticación
│   ├── home/           # Recursos de pantalla principal
│   ├── favoritos/      # Recursos de favoritos
│   ├── TravelPlan/     # Recursos de planificación
│   ├── clima/          # Recursos climáticos
│   └── MyProfile/      # Recursos de perfil
├── android/            # Configuración Android
├── ios/                # Configuración iOS
└── test/              # Pruebas unitarias
```

## 🔧 Scripts Disponibles

```bash
# Análisis de código
flutter analyze

# Ejecutar pruebas
flutter test

# Generar APK
flutter build apk

# Generar bundle para Play Store
flutter build appbundle

# Limpiar proyecto
flutter clean
```

## 📋 Dependencias Principales

| Dependencia | Versión | Propósito |
|------------|---------|-----------|
| `google_maps_flutter` | ^2.5.0 | Integración de Google Maps |
| `firebase_auth` | ^4.12.1 | Autenticación de usuarios |
| `cloud_firestore` | ^4.13.3 | Base de datos NoSQL |
| `flutter_bloc` | ^8.1.3 | Gestión de estado |
| `location` | ^5.0.3 | Servicios de ubicación |
| `auto_route` | ^7.8.4 | Navegación automática |
| `google_places_flutter` | ^2.0.6 | Búsqueda de lugares |
| `permission_handler` | ^11.0.1 | Gestión de permisos |

## 🧱 Reglas de Negocio

- **Seguridad de contraseñas**: Mínimo 8 caracteres con mayúscula, minúscula, número y carácter especial
- **Multiusuario habilitado**: Acciones clave requieren sesión activa
- **Límites de itinerario**: Máximo 7 días por plan de viaje
- **Rutas en curso**: No iniciar nueva ruta si hay una activa
- **Estándares de accesibilidad**: Cumplimiento WCAG
- **Protección de datos**: Información personal y ubicaciones protegidas

## ⚙️ Requisitos del Sistema

### **Funcionales**
- Registro y autenticación de usuarios
- Búsqueda y filtrado de lugares por categorías
- Creación y edición de planes de viaje
- Navegación GPS con múltiples medios de transporte
- Gestión de favoritos y recomendaciones personalizadas

### **No Funcionales**
- **Plataforma**: Android (principal)
- **Consumo**: Optimizado para bajo consumo de batería
- **Rendimiento**: Binario < 1 GB, dispositivo con ≥ 4 GB RAM
- **Disponibilidad**: Sujeta al dispositivo local del usuario
- **Seguridad**: Protección de datos sensibles en Firebase

## ✅ Resultados de Pruebas

El proyecto ha sido sometido a pruebas funcionales exhaustivas con los siguientes resultados:

### **Pruebas por Módulo**
- **Crear cuenta**: 100% funcionalidad (7/7)
- **Seleccionar preferencias**: 100% (4/4)  
- **Inicio de sesión**: 91% (10/11)
- **Cambio de idioma**: 70% (7/10)
- **Crear plan de viaje**: 95% (25/26)
- **Catálogos**: 94% (13/14)
- **Editar plan**: 100% (25/25)
- **FAQ**: 100% (7/7)
- **Ubicación actual**: 86% (12/14)
- **Información climática**: 100% (5/5)
- **Favoritos**: 100% (4/4)
- **Recomendaciones**: 88% (8/9)
- **Trayecto óptimo**: 100% (6/6)

### **Evaluación de Usabilidad**
**Fortalezas identificadas:**
- Propuesta de valor diferencial para turistas
- Interfaz atractiva y fácil de usar
- Funcionalidades bien integradas

**Áreas de mejora:**
- Notificaciones y mensajes de error más específicos
- Optimización de rendimiento del mapa
- Integración completa de recuperación de contraseña
- Mejoras en accesibilidad de funciones

## 🗺️ Roadmap de Desarrollo

### **Próximas Mejoras**
- [ ] Notificaciones push para alertas de ubicación
- [ ] Modo offline con mapas descargados  
- [ ] Integración con Wearables
- [ ] Análisis de patrones de viaje
- [ ] Compartir ubicación en tiempo real
- [ ] Crashlytics y métricas de estabilidad
- [ ] Tests instrumentados en dispositivos reales

### **Optimizaciones Técnicas**
- [ ] Mejorar onboarding y discoverability
- [ ] Completar transporte público en rutas
- [ ] Internacionalización completa
- [ ] Panel de telemetría y calidad
- [ ] Caché inteligente para mejor rendimiento

## 🤝 Contribución

Las contribuciones son bienvenidas. Para contribuir:

1. Fork el proyecto
2. Crea una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

## 📄 Documentación Adicional

- **[Documentación Técnica Completa](./Documentacion.pdf)** - Documentación detallada del proyecto incluyendo alcance, sprints, casos de uso, pruebas y evaluaciones
- **[Documentación Comprimida](./Traknav-comprimido.pdf)** - Versión resumida para consulta rápida

## 🏫 Información Académica

**Proyecto desarrollado en:**
- **Instituto Politécnico Nacional**
- **Escuela Superior de Cómputo**
- **Ingeniería en Sistemas Computacionales**
- **Grupo:** 5CM2
- **Profesora:** Maldonado Castillo Idalia
- **Fecha:** 18 de Diciembre 2023

**Equipo de Desarrollo "Los Maquiavélicos":**
- Buendia Velazco Abel
- Cruz de la Vega Edmundo Alejandro  
- Herrera Albavera Luis Enrique
- Juseppe Pérez Julio Cesar
- Martinez Acosta José Miguel
- Muñoz Tapia Alan Arath
- Ortega Santiago Aaron Uriel
- Ramirez Garcia Juan Carlos
- Ramirez López Felipe Hiram
- Vázquez Cisneros Miguel Angel
- **Zamudio Onofre Cesar Osvaldo** (Autor del repositorio)

## 👨‍💻 Autor del Repositorio

**Cesar Zamudio** - [@Czamudioo121](https://github.com/Czamudioo121)
- 📍 Ubicación: CDMX, México
- 📧 Contacto: [GitHub Profile](https://github.com/Czamudioo121)

---

### 🚀 ¿Listo para navegar? ¡Explora el mundo con TrakNav! 

*Desarrollado con ❤️ usando Flutter por el equipo Los Maquiavélicos*
