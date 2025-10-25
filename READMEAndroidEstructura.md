# Estructura proyecto AndroidStudio

```
app
├── manifests
│   └── AndroidManifest.xml
```
<details>
  <summary>app.manifests.AndroidManifest</summary>
    Archivo fundamental que describe la app al sistema operativo Android: declara componentes, permisos y características.
</details>

```
│
├── kotlin+java
│   ├── com.example.androidappconfiguracion 
│   │   ├── LinearLayoutActivity.kt       - Archivo de código Kotlin para una de las pantallas (Activity) de la app.
│   │   └── MainActivity.kt               - Archivo de código Kotlin para la pantalla principal de la app.
│   │
│   ├── com.example.androidappconfiguracion (androidTest) 
│   │
│   └── com.example.androidappconfiguracion (test) 
```
<details>
  <summary>kotlin+java</summary>
    Paquete principal que contiene el código fuente de la aplicación. Nos encontramos las clases de los métodos que tiene Kotlin. 5 clases 5 controladores.
</details>

```
│
├── java (generated)
│   └── (archivos generados)
│
└── res                                   - Carpeta para todos los recursos que no son código: imágenes, diseños, textos, etc.
    ├── drawable                          - Recursos gráficos como imágenes (PNG, JPG), vectores y formas definidas en XML.
    │   ├── gato.jpg
    │   └──...
    │
    ├── layout                            - Archivos XML que definen la estructura de la interfaz de usuario (las pantallas y sus componentes).
    │   ├── activity_ejemplo.xml
    │   └──...
    │
    ├── mipmap                            - Específicamente para los iconos de la aplicación que se muestran en el lanzador del dispositivo, en diferentes densidades.[17, 27, 18, 19, 20, 21, 26]
    │   ├── ic_launcher
    │   └── ic_launcher_round
    │
    ├── values                            - Archivos XML que definen valores simples y constantes para reutilizar en la app.[17, 27, 18, 19, 20, 21, 26, 28]
    │   ├── colors.xml                    - Define la paleta de colores de la app.
    │   ├── strings.xml                   - Almacena todos los textos para facilitar la traducción y el mantenimiento.
    │   └── themes/                       - Definen la apariencia visual (temas y estilos) de la app y sus componentes.
    │
    └── xml                               - Para archivos de configuración XML arbitrarios (ej. preferencias de la app, reglas de seguridad de red).[29, 30]
        ├── backup_rules.xml
        └── data_extraction_rules.xml
```
<details>
  <summary>res</summary>
  Carpeta para todos los recursos que no son código: imágenes, diseños, textos, etc.
</details>

  - <details>
      <summary>res.drawable</summary>
      Recursos gráficos como imágenes (PNG, JPG), vectores y formas definidas en XML.
    </details>

  - <details>
      <summary>res.layout</summary>
      Archivos XML que definen la estructura de la interfaz de usuario o las vistas (las pantallas y sus componentes).
    </details>

  - <details>
      <summary>res.mipmap</summary>
      Específicamente para los iconos de la aplicación que se muestran en el lanzador del dispositivo, en diferentes densidades.
    </details>

  - <details>
      <summary>res.values</summary>
      Archivos XML que definen valores simples y constantes para reutilizar en la app.
      
    </details>

    - <details>
        <summary>res.values.colors.xml</summary>
        Archivos XML que definen valores simples y constantes para reutilizar en la app.
      </details>
  
    - <details>
        <summary>res.values.strings</summary>
        Archivos XML que definen valores simples y constantes para reutilizar en la app.
      </details>
      
    - <details>
        <summary>res.values.style</summary>
        Es donde se definen los estilos y temas de una aplicación de Android. Su propósito principal es separar el diseño y la apariencia de la estructura de la interfaz de usuario, de manera similar a como lo hacen las hojas de estilo (CSS) en el diseño web.
      </details>    

```

Gradle Scripts
├── build.gradle.kts (Project)            - Configuración de compilación para todo el proyecto (repositorios, versiones de plugins).[31, 32]
├── build.gradle.kts (Module: app)        - Configuración específica para el módulo 'app' (dependencias, versión de la app, SDK mínimo).[31, 32]
├── proguard-rules.pro                    - Reglas para ofuscar y reducir el tamaño del código en la versión final de la app.
├── gradle.properties                     - Propiedades globales para Gradle (ej. configuración de memoria para mejorar el rendimiento de la compilación).[32]
├── gradle-wrapper.properties             - Define qué versión de Gradle usar, asegurando que todos los desarrolladores usen la misma.[32]
├── libs.versions.toml                    - Catálogo centralizado para gestionar las versiones de las librerías y dependencias del proyecto.[33]
├── local.properties                      - Propiedades locales del desarrollador (como la ruta del SDK de Android). No se comparte en el control de versiones.[32]
└── settings.gradle.kts                   - Define los módulos (sub-proyectos) que se incluyen en el proyecto global.[32]
```

<details>
  <summary>build.gradle.kts (Module: app)</summary>
  Configuración específica para el módulo 'app' (dependencias, versión de la app, SDK mínimo).
</details>
