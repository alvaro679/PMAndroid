# Estructura proyecto AndroidStudio
- app
  <details>
    <summary>manifests.AndroidManifest</summary>
      Archivo fundamental que describe la app al sistema operativo Android: declara componentes, permisos y características.
  </details>
  <details>
    <summary>kotlin+java</summary>
      Paquete principal que contiene el código fuente de la aplicación. Nos encontramos las clases de los métodos que tiene Kotlin. 5 clases 5 controladores.
  </details>
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
          <summary>res.values.colors</summary>
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
<details>
  <summary>build.gradle.kts (Module: app)</summary>
  Configuración específica para el módulo 'app' (dependencias, versión de la app, SDK mínimo).
</details>

```
app
├── manifests
│   └── AndroidManifest.xml
│
├── kotlin+java
│   ├── com.example.androidappconfiguracion 
│   │   ├── LinearLayoutActivity.kt       - Archivo de código Kotlin para una de las pantallas (Activity) de la app.
│   │   └── MainActivity.kt               - Archivo de código Kotlin para la pantalla principal de la app.
│   │
│   ├── com.example.androidappconfiguracion (androidTest) 
│   │
│   └── com.example.androidappconfiguracion (test) 
│
├── java (generated)
│   └── (archivos generados)
│
└── res                                   
    ├── drawable                          
    │   ├── gato.jpg
    │   └──...
    │
    ├── layout                           
    │   ├── activity_ejemplo.xml
    │   └──...
    │
    ├── mipmap                            
    │   ├── ic_launcher
    │   └── ic_launcher_round
    │
    ├── values                            
    │   ├── colors.xml                    
    │   ├── strings.xml                   
    │   └── themes/                       
    │
    └── xml                               - Para archivos de configuración XML arbitrarios (ej. preferencias de la app, reglas de seguridad de red).
        ├── backup_rules.xml
        └── data_extraction_rules.xml

Gradle Scripts
├── build.gradle.kts (Project)            - Configuración de compilación para todo el proyecto (repositorios, versiones de plugins).
├── build.gradle.kts (Module: app)        - Configuración específica para el módulo 'app' (dependencias, versión de la app, SDK mínimo).
├── proguard-rules.pro                    - Reglas para ofuscar y reducir el tamaño del código en la versión final de la app.
├── gradle.properties                     - Propiedades globales para Gradle (ej. configuración de memoria para mejorar el rendimiento de la compilación).
├── gradle-wrapper.properties             - Define qué versión de Gradle usar, asegurando que todos los desarrolladores usen la misma.
├── libs.versions.toml                    - Catálogo centralizado para gestionar las versiones de las librerías y dependencias del proyecto.
├── local.properties                      - Propiedades locales del desarrollador (como la ruta del SDK de Android). No se comparte en el control de versiones.
└── settings.gradle.kts                   - Define los módulos (sub-proyectos) que se incluyen en el proyecto global.
```

