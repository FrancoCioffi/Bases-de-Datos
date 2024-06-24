# Trabajo Práctico Nro 6: Instalación de Sistemas Operativos y Administradores de Archivos
1.- Investigue la instalación de sistemas operativos en Modo UEFI teniendo en cuenta todos los pasos del proceso. Desde la preparación del medio hasta el manejo de las claves de seguridad (Secure Boot)
```
    Preparación del Medio de Instalación:
    Obtener la imagen ISO del sistema operativo que se quiere instalar, para luego crear el medio de instalacion utilizando     
    herramientos como Rufus, UNetbootin si se usara USB o grabar la imagen ISO en un DVD usando ImgBurn.
    Configuración de BIOS/UEFI:
    Prender la computadora y acceder a la configuracion de BIOS/UEFI (apretando F2,F10 DEL o ESC generalmente)
    Asegurate de que el modo de arranque esté configurado en UEFI.
    En algunos casos, quizas necesitemos desactivar el Secure Boot para permitir la instalación de ciertos sistemas operativos.
    Instalación del Sistema Operativo:
    Enchufar el USB o DVD y seleccionarlo como arranque, luego seguimos las instrucciones del instalador del S.O. Si fuera Windows 
    seleccionariamos "Custom Install" para crear particiones. 
    Crear una partición para el sistema EFI y formatear en FAT32.
    Configuración de Particiones:
    Crea las particiones necesarias para el sistema operativo y otros datos, después de la instalación del sistema operativo,     
    puedes volver a habilitar Secure Boot si lo habías desactivado.
``` 
2.- Investigue los requisitos de instalación mínimos y recomendados para la instalación de sistemas operativos actuales en sus 
últimas versiones. Investigue también las versiones corporativas tipo Windows Server Editions. Investigue las capacidades máximas 
de administración tanto de memoria, disco y procesador de cada uno. Investigue los costos de las licencias.
```
    # Windows 11:
    Mínimos:
    Procesador: 1 GHz o superior
    RAM: 4 GB (64 bits)
    Almacenamiento: 64 GB
    Tarjeta gráfica: DirectX 12 o superior con controlador WDDM 2.0
    Pantalla: 800x600 (mínimo) o 1366x768 (recomendado)
    Firmware: UEFI y Arranque seguro
    TPM 2.0

    Recomendados:
    Procesador: 2 GHz o superior
    RAM: 8 GB
    Almacenamiento: 128 GB
    Tarjeta gráfica: DirectX 12 o superior con controlador WDDM 2.1
    Pantalla: 1920x1080 o superior

    # macOS Monterey:
    Computadora Mac compatible
    macOS 10.12 o superior
    4 GB de RAM
    1 GB de espacio disponible en disco

    # Ubuntu 22.04 LTS:
    Procesador: 2 GHz o superior de 64 bits
    RAM: 4 GB
    Almacenamiento: 25 GB
    Tarjeta gráfica: compatible con OpenGL 3.0 o superior

    # Windows Server 2022:
    Mínimos:
    Procesador: Server Xeon E5-2630 v4 a 2.0 GHz o equivalente
    RAM: 32 GB
    Almacenamiento: 128 GB
    Tarjeta de red: Gigabit Ethernet

    Recomendados: 
    Procesador: Server Xeon Platinum 8328 a 2.1 GHz o equivalente
    RAM: 64 GB
    Almacenamiento: 512 GB
    Tarjeta de red: 10 GbE

    # Capacidades máximas:
    Windows 11:
    Memoria: 64 TB (para ediciones Workstation y Pro)
    Almacenamiento: 8 PB
    Procesadores: sin límite oficial (depende de la arquitectura)

    macOS Monterey:
    Memoria: 64 GB
    Almacenamiento: 8 TB
    Procesadores: sin límite oficial (depende del modelo de Mac)

    Ubuntu 22.04 LTS:
    Memoria: sin límite oficial (depende de la arquitectura)
    Almacenamiento: sin límite oficial
    Procesadores: sin límite oficial (depende de la arquitectura)

    Windows Server 2022:
    Memoria: 8 TB (para ediciones Datacenter y Standard)
    Almacenamiento: Petabytes (depende de la configuración)
    Procesadores: 2 sockets físicos con hasta 80 núcleos físicos y 160 subprocesos lógicos por socket

    #Costos de licencias:
    Windows 11:
    Home: $139 USD
    Pro: $199 USD

    macOS Monterey:
    Gratis con la compra de una Mac compatible

    Ubuntu 22.04 LTS:
    Gratis

    Windows Server 2022:
    Datacenter: 6155 USD
    Estandar: 1069 USD
    Essentials: 501 USD
    
``` 
3.- Investigue las funciones del módulo TPM.
```     
    El Módulo de Plataforma Segura (TPM) es un chip integrado en la placa base de algunos ordenadores que proporciona un 
    conjunto de funciones de seguridad para proteger los datos y el sistema.
    Las principales funciones del TPM son:
    Almacenamiento seguro de claves:
    El TPM puede almacenar claves criptográficas de forma segura, como contraseñas, certificados y claves de cifrado. Estas            claves se almacenan en un enclave seguro dentro del TPM, lo que las protege del acceso no autorizado, incluso si el sistema        operativo está infectado con malware.
    Arranque seguro:
    El TPM puede ayudar a garantizar que el sistema operativo se inicie de forma segura y que no se manipule antes de cargarse.        Esto ayuda a proteger el sistema de ataques de firmware y rootkits.
    Cifrado de disco completo:
    El TPM puede utilizarse para cifrar el disco duro de un ordenador, lo que protege los datos en caso de robo o pérdida del     
    ordenador.
    Autenticación segura:
    El TPM puede utilizarse para autenticar a los usuarios y los dispositivos, lo que ayuda a proteger el acceso a los datos y     
    recursos sensibles.
    Protección contra malware:
    El TPM puede utilizarse para proteger el sistema contra malware, ya que puede detectar y bloquear intentos de manipular            el sistema operativo o el firmware.
``` 
4.- Investigue los utilitarios que permiten cambiar el tamaño de las particiones. Por lo menos nombre a tres.
``` 
    AOMEI Partition Assistant:
    Es una herramienta gratuita y de pago con una interfaz fácil de usar y funciones avanzadas como la migración de sistemas           operativos, la recuperación de particiones y la creación de particiones virtuales. Soporta una amplia gama de sistemas de          archivos y dispositivos de almacenamiento.
    
    EaseUS Partition Master:
    Otra opción popular con versiones gratuitas y de pago. Ofrece funciones similares a AOMEI Partition Assistant, incluyendo la       redimensión, la creación, la eliminación y la conversión de particiones. También es compatible con una amplia gama de sistemas     de archivos y dispositivos de almacenamiento.

    GParted:
    Un potente editor de particiones de código abierto y gratuito para sistemas operativos basados en Linux. Ofrece funciones          avanzadas como la creación y eliminación de particiones, el formateo, la copia y el pegado de particiones, y la comprobación y     reparación de errores de disco. Sin embargo, su interfaz puede ser menos intuitiva para usuarios principiantes.
``` 
5.- Investigue gestores de arranque para elegir Sistemas Operativos múltiples en un equipo. Que trabajen en modo MBR o UEFI o ambos. Haga una comparativa.
```
    1. GRUB (GRand Unified Bootloader):
    Compatibilidad: MBR, UEFI
    Características: Potente, personalizable, compatible con una amplia gama de sistemas operativos, gestor de arranque por 
    defecto en muchas distribuciones de Linux.
    Ventajas: Altamente configurable, opciones avanzadas para la gestión de particiones, soporte para múltiples idiomas.
    Desventajas: Curva de aprendizaje más pronunciada para usuarios principiantes, puede ser complejo para configuraciones no     
    estándar.

    2. rEFInd (reborn EFI bootloader):
    Compatibilidad: MBR, UEFI (recomendado)
    Características: Interfaz gráfica intuitiva, fácil de usar, compatible con una amplia gama de sistemas operativos, menú de 
    arranque personalizable.
    Ventajas: Interfaz amigable, ideal para usuarios principiantes, menú de arranque personalizable con temas e íconos.
    Desventajas: Menos opciones avanzadas de configuración en comparación con GRUB, puede no ser compatible con sistemas 
    operativos antiguos o poco comunes.

    3. EasyUEFI:
    Compatibilidad: MBR, UEFI
    Características: Interfaz gráfica fácil de usar, clonación de discos, gestión de particiones, opciones de arranque avanzadas.
    Ventajas: Interfaz intuitiva, ideal para usuarios principiantes, herramientas integradas para la gestión de discos y 
    particiones.
    Desventajas: Menos personalizable que otros gestores de arranque, funciones avanzadas pueden requerir la versión de pago.
    | Gestor de arranque | Compatibilidad | Caracteristicas                 | Ventajas                                    |        Desventajas       |
    |--------------------|----------------|---------------------------------|---------------------------------------------|--------------------------|
    | GRUB               | MBR, UEFI      | Potente, personalizable         | Amplia compatibilidad, opciones avanzadas   | Curva de aprendizaje     |
    | rEFInd             | MBR, UEFI      | Interfaz grafica intuitiva      | Facil de usar, menu personalizable          | Menos opciones avanzadas |
    | EasyUEFI           | MBR, UEFI      | Interfaz grafica facil  de usar | Intefaz  intuitiva, herramientas integradas | Menos personizable       |
``` 
6.- Haga una lista comparativa de al menos 10 administradores de archivos. Pueden ser de diferentes plataformas. Compare 
funcionalidades y capacidades de expansión. Clasifíquelos luego por categoría con una descripción de cada una.
```
    1. Explorador de archivos de Windows (Windows):
    Funcionalidades: Administración básica de archivos, búsqueda integrada, integración con OneDrive.
    Capacidades de expansión: Extensiones limitadas, personalización básica.

    2. Finder (macOS):    
    Funcionalidades: Administración avanzada de archivos, búsqueda Spotlight, integración con iCloud.
    Capacidades de expansión: Scripts de Automator, personalización avanzada.

    3. Nautilus (Linux):    
    Funcionalidades: Administración completa de archivos, integraciones con servicios en la nube, personalización avanzada.
    Capacidades de expansión: Extensiones, plugins, temas.

    4. FreeCommander (Windows):    
    Funcionalidades: Paneles duales, administración avanzada de archivos, soporte para FTP/WebDAV.
    Capacidades de expansión: Plugins, scripts, temas.

    5. XYplorer (Windows):    
    Funcionalidades: Paneles con pestañas, búsqueda avanzada, potentes opciones de filtrado.
    Capacidades de expansión: Plugins, scripts, temas.
    Plataforma: Windows.

    6. Directory Opus (Windows):
    Funcionalidades: Altamente personalizable, automatización de tareas, soporte para FTP/WebDAV.
    Capacidades de expansión: Plugins, scripts, temas.

    7. Total Commander (Windows):    
    Funcionalidades: Paneles duales, administración avanzada de archivos, soporte para FTP/WebDAV.
    Capacidades de expansión: Plugins, scripts, temas.

    8. Commander One (macOS, Windows):    
    Funcionalidades: Paneles duales, administración avanzada de archivos, soporte para FTP/WebDAV.
    Capacidades de expansión: Plugins, scripts, temas.

    9. DCommander (Linux):    
    Funcionalidades: Interfaz similar a Norton Commander, administración avanzada de archivos, soporte para FTP/WebDAV.
    Capacidades de expansión: Plugins, scripts, temas.

    10. Krusader (Linux, macOS, Windows):
    Funcionalidades: Paneles cuádruples, administración avanzada de archivos, soporte para FTP/WebDAV.
    Capacidades de expansión: Plugins, scripts, temas.

    Categorías:
    1. Administradores de archivos básicos:
    Explorador de archivos de Windows (Windows)
    Finder (macOS)
    Nautilus (Linux)

    2. Administradores de archivos con paneles duales:    
    FreeCommander (Windows)
    Total Commander (Windows)
    Commander One (macOS, Windows)
    DCommander (Linux)
    Krusader (Linux, macOS, Windows)

    3. Administradores de archivos con funciones avanzadas:
    XYplorer (Windows)
    Directory Opus (Windows)
``` 
