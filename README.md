💾 Gestión de tarjeta microSD con ESP32

Este proyecto implementa un sistema completo de gestión de archivos y directorios utilizando una tarjeta microSD conectada a una ESP32 mediante comunicación SPI.

🧠 Descripción

El programa permite realizar operaciones avanzadas sobre el sistema de archivos de una tarjeta SD, simulando funcionalidades básicas de un sistema operativo en un entorno embebido.

Se pueden crear, leer, modificar y eliminar archivos y carpetas, así como visualizar la estructura completa de la tarjeta.

🔧 Funcionalidades

📁 Gestión de directorios

Crear directorios (mkdir)
Borrar directorios vacíos (rmdir)
Borrado recursivo de directorios (incluyendo contenido)
Navegación por carpetas
Mostrar estructura en árbol

📄 Gestión de archivos

Crear archivos
Escribir contenido
Añadir datos (append)
Leer archivos
Borrar archivos
Renombrar archivos
Comprobar existencia

📂 Operaciones avanzadas

Copiar archivos
Calcular tamaño de directorios (recursivo)
Listar archivos con nombre y tamaño
Mostrar árbol completo del sistema de archivos

🌳 Ejemplo de salida
/
  [DIR] practica
    [DIR] logs
      [FILE] log1.txt
    [DIR] datos
      [FILE] sensor.txt
    [FILE] info.txt
    
🔌 Hardware utilizado

ESP32
Módulo microSD (MH-SD Card Module)
Tarjeta microSD (formateada en FAT32)

⚙️ Conexión (SPI)

Módulo SD	ESP32
3.3V	3V3
GND	GND
CS	GPIO 5
SCK	GPIO 18
MOSI	GPIO 23
MISO	GPIO 19

🚀 Uso

Formatear la tarjeta en FAT32
Conectar el módulo a la ESP32
Subir el código
Abrir el monitor serie (115200 baudios)
Observar las operaciones realizadas automáticamente

⚠️ Requisitos y limitaciones

La tarjeta debe estar en formato FAT32
No compatible con exFAT en la mayoría de implementaciones
El módulo debe estar correctamente alimentado (3.3V o 5V según modelo)
Los directorios deben estar vacíos para usar rmdir (salvo borrado recursivo)

🧠 Aplicaciones

Este sistema puede utilizarse en proyectos como:

Registro de datos de sensores (logging)
Sistemas IoT
Almacenamiento de configuraciones
Sistemas de control y monitorización

📌 Conclusión

El proyecto demuestra que es posible implementar un sistema completo de gestión de archivos en un entorno embebido con recursos limitados, utilizando una ESP32 y una tarjeta microSD.
