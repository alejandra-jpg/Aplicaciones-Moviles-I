📚 StudyPlan

Aplicación móvil nativa para Android desarrollada en Kotlin con Jetpack Compose, diseñada para organizar, gestionar y recibir recordatorios de planes de estudio.

✨ Características principales

Gestión de planes de estudio: Organización estructurada de tareas, materias o sesiones de estudio mediante arquitectura reactiva (StudyViewModel).

Interfaz moderna: Pantallas construidas de forma declarativa en Kotlin (Screens.kt) con tema personalizado (Theme.kt).

Sistema de notificaciones: Recordatorios locales programados para el seguimiento de actividades (Notifier.kt).

Gestión de datos: Modelo de datos limpio y desacoplado (Data.kt).

🛠️ Tecnologías utilizadas

Lenguaje: Kotlin

Interfaz de usuario: Jetpack Compose / Material Design

Arquitectura: MVVM (ViewModel + Estado reactivo)

Sistema de compilación: Gradle con Kotlin DSL (build.gradle.kts, settings.gradle.kts)

Notificaciones: Android Notification Manager (Notifier.kt)

📂 Estructura del proyecto

StudyPlan/
├── app/
│   ├── build.gradle.kts                  # Configuración de dependencias y SDK del módulo app
│   └── src/
│       └── main/
│           ├── AndroidManifest.xml       # Permisos, componentes y configuración de la app
│           ├── java/com/studyplan/app/
│           │   ├── Data.kt               # Modelos y estructuras de datos
│           │   ├── MainActivity.kt       # Punto de entrada principal de la aplicación
│           │   ├── Notifier.kt           # Lógica de creación y envío de notificaciones
│           │   ├── Screens.kt            # Pantallas y componentes de interfaz (UI)
│           │   ├── StudyViewModel.kt     # Lógica de negocio y gestión de estado
│           │   └── Theme.kt              # Paleta de colores, tipografía y estilos
│           └── res/
│               ├── drawable/             # Íconos de lanzador y notificaciones
│               └── values/               # Cadenas de texto (strings.xml) y temas (themes.xml)
├── gradle/                               # Gradle Wrapper
├── build.gradle.kts                      # Configuración global de Gradle
├── settings.gradle.kts                   # Configuración de módulos del proyecto
└── gradlew / gradlew.bat                 # Scripts de ejecución de Gradle


🚀 Requisitos previos

Android Studio (recomendado Iguana / Jellyfish / Ladybug o superior).

JDK 17 o superior configurado en Android Studio.

Dispositivo físico o emulador Android con soporte para notificaciones.

⚙️ Instalación y ejecución

Clona este repositorio:

git clone https://github.com/tu-usuario/StudyPlan.git


Abre el proyecto en Android Studio:

Selecciona File > Open y elige la carpeta raíz StudyPlan/.

Espera a que Gradle sincronice y descargue las dependencias automáticamente.

Ejecuta la aplicación:

Conecta un dispositivo Android (con Depuración USB habilitada) o inicia un emulador.

Haz clic en el botón Run (Shift + F10) o ejecuta desde la terminal:

./gradlew assembleDebug


🔔 Permisos

La aplicación utiliza permisos de notificaciones de Android (como POST_NOTIFICATIONS en Android 13+) para alertar al usuario sobre sus sesiones de estudio programadas. Asegúrate de conceder el permiso al iniciar la aplicación por primera vez.

