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

4.- Investigue los utilitarios que permiten cambiar el tamaño de las particiones. Por lo menos nombre a tres.

5.- Investigue gestores de arranque para elegir Sistemas Operativos múltiples en un equipo. Que trabajen en modo MBR o UEFI o ambos. # Haga una comparativa.

6.- Haga una lista comparativa de al menos 10 administradores de archivos. Pueden ser de diferentes plataformas. Compare 
funcionalidades y capacidades de expansión. Clasifíquelos luego por categoría con una descripción de cada una.
