# Trabajo Práctico Nro 6: Instalación de Sistemas Operativos y Administradores de Archivos
1.- Investigue la instalación de sistemas operativos en Modo UEFI teniendo en cuenta todos los pasos del proceso. Desde la preparación del medio hasta el manejo de las claves de seguridad (Secure Boot)
  """
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
  """
2.- Investigue los requisitos de instalación mínimos y recomendados para la instalación de sistemas operativos actuales en sus 
últimas versiones. Investigue también las versiones corporativas tipo Windows Server Editions. Investigue las capacidades máximas 
de administración tanto de memoria, disco y procesador de cada uno. Investigue los costos de las licencias.

3.- Investigue las funciones del módulo TPM.

4.- Investigue los utilitarios que permiten cambiar el tamaño de las particiones. Por lo menos nombre a tres.

5.- Investigue gestores de arranque para elegir Sistemas Operativos múltiples en un equipo. Que trabajen en modo MBR o UEFI o ambos. # Haga una comparativa.

6.- Haga una lista comparativa de al menos 10 administradores de archivos. Pueden ser de diferentes plataformas. Compare 
funcionalidades y capacidades de expansión. Clasifíquelos luego por categoría con una descripción de cada una.
