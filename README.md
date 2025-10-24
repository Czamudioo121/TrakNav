# 🚀 TrakNav - Aplicación de Navegación GPS y Planificación de Viajes

**TrakNav** es una solución integral de navegación GPS y planificación turística desarrollada con metodologías ágiles SCRUM. La aplicación combina tecnologías modernas de Flutter con servicios en la nube para ofrecer una experiencia completa de viajes personalizados y navegación inteligente.

## 📑 Tabla de Contenidos

1. [🎯 Visión del Proyecto](#1-visión-del-proyecto)
2. [📋 Metodología de Desarrollo](#2-metodología-de-desarrollo)
   - 2.1 [SCRUM Framework](#21-scrum-framework)
   - 2.2 [Sprint Planning Overview](#22-sprint-planning-overview)
   - 2.3 [Equipo SCRUM "Los Maquiavélicos"](#23-equipo-scrum-los-maquiavélicos)
3. [🏗️ Arquitectura y Stack Tecnológico](#3-arquitectura-y-stack-tecnológico)
   - 3.1 [Frontend & Framework](#31-frontend--framework)
   - 3.2 [Backend & Servicios en la Nube](#32-backend--servicios-en-la-nube)
   - 3.3 [APIs y Servicios Externos](#33-apis-y-servicios-externos)
   - 3.4 [Herramientas de Desarrollo](#34-herramientas-de-desarrollo)
4. [📱 Funcionalidades Principales](#4-funcionalidades-principales)
   - 4.1 [🔐 Gestión de Usuarios Avanzada](#41-gestión-de-usuarios-avanzada)
   - 4.2 [🗺️ Navegación y Mapas Inteligentes](#42-navegación-y-mapas-inteligentes)
   - 4.3 [📅 Planificación de Viajes Profesional](#43-planificación-de-viajes-profesional)
   - 4.4 [⭐ Sistema de Favoritos y Recomendaciones](#44-sistema-de-favoritos-y-recomendaciones)
   - 4.5 [🌤️ Información Contextual](#45-información-contextual)
5. [🛠️ Implementación y Configuración](#5-implementación-y-configuración)
   - 5.1 [Prerrequisitos del Sistema](#51-prerrequisitos-del-sistema)
   - 5.2 [Configuración del Proyecto](#52-configuración-del-proyecto)
   - 5.3 [Comandos de Desarrollo](#53-comandos-de-desarrollo)
6. [🔧 Arquitectura del Sistema](#6-arquitectura-del-sistema)
   - 6.1 [Patrón BLoC (Business Logic Component)](#61-patrón-bloc-business-logic-component)
   - 6.2 [Flujo de Datos](#62-flujo-de-datos)
7. [⚙️ Reglas de Negocio y Validaciones](#7-reglas-de-negocio-y-validaciones)
   - 7.1 [Seguridad y Autenticación](#71-seguridad-y-autenticación)
   - 7.2 [Limitaciones Funcionales](#72-limitaciones-funcionales)
   - 7.3 [Estándares de Calidad](#73-estándares-de-calidad)
8. [📊 Resultados de Testing y Calidad](#8-resultados-de-testing-y-calidad)
   - 8.1 [Testing Automatizado por Módulos](#81-testing-automatizado-por-módulos)
   - 8.2 [Evaluación de Usabilidad Profesional](#82-evaluación-de-usabilidad-profesional)
9. [🚀 Roadmap de Evolución](#9-roadmap-de-evolución)
   - 9.1 [Fase 1: Optimización](#91-fase-1-optimización)
   - 9.2 [Fase 2: Expansión](#92-fase-2-expansión)
   - 9.3 [Fase 3: Inteligencia](#93-fase-3-inteligencia)
10. [📈 Métricas de Rendimiento](#10-métricas-de-rendimiento)
    - 10.1 [Benchmarks Técnicos](#101-benchmarks-técnicos)
    - 10.2 [KPIs de Negocio](#102-kpis-de-negocio)
11. [🏫 Contexto Académico](#11-contexto-académico)
    - 11.1 [Equipo de Desarrollo](#111-equipo-de-desarrollo)
12. [📄 Documentación Técnica](#12-documentación-técnica)
13. [👨‍💻 Información del Autor](#13-información-del-autor)

## 1. 🎯 Visión del Proyecto

Fomentar el turismo mediante una plataforma móvil que proporcione información relevante, recomendaciones contextuales y herramientas de planificación avanzadas. El objetivo es crear una experiencia de viaje intuitiva que integre geolocalización, recomendaciones personalizadas y navegación optimizada según el medio de transporte.

## 2. 📋 Metodología de Desarrollo

### 2.1 **SCRUM Framework**
El proyecto fue desarrollado utilizando **metodología SCRUM** con 8 sprints estructurados que abarcaron desde la conceptualización hasta la implementación completa:

### 2.2 **Sprint Planning Overview**
- **Sprint 1** (20-22 Sep 2023): Definición de alcance, requerimientos y reglas de negocio
- **Sprint 2** (22-29 Sep 2023): Desarrollo de prototipos no funcionales y diseño de interfaces
- **Sprint 3** (09-13 Oct 2023): Refinamiento de interfaces y casos de uso suplementarios
- **Sprint 4** (16-20 Oct 2023): Implementación de casos de uso fundamentales
- **Sprint 5** (23 Oct-03 Nov 2023): Configuración de entornos, Firebase y definición del MVP
- **Sprint 6** (06-28 Nov 2023): Desarrollo del frontend e integración de APIs
- **Sprint 7** (29 Nov-12 Dic 2023): Implementación del backend y testing integral
- **Sprint 8** (13-19 Dic 2023): Integración final, pruebas y optimización

### 2.3 **Equipo SCRUM "Los Maquiavélicos"**
Equipo multidisciplinario de 11 desarrolladores con roles especializados en frontend, backend, documentación técnica, testing y arquitectura de sistemas.

## 3. 🏗️ Arquitectura y Stack Tecnológico

### 3.1 **Frontend & Framework**
- **Flutter** (SDK >=3.0.0) - Desarrollo multiplataforma nativo
- **Dart** - Lenguaje de programación principal
- **BLoC Pattern** - Arquitectura de gestión de estado reactiva
- **Auto Route** - Sistema de navegación declarativa

### 3.2 **Backend & Servicios en la Nube**
- **Firebase Core** - Plataforma backend como servicio
- **Firebase Authentication** - Autenticación segura multiproveedor
- **Cloud Firestore** - Base de datos NoSQL en tiempo real
- **Firebase Dynamic Links** - Enlaces dinámicos para compartir

### 3.3 **APIs y Servicios Externos**
- **Google Maps Flutter** - Mapas interactivos y navegación
- **Google Places API** - Búsqueda y información de lugares
- **Google Maps Webservice** - Servicios de geocodificación y rutas
- **Weather API** - Información meteorológica contextual

### 3.4 **Herramientas de Desarrollo**
- **Freezed** - Generación de código inmutable
- **JSON Serializable** - Serialización automática de datos
- **Build Runner** - Generación de código automatizada
- **Flutter Lints** - Análisis estático de código

## 4. 📱 Funcionalidades Principales

### 4.1 **🔐 Gestión de Usuarios Avanzada**
- Autenticación Firebase con validación robusta
- Sistema multiusuario con cambio de cuentas dinámico
- Recuperación de contraseñas con preguntas de seguridad
- Perfiles personalizables con preferencias de viaje

### 4.2 **🗺️ Navegación y Mapas Inteligentes**
- Geolocalización en tiempo real con GPS de alta precisión
- Rutas optimizadas para múltiples medios de transporte:
  - **A pie** - Rutas peatonales optimizadas
  - **Bicicleta** - Ciclovías y rutas ciclistas
  - **Automóvil** - Navegación vehicular con tráfico
  - **Transporte público** - Integración con sistemas urbanos
- Búsqueda contextual con autocompletado inteligente

### 4.3 **📅 Planificación de Viajes Profesional**
- Creación de itinerarios de hasta 7 días
- Algoritmo de recomendaciones basado en:
  - Preferencias del usuario
  - Historial de visitas
  - Proximidad geográfica
  - Calificaciones comunitarias
- Gestión completa de planes: crear, editar, duplicar, eliminar

### 4.4 **⭐ Sistema de Favoritos y Recomendaciones**
- Gestión inteligente de lugares favoritos
- Recomendaciones personalizadas por categorías
- Integración con Google Places para información actualizada
- Compartir ubicaciones mediante enlaces dinámicos

### 4.5 **🌤️ Información Contextual**
- Datos meteorológicos en tiempo real
- Notificaciones climáticas por ubicación
- Información de horarios y disponibilidad de establecimientos
- Catálogo extenso por categorías (restaurantes, museos, hoteles, etc.)

## 5. 🛠️ Implementación y Configuración

### 5.1 **Prerrequisitos del Sistema**
```bash
Flutter SDK >=3.0.0
Dart >=3.0.0
Android Studio / VS Code
Git para control de versiones
```

### 5.2 **Configuración del Proyecto**

1. **Clonar y configurar dependencias**
```bash
git clone https://github.com/Czamudioo121/TrakNav.git
cd TrakNav
flutter pub get
flutter packages pub run build_runner build --delete-conflicting-outputs
```

2. **Configuración de Firebase**
```bash
# Instalar Firebase CLI
npm install -g firebase-tools

# Configurar proyecto Firebase
firebase login
firebase projects:list
```

3. **Configuración de APIs de Google**
- Habilitar Google Maps SDK para Android/iOS
- Configurar Google Places API
- Obtener claves API y configurar en:
  - `android/app/src/main/AndroidManifest.xml`
  - `ios/Runner/AppDelegate.swift`

4. **Estructura de configuración**
```
android/
  app/
    src/main/
      AndroidManifest.xml  # Google Maps API Key
      google-services.json # Firebase Config
ios/
  Runner/
    Info.plist           # iOS Configuration
    GoogleService-Info.plist # Firebase iOS
```

### 5.3 **Comandos de Desarrollo**

```bash
# Análisis de código
flutter analyze

# Ejecución en desarrollo
flutter run --debug

# Compilación para producción
flutter build apk --release
flutter build appbundle --release

# Testing automatizado
flutter test
```

## 6. 🔧 Arquitectura del Sistema

### 6.1 **Patrón BLoC (Business Logic Component)**
```
lib/
├── core/
│   ├── constants/         # Constantes globales
│   ├── errors/           # Manejo de errores
│   ├── services/         # Servicios compartidos
│   └── utils/            # Utilidades
├── features/
│   ├── auth/             # Autenticación
│   │   ├── bloc/         # Lógica de negocio
│   │   ├── data/         # Repositorios y modelos
│   │   └── presentation/ # Interfaces de usuario
│   ├── maps/             # Funcionalidades de mapas
│   ├── travel_plan/      # Planificación de viajes
│   ├── favorites/        # Gestión de favoritos
│   └── weather/          # Información climática
└── shared/
    ├── widgets/          # Componentes reutilizables
    ├── themes/           # Temas y estilos
    └── localization/     # Internacionalización
```

### 6.2 **Flujo de Datos**
1. **UI Layer** - Interfaces Flutter con widgets reactivos
2. **BLoC Layer** - Lógica de negocio y gestión de estados
3. **Repository Layer** - Abstracción de fuentes de datos
4. **Data Layer** - APIs, Firebase y almacenamiento local

## 7. ⚙️ Reglas de Negocio y Validaciones

### 7.1 **Seguridad y Autenticación**
- Contraseñas: mínimo 8 caracteres con mayúscula, minúscula, número y carácter especial
- Validación de correos electrónicos únicos por cuenta
- Preguntas de seguridad obligatorias para recuperación
- Sesiones seguras con tokens JWT de Firebase

### 7.2 **Limitaciones Funcionales**
- Máximo 7 días por itinerario de viaje
- Máximo 8 lugares por día en planes de viaje
- Restricción de rutas simultáneas (una activa por usuario)
- Geolocalización requerida para funcionalidades principales

### 7.3 **Estándares de Calidad**
- Cumplimiento WCAG 2.1 para accesibilidad
- Protección de datos personales (GDPR compliance)
- Optimización para dispositivos con ≥4GB RAM
- Aplicación <1GB de almacenamiento

## 8. 📊 Resultados de Testing y Calidad

### 8.1 **Testing Automatizado por Módulos**
El proyecto implementó testing exhaustivo con los siguientes resultados:

| Módulo | Funcionalidad | Cobertura |
|--------|---------------|-----------|
| **Autenticación** | Crear cuenta | 100% (7/7) |
| **Preferencias** | Selección inicial | 100% (4/4) |
| **Sesiones** | Inicio de sesión | 91% (10/11) |
| **Localización** | Cambio de idioma | 70% (7/10) |
| **Planificación** | Crear itinerario | 95% (25/26) |
| **Catálogos** | Navegación | 94% (13/14) |
| **Edición** | Modificar planes | 100% (25/25) |
| **Soporte** | FAQs | 100% (7/7) |
| **Geolocalización** | Ubicación actual | 86% (12/14) |
| **Clima** | Información meteorológica | 100% (5/5) |
| **Favoritos** | Gestión de lugares | 100% (4/4) |
| **Recomendaciones** | Algoritmo personalizado | 88% (8/9) |
| **Navegación** | Rutas óptimas | 100% (6/6) |

### 8.2 **Evaluación de Usabilidad Profesional**

**Fortalezas Identificadas:**
- Propuesta de valor única para el sector turístico
- Interfaz intuitiva con excelente experiencia de usuario
- Integración efectiva de servicios externos
- Rendimiento optimizado en dispositivos objetivo

**Áreas de Optimización:**
- Mensajes de error más contextuales y específicos
- Recuperación de contraseñas completamente in-app
- Optimización de rendimiento en mapas con muchos marcadores
- Internacionalización completa de formularios

## 9. 🚀 Roadmap de Evolución

### 9.1 **Fase 1: Optimización**
- [ ] Implementación de Crashlytics para telemetría
- [ ] Modo offline con caché inteligente de mapas
- [ ] Notificaciones push contextuales
- [ ] Métricas de uso y analytics avanzados

### 9.2 **Fase 2: Expansión**
- [ ] Integración con wearables (Apple Watch, Wear OS)
- [ ] Realidad aumentada para navegación
- [ ] Compartir ubicación en tiempo real
- [ ] API pública para desarrolladores

### 9.3 **Fase 3: Inteligencia**
- [ ] Machine Learning para recomendaciones
- [ ] Análisis predictivo de patrones de viaje
- [ ] Asistente virtual por voz
- [ ] Integración con IoT y ciudades inteligentes

## 10. 📈 Métricas de Rendimiento

### 10.1 **Benchmarks Técnicos**
- **Tiempo de inicio**: <3 segundos en dispositivos objetivo
- **Consumo de batería**: Optimizado para 8+ horas de uso continuo
- **Uso de memoria**: <512MB RAM promedio
- **Tamaño de aplicación**: <150MB instalación completa

### 10.2 **KPIs de Negocio**
- **Retención de usuarios**: Meta 70% a 30 días
- **Engagement**: Sesiones promedio >10 minutos
- **Conversión**: 85% de usuarios completan primer itinerario
- **Satisfacción**: Score NPS objetivo >50

## 11. 🏫 Contexto Académico

**Institución:** Instituto Politécnico Nacional - Escuela Superior de Cómputo  
**Carrera:** Ingeniería en Sistemas Computacionales  
**Materia:** Análisis y diseño de sistemas  
**Profesora:** Maldonado Castillo Idalia  
**Grupo:** 5CM2  
**Periodo:** Agosto - Diciembre 2023

### 11.1 **Equipo de Desarrollo**

**Scrum Master & Product Owner:**
- Martinez Acosta José Miguel

**Development Team:**
- Buendia Velazco Abel 
- Cruz de la Vega Edmundo Alejandro
- Herrera Albavera Luis Enrique 
- Juseppe Pérez Julio Cesar 
- Muñoz Tapia Alan Arath 
- Ortega Santiago Aaron Uriel 
- Ramirez Garcia Juan Carlos 
- Ramirez López Felipe Hiram 
- Vázquez Cisneros Miguel Angel
- Zamudio Onofre Cesar Osvaldo

## 12. 📄 Documentación Técnica

- **[Documentación Completa del Proyecto](./Documentacion.pdf)** - 200+ páginas con análisis completo, metodología SCRUM, casos de uso detallados, arquitectura del sistema, testing integral y evaluaciones de desempeño
- **[Presentación Ejecutiva](./Traknav-comprimido.pdf)** - Resumen ejecutivo para consulta rápida

## 13. 👨‍💻 Información del Autor

**Cesar Osvaldo Zamudio Onofre**  
[@Czamudioo121](https://github.com/Czamudioo121)

📍 **Ubicación:** Ciudad de México, México  
🎓 **Rol en el proyecto:** Development Team Member & Documentation Lead & Designer UI/UX
📧 **Contacto:** [GitHub Profile](https://github.com/Czamudioo121)

---

### 🌟 TrakNav representa la convergencia entre tecnología moderna, metodologías ágiles y experiencia de usuario excepcional

*Desarrollado con metodología SCRUM y tecnologías de vanguardia por el equipo "Los Maquiavélicos"*

**Stack Principal:** Flutter • Firebase • Google Maps • SCRUM • BLoC Pattern
