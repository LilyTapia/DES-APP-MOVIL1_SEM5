# VeterinariaApp 🐾

Aplicación Android desarrollada en **Kotlin** utilizando **Jetpack Compose**, diseñada para la gestión de consultas veterinarias. Este proyecto forma parte de la evaluación de la **Semana 5 (Integrando Kotlin en Android Studio)** para la asignatura de Desarrollo de Apps Móviles I en DUOC.

El proyecto destaca por su arquitectura **modular**, separando claramente la lógica de negocio, la interfaz de usuario y las utilidades.

## 📱 Características

*   **Pantalla de Bienvenida Dinámica**: Muestra un resumen en tiempo real de:
    *   Total de mascotas registradas.
    *   Total de consultas realizadas.
    *   Nombre del último dueño registrado.
*   **Registro de Consultas**: Flujo paso a paso para registrar:
    *   Datos del Dueño.
    *   Datos de la Mascota.
    *   Tipo de Servicio (Control, Vacuna, Urgencia, Otro).
*   **Resumen de Atención**: Confirmación de los datos ingresados antes de finalizar.
*   **Interfaz Moderna**: Implementada 100% con Jetpack Compose y Material Design 3.

## 🛠 Tecnología y Arquitectura

El proyecto sigue una arquitectura modular y utiliza las últimas tecnologías recomendadas por Google:

*   **Lenguaje**: [Kotlin](https://kotlinlang.org/)
*   **UI Toolkit**: [Jetpack Compose](https://developer.android.com/jetpack/compose)
*   **Gestión de Estado**: `ViewModel` y `LiveData` / `State`.
*   **Concurrencia**: `Kotlin Coroutines`.
*   **Build System**: Gradle Kotlin DSL (`.kts`) con Version Catalog (`libs.versions.toml`).

### 📦 Estructura de Módulos

El proyecto está organizado en 4 módulos para asegurar la escalabilidad y mantenibilidad:

1.  **:app**: Módulo principal que actúa como punto de entrada (`MainActivity`). Orquesta la navegación y las dependencias.
2.  **:ui**: Contiene toda la interfaz de usuario (Screens, Components, Theme, Navigation y ViewModels).
3.  **:data**: Contiene la lógica de negocio, modelos de datos (`Mascota`, `Consulta`, `Dueno`) y repositorios (`VeterinariaRepository`).
4.  **:util**: Funciones de utilidad y extensiones transversales (`InputUtils`, etc.).

## 🚀 Instalación y Ejecución

1.  Clonar el repositorio:
    ```bash
    git clone https://github.com/LilyTapia/DES-APP-MOVIL1_SEM5.git
    ```
2.  Abrir en **Android Studio** (Ladybug o superior recomendado).
3.  Esperar a que finalice la sincronización de Gradle.
4.  Seleccionar el módulo `app` y ejecutar en un emulador o dispositivo físico (Min SDK 24).

---
**Desarrollado por:** Liliana Tapia
**Asignatura:** Desarrollo de Apps Móviles I - DUOC UC
