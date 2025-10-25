# Clínica Dental Dra. Yocaina Pérez – Aplicación Móvil Android

## Descripción del Proyecto
La aplicación móvil **Clínica Dental Dra. Yocaina Pérez** tiene como propósito complementar la plataforma web desarrollada en **ASP.NET Core MVC**, permitiendo que pacientes, doctores y personal administrativo gestionen citas, historiales médicos, tratamientos y pagos desde sus dispositivos Android.

El objetivo principal es ofrecer una experiencia **moderna, segura y accesible**, fortaleciendo la comunicación entre la clínica y sus pacientes mediante notificaciones en tiempo real y acceso inmediato a los servicios odontológicos.

---

## Exposición del Problema
Aunque la clínica cuenta con un sistema web funcional, muchos usuarios dependen del acceso mediante navegadores, lo que limita la portabilidad y la interacción rápida.  
El **problema identificado** es la falta de comunicación inmediata y acceso en movilidad.  
Con esta aplicación nativa se busca:
- Facilitar la gestión de citas y recordatorios desde el teléfono.  
- Permitir al personal clínico acceder a los historiales en tiempo real.  
- Optimizar la experiencia del paciente mediante notificaciones y una interfaz amigable.

---

## Plataforma y Tecnologías
El desarrollo se realizará en **Android Studio (versión 2025.x)** utilizando **Kotlin** y el patrón de arquitectura **MVVM**.

**Herramientas y frameworks principales:**
- **Retrofit** → Consumo de API REST del sistema web.  
- **Firebase Authentication** → Inicio de sesión seguro y gestión de usuarios.  
- **Room Database** → Almacenamiento local y sincronización offline.  
- **Material Design 3 / Jetpack Compose** → Interfaz de usuario moderna.  
- **GitHub Actions** → Integración continua (CI/CD).  

**Base de datos:** conexión remota a **SQL Server** mediante API ASP.NET.  
**Control de versiones:** GitHub Classroom (repositorio oficial del curso).

---

## Interfaz de Usuario y Administrador

### Interfaz del Usuario (Paciente)
- Registro e inicio de sesión.  
- Consulta y reserva de citas.  
- Visualización de historial médico.  
- Notificaciones push sobre recordatorios y pagos.  
- Chat interno con la clínica.

### Interfaz del Administrador (Doctor / Recepcionista)
- Panel diario de citas.  
- Registro y actualización de tratamientos.  
- Control de pagos y facturación.  
- Acceso al historial médico del paciente.  
- Reprogramación de citas y seguimiento clínico.

---

## Funcionalidades Principales
- Inicio de sesión autenticado (Firebase).  
- Gestión de citas sincronizada con la base de datos web.  
- Consulta de tratamientos, pagos y diagnósticos.  
- Notificaciones automáticas (Firebase Cloud Messaging).  
- Soporte offline con sincronización automática.  
- Reportes simples de citas y tratamientos.  
- Interfaz adaptable a distintos tamaños de pantalla.

---

## Diseño (Wireframes / Esquemas de Página)
Los primeros bocetos del diseño se desarrollarán en **Figma**, siguiendo los principios de **Material You**.  
A continuación, la estructura base de navegación:

1. **Pantalla de Inicio de Sesión**  
   - Campos de usuario, contraseña y botón de acceso.  

2. **Menú Principal (Bottom Navigation):**  
   - Citas | Historial | Pagos | Perfil  

3. **Pantalla de Citas:**  
   - Lista de citas con opciones para agregar, cancelar o reprogramar.  

4. **Pantalla de Historial:**  
   - Información de tratamientos, fechas y observaciones del doctor.  

5. **Panel Administrativo:**  
   - Vista de calendario, registro de tratamientos y control de pagos.

*(Los wireframes se incluirán posteriormente en la carpeta `/design` del repositorio).*

---

## Estructura del Repositorio

ClinicaDentalApp-Mobile/
│
├── app/                  # Código fuente en Kotlin
├── design/               # Wireframes y mockups (Figma / imágenes)
├── docs/                 # Documentación técnica y manual de usuario
├── api/                  # Configuración de conexión con la API ASP.NET
├── build.gradle          # Configuración del proyecto
├── README.md             # Borrador del proyecto
└── LICENSE
