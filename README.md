# 🛡️ Cosme Firewall - Control de Red en Android

![Etiqueta de Estado](https://img.shields.io/badge/Estado-Beta%20Privada-yellow)
![Etiqueta de Licencia](https://img.shields.io/badge/Licencia-GPLv3-blue)
![Etiqueta de Plataforma](https://img.shields.io/badge/Plataforma-Android%205.0%2B-green)

## 🌟 Resumen del Proyecto

**Cosme Firewall** es una aplicación de código abierto para Android diseñada para dar a los usuarios **control granular** sobre el tráfico de red de sus aplicaciones. Utilizando la API de VPN local de Android (modo No-Root) o las capacidades de *iptables* (modo Root), Cosme permite **bloquear conexiones no deseadas**, **reducir el consumo de datos** y **mejorar la privacidad** del dispositivo.

**Relevancia en Ciberseguridad/Flutter:** Este proyecto demuestra mi conocimiento profundo de la **seguridad móvil en Android**, la gestión del tráfico a nivel de sistema, y mi habilidad para desarrollar interfaces de usuario robustas y funcionales usando **Flutter (para la UI)** y lógica de red nativa (para la función de firewall).

## ✨ Características Principales

* **Filtrado por Aplicación:** Bloquea el acceso a internet (Wi-Fi y/o datos móviles) por aplicación individual.
* **Modo No-Root (VPN Service):** Utiliza el servicio VPN local de Android para interceptar y filtrar el tráfico sin necesidad de acceso Root.
* **Monitoreo en Tiempo Real:** Interfaz clara (gracias a Flutter) para visualizar qué aplicaciones están intentando acceder a la red.
* **Bajo Consumo:** Optimizado para funcionar en segundo plano con un impacto mínimo en la batería.
* **Exportación de Reglas:** Permite guardar y cargar configuraciones de reglas de firewall.

## 💻 Tecnologías Utilizadas

* **Frontend (UI):** **Flutter** (Dart)
* **Backend (Lógica de Red):** Kotlin/Java para la implementación del `VpnService` de Android.
* **Base de Datos (Reglas):** SQLite (o Hive/Isar si usas Flutter solo)
* **Despliegue/Distribución:** Archivo **APK** (distribución vía GitHub Releases, F-Droid, o Google Play).

## 🛠️ Instalación y Uso

### 📥 Descarga la Aplicación (APK)

La última versión estable está disponible en la sección **[Releases]** de este repositorio:

* [Descargar Cosme-Firewall-v1.0.0.apk](https://www.mediafire.com/file/12af7ujb0hgpphq/Cosm3_Firewall_v2.apk/file) *(Reemplaza con el enlace real)*

**Pasos de Instalación:**

1.  Descarga el archivo `Cosme-Firewall.apk` en tu dispositivo Android.
2.  Asegúrate de tener habilitada la opción "Instalar aplicaciones de fuentes desconocidas".
3.  Instala el APK.
4.  Al abrir, **debes aceptar la solicitud de conexión VPN** para que el firewall sin Root pueda operar.

### ⚙️ Compilar desde el Código Fuente

Si quieres compilar la aplicación tú mismo:

1.  **Clonar el Repositorio:**
    ```bash
    git clone [https://github.com/tu_usuario/Cosme-Firewall.git](https://github.com/tu_usuario/Cosme-Firewall.git)
    cd Cosme-Firewall
    ```
2.  **Abrir con Android Studio/VS Code:** Abre la carpeta del proyecto.
3.  **Ejecutar Build:**
    ```bash
    # Si usas Flutter
    flutter build apk --release
    # O compila directamente desde Android Studio.
    ```
    El archivo APK se encontrará en `build/app/outputs/flutter-apk/app-release.apk`.

## 🗺️ Roadmap

* **Soporte a IPv6:** Extender el filtrado a paquetes IPv6.
* **Reglas Geográficas:** Opción de bloquear conexiones a países específicos.
* **Detección de Spyware:** Implementar listas negras actualizadas para bloquear servidores espía conocidos.
* **Interfaz de Monitorización Avanzada (Flutter):** Dashboard con gráficos de flujo de datos y alertas.

## 🤝 Contribuciones y Reporte de Bugs

Tu experiencia es valiosa. Si encuentras un error o quieres sugerir una mejora, por favor, abre un **[Issue]** o envía un **[Pull Request]**.

## 📄 Licencia

Este proyecto está bajo la Licencia **GPLv3**. Consulta el archivo [LICENSE](LICENSE) para más detalles.

---

**Siguiente paso:** Para que los reclutadores puedan descargar y probar tu APK, necesitas subirla a la sección **Releases** de tu repositorio. ¿Quieres que te muestre cómo se hace?
