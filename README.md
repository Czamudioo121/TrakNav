# 🚀 TrakNav - Aplicación de Navegación GPS y Planificación de Viajes

**TrakNav** es una solución integral de navegación GPS y planificación turística desarrollada con metodologías ágiles SCRUM. La aplicación combina tecnologías modernas de Flutter con servicios en la nube para ofrecer una experiencia completa de viajes personalizados y navegación inteligente.

## 📑 Tabla de Contenidos

1. [🎯 Visión del Proyecto](#vision-del-proyecto)
2. [📋 Metodología de Desarrollo](#metodologia-de-desarrollo)
   - 2.1 [SCRUM Framework](#scrum-framework)
   - 2.2 [Sprint Planning Overview](#sprint-planning-overview)
   - 2.3 [Equipo SCRUM "Los Maquiavélicos"](#equipo-scrum-los-maquiavelicos)
3. [🏗️ Arquitectura y Stack Tecnológico](#arquitectura-y-stack-tecnologico)
   - 3.1 [Frontend & Framework](#frontend-framework)
   - 3.2 [Backend & Servicios en la Nube](#backend-servicios-en-la-nube)
   - 3.3 [APIs y Servicios Externos](#apis-y-servicios-externos)
   - 3.4 [Herramientas de Desarrollo](#herramientas-de-desarrollo)
4. [📱 Funcionalidades Principales](#funcionalidades-principales)
   - 4.1 [🔐 Gestión de Usuarios Avanzada](#gestion-de-usuarios-avanzada)
   - 4.2 [🗺️ Navegación y Mapas Inteligentes](#navegacion-y-mapas-inteligentes)
   - 4.3 [📅 Planificación de Viajes Profesional](#planificacion-de-viajes-profesional)
   - 4.4 [⭐ Sistema de Favoritos y Recomendaciones](#sistema-de-favoritos-y-recomendaciones)
   - 4.5 [🌤️ Información Contextual](#informacion-contextual)
5. [🛠️ Implementación y Configuración](#implementacion-y-configuracion)
   - 5.1 [Prerrequisitos del Sistema](#prerrequisitos-del-sistema)
   - 5.2 [Configuración del Proyecto](#configuracion-del-proyecto)
   - 5.3 [Comandos de Desarrollo](#comandos-de-desarrollo)
6. [🔧 Arquitectura del Sistema](#arquitectura-del-sistema)
   - 6.1 [Patrón BLoC (Business Logic Component)](#patron-bloc-business-logic-component)
   - 6.2 [Flujo de Datos](#flujo-de-datos)
7. [⚙️ Reglas de Negocio y Validaciones](#reglas-de-negocio-y-validaciones)
   - 7.1 [Seguridad y Autenticación](#seguridad-y-autenticacion)
   - 7.2 [Limitaciones Funcionales](#limitaciones-funcionales)
   - 7.3 [Estándares de Calidad](#estandares-de-calidad)
8. [📊 Resultados de Testing y Calidad](#resultados-de-testing-y-calidad)
   - 8.1 [Testing Automatizado por Módulos](#testing-automatizado-por-modulos)
   - 8.2 [Evaluación de Usabilidad Profesional](#evaluacion-de-usabilidad-profesional)
9. [🚀 Roadmap de Evolución](#roadmap-de-evolucion)
   - 9.1 [Fase 1: Optimización](#fase-1-optimizacion)
   - 9.2 [Fase 2: Expansión](#fase-2-expansion)
   - 9.3 [Fase 3: Inteligencia](#fase-3-inteligencia)
10. [📈 Métricas de Rendimiento](#metricas-de-rendimiento)
    - 10.1 [Benchmarks Técnicos](#benchmarks-tecnicos)
    - 10.2 [KPIs de Negocio](#kpis-de-negocio)
11. [🏫 Contexto Académico](#contexto-academico)
    - 11.1 [Equipo de Desarrollo](#equipo-de-desarrollo)
12. [📄 Documentación Técnica](#documentacion-tecnica)
13. [👨‍💻 Información del Autor](#informacion-del-autor)

<h2 id="vision-del-proyecto">1. 🎯 Visión del Proyecto</h2>

Fomentar el turismo mediante una plataforma móvil que proporcione información relevante, recomendaciones contextuales y herramientas de planificación avanzadas. El objetivo es crear una experiencia de viaje intuitiva que integre geolocalización, recomendaciones personalizadas y navegación optimizada según el medio de transporte.

<h2 id="metodologia-de-desarrollo">2. 📋 Metodología de Desarrollo</h2>

<h3 id="scrum-framework">2.1 SCRUM Framework</h3>

El proyecto fue desarrollado utilizando **metodología SCRUM** con 8 sprints estructurados que abarcaron desde la conceptualización hasta la implementación completa.

<h3 id="sprint-planning-overview">2.2 Sprint Planning Overview</h3>

- **Sprint 1** (20-22 Sep 2023): Definición de alcance, requerimientos y reglas de negocio
- **Sprint 2** (22-29 Sep 2023): Desarrollo de prototipos no funcionales y diseño de interfaces
- **Sprint 3** (09-13 Oct 2023): Refinamiento de interfaces y casos de uso suplementarios
- **Sprint 4** (16-20 Oct 2023): Implementación de casos de uso fundamentales
- **Sprint 5** (23 Oct-03 Nov 2023): Configuración de entornos, Firebase y definición del MVP
- **Sprint 6** (06-28 Nov 2023): Desarrollo del frontend e integración de APIs
- **Sprint 7** (29 Nov-12 Dic 2023): Implementación del backend y testing integral
- **Sprint 8** (13-19 Dic 2023): Integración final, pruebas y optimización

<h3 id="equipo-scrum-los-maquiavelicos">2.3 Equipo SCRUM "Los Maquiavélicos"</h3>

Equipo multidisciplinario de 11 desarrolladores con roles especializados en frontend, backend, documentación técnica, testing y arquitectura de sistemas.

<h2 id="arquitectura-y-stack-tecnologico">3. 🏗️ Arquitectura y Stack Tecnológico</h2>

<h3 id="frontend-framework">3.1 Frontend & Framework</h3>

- **Flutter** (SDK >=3.0.0) - Desarrollo multiplataforma nativo
- **Dart** - Lenguaje de programación principal
- **BLoC Pattern** - Arquitectura de gestión de estado reactiva
- **Auto Route** - Sistema de navegación declarativa

<h3 id="backend-servicios-en-la-nube">3.2 Backend & Servicios en la Nube</h3>

- **Firebase Core** - Plataforma backend como servicio
- **Firebase Authentication** - Autenticación segura multiproveedor
- **Cloud Firestore** - Base de datos NoSQL en tiempo real
- **Firebase Dynamic Links** - Enlaces dinámicos para compartir

<h3 id="apis-y-servicios-externos">3.3 APIs y Servicios Externos</h3>

- **Google Maps Flutter** - Mapas interactivos y navegación
- **Google Places API** - Búsqueda y información de lugares
- **Google Maps Webservice** - Servicios de geocodificación y rutas
- **Weather API** - Información meteorológica contextual

<h3 id="herramientas-de-desarrollo">3.4 Herramientas de Desarrollo</h3>

- **Freezed** - Generación de código inmutable
- **JSON Serializable** - Serialización automática de datos
- **Build Runner** - Generación de código automatizada
- **Flutter Lints** - Análisis estático de código

<h2 id="funcionalidades-principales">4. 📱 Funcionalidades Principales</h2>

<h3 id="gestion-de-usuarios-avanzada">4.1 🔐 Gestión de Usuarios Avanzada</h3>

- Autenticación Firebase con validación robusta
- Sistema multiusuario con cambio de cuentas dinámico
- Recuperación de contraseñas con preguntas de seguridad
- Perfiles personalizables con preferencias de viaje

<h3 id="navegacion-y-mapas-inteligentes">4.2 🗺️ Navegación y Mapas Inteligentes</h3>

- Geolocalización en tiempo real con GPS de alta precisión
- Rutas optimizadas para múltiples medios de transporte:
  - **A pie** - Rutas peatonales optimizadas
  - **Bicicleta** - Ciclovías y rutas ciclistas
  - **Automóvil** - Navegación vehicular con tráfico
  - **Transporte público** - Integración con sistemas urbanos
- Búsqueda contextual con autocompletado inteligente

<h3 id="planificacion-de-viajes-profesional">4.3 📅 Planificación de Viajes Profesional</h3>

- Creación de itinerarios de hasta 7 días
- Algoritmo de recomendaciones basado en:
  - Preferencias del usuario
  - Historial de visitas
  - Proximidad geográfica
  - Calificaciones comunitarias
- Gestión completa de planes: crear, editar, duplicar, eliminar

<h3 id="sistema-de-favoritos-y-recomendaciones">4.4 ⭐ Sistema de Favoritos y Recomendaciones</h3>

- Gestión inteligente de lugares favoritos
- Recomendaciones personalizadas por categorías
- Integración con Google Places para información actualizada
- Compartir ubicaciones mediante enlaces dinámicos

<h3 id="informacion-contextual">4.5 🌤️ Información Contextual</h3>

- Datos meteorológicos en tiempo real
- Notificaciones climáticas por ubicación
- Información de horarios y disponibilidad de establecimientos
- Catálogo extenso por categorías (restaurantes, museos, hoteles, etc.)

<h2 id="implementacion-y-configuracion">5. 🛠️ Implementación y Configuración</h2>

<h3 id="prerrequisitos-del-sistema">5.1 Prerrequisitos del Sistema</h3>

```bash
Flutter SDK >=3.0.0
Dart >=3.0.0
Android Studio / VS Code
Git para control de versiones
```

<h3 id="configuracion-del-proyecto">5.2 Configuración del Proyecto</h3>

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

<h3 id="comandos-de-desarrollo">5.3 Comandos de Desarrollo</h3>

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

<h2 id="arquitectura-del-sistema">6. 🔧 Arquitectura del Sistema</h2>

<h3 id="patron-bloc-business-logic-component">6.1 Patrón BLoC (Business Logic Component)</h3>

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

<h3 id="flujo-de-datos">6.2 Flujo de Datos</h3>

1. **UI Layer** - Interfaces Flutter con widgets reactivos
2. **BLoC Layer** - Lógica de negocio y gestión de estados
3. **Repository Layer** - Abstracción de fuentes de datos
4. **Data Layer** - APIs, Firebase y almacenamiento local

<h2 id="reglas-de-negocio-y-validaciones">7. ⚙️ Reglas de Negocio y Validaciones</h2>

<h3 id="seguridad-y-autenticacion">7.1 Seguridad y Autenticación</h3>

- Contraseñas: mínimo 8 caracteres con mayúscula, minúscula, número y carácter especial
- Validación de correos electrónicos únicos por cuenta
- Preguntas de seguridad obligatorias para recuperación
- Sesiones seguras con tokens JWT de Firebase

<h3 id="limitaciones-funcionales">7.2 Limitaciones Funcionales</h3>

- Máximo 7 días por itinerario de viaje
- Máximo 8 lugares por día en planes de viaje
- Restricción de rutas simultáneas (una activa por usuario)
- Geolocalización requerida para funcionalidades principales

<h3 id="estandares-de-calidad">7.3 Estándares de Calidad</h3>

- Cumplimiento WCAG 2.1 para accesibilidad
- Protección de datos personales (GDPR compliance)
- Optimización para dispositivos con ≥4GB RAM
- Aplicación <1GB de almacenamiento

<h2 id="resultados-de-testing-y-calidad">8. 📊 Resultados de Testing y Calidad</h2>

<h3 id="testing-automatizado-por-modulos">8.1 Testing Automatizado por Módulos</h3>

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

<h3 id="evaluacion-de-usabilidad-profesional">8.2 Evaluación de Usabilidad Profesional</h3>

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

<h2 id="roadmap-de-evolucion">9. 🚀 Roadmap de Evolución</h2>

<h3 id="fase-1-optimizacion">9.1 Fase 1: Optimización</h3>

- [ ] Implementación de Crashlytics para telemetría
- [ ] Modo offline con caché inteligente de mapas
- [ ] Notificaciones push contextuales
- [ ] Métricas de uso y analytics avanzados

<h3 id="fase-2-expansion">9.2 Fase 2: Expansión</h3>

- [ ] Integración con wearables (Apple Watch, Wear OS)
- [ ] Realidad aumentada para navegación
- [ ] Compartir ubicación en tiempo real
- [ ] API pública para desarrolladores

<h3 id="fase-3-inteligencia">9.3 Fase 3: Inteligencia</h3>

- [ ] Machine Learning para recomendaciones
- [ ] Análisis predictivo de patrones de viaje
- [ ] Asistente virtual por voz
- [ ] Integración con IoT y ciudades inteligentes

<h2 id="metricas-de-rendimiento">10. 📈 Métricas de Rendimiento</h2>

<h3 id="benchmarks-tecnicos">10.1 Benchmarks Técnicos</h3>

- **Tiempo de inicio**: <3 segundos en dispositivos objetivo
- **Consumo de batería**: Optimizado para 8+ horas de uso continuo
- **Uso de memoria**: <512MB RAM promedio
- **Tamaño de aplicación**: <150MB instalación completa

<h3 id="kpis-de-negocio">10.2 KPIs de Negocio</h3>

- **Retención de usuarios**: Meta 70% a 30 días
- **Engagement**: Sesiones promedio >10 minutos
- **Conversión**: 85% de usuarios completan primer itinerario
- **Satisfacción**: Score NPS objetivo >50

<h2 id="contexto-academico">11. 🏫 Contexto Académico</h2>

**Institución:** Instituto Politécnico Nacional - Escuela Superior de Cómputo  
**Carrera:** Ingeniería en Sistemas Computacionales  
**Materia:** Análisis y diseño de sistemas  
**Profesora:** Maldonado Castillo Idalia  
**Grupo:** 5CM2  
**Periodo:** Agosto - Diciembre 2023

<h3 id="equipo-de-desarrollo">11.1 Equipo de Desarrollo</h3>

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

<h2 id="documentacion-tecnica">12. 📄 Documentación Técnica</h2>

- **[Documentación Completa del Proyecto](./Documentacion.pdf)** - 200+ páginas con análisis completo, metodología SCRUM, casos de uso detallados, arquitectura del sistema, testing integral y evaluaciones de desempeño
- **[Presentación Ejecutiva](./Traknav-comprimido.pdf)** - Resumen ejecutivo para consulta rápida

<h2 id="informacion-del-autor">13. 👨‍💻 Información del Autor</h2>

**Cesar Osvaldo Zamudio Onofre**  
[@Czamudioo121](https://github.com/Czamudioo121)

📍 **Ubicación:** Ciudad de México, México  
🎓 **Rol en el proyecto:** Development Team Member & Documentation Lead & Designer UI/UX  
📧 **Contacto:** [GitHub Profile](https://github.com/Czamudioo121)

---

### 🌟 TrakNav representa la convergencia entre tecnología moderna, metodologías ágiles y experiencia de usuario excepcional

*Desarrollado con metodología SCRUM y tecnologías de vanguardia por el equipo "Los Maquiavélicos"*

**Stack Principal:** Flutter • Firebase • Google Maps • SCRUM • BLoC Pattern