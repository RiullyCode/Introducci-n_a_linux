# APUNTES NTRODUCCIÓN A LINUX

## ¿Qué es un sistema operativo?

Un sistema operativo (SO) es un programa que controla todo el hardware y software de un ordenador. Es como el "jefe" que organiza y gestiona todos los recursos y tareas del sistema.

### Funciones Principales de un Sistema Operativo:

1. **Gestión de Procesos**: 
   - **Proceso**: Es un programa en ejecución.
   - **Gestión**: El SO decide qué procesos deben ejecutarse y por cuánto tiempo, asegurando que cada uno reciba suficiente tiempo de CPU.

2. **Gestión de Memoria**:
   - **Memoria RAM**: Es el espacio de trabajo para los programas.
   - **Gestión**: El SO asigna memoria a los programas en ejecución y libera la memoria cuando ya no es necesaria.

3. **Gestión de Almacenamiento**:
   - **Archivos y Carpetas**: Todo se guarda en archivos organizados en carpetas.
   - **Gestión**: El SO maneja la lectura, escritura y organización de estos archivos en dispositivos como discos duros o SSDs.

4. **Control de Dispositivos**:
   - **Periféricos**: Son dispositivos externos como impresoras, monitores, teclados, etc.
   - **Gestión**: El SO actúa como intermediario, facilitando la comunicación entre el software y el hardware.

5. **Interfaz de Usuario**:
   - **GUI y CLI**: Las interfaces pueden ser gráficas (ventanas, íconos) o de línea de comandos (texto).
   - **Gestión**: El SO proporciona estas interfaces para que los usuarios interactúen con el sistema.

## ¿Qué es el pentesting?
***Pentesting o (Pruebas de Penetración)*** es una práctica para evaluar la seguridad de un sistema informático mediante simulaciones de ataques cibernéticos. Para esta tarea, se utilizan herramientas especializadas, y Parrot y Kali Linux son dos sistemas operativos populares entre los pentesters.

## Los sistemas operativos Parrot y Kali Linux para el pentesting

### Kali Linux:

1. **Preconfigurado**: Viene con cientos de herramientas de seguridad y pentesting preinstaladas, como Nmap, Metasploit, Wireshark, y más.
2. **Actualizaciones Frecuentes**: Ofrece actualizaciones regulares para mantener las herramientas al día con las últimas vulnerabilidades y técnicas.
3. **Documentación y Comunidad**: Tiene una amplia documentación y una gran comunidad de usuarios y desarrolladores, lo que facilita encontrar soporte y tutoriales.
4. **Especialización**: Está diseñado específicamente para pentesting y análisis forense, lo que significa que todas las configuraciones y optimizaciones están orientadas a estas tareas.

### Parrot OS:

1. **Multifuncional**: Además de pentesting, está diseñado para desarrollo de software, privacidad y uso diario.
2. **Ligero y Eficiente**: Consume menos recursos que Kali Linux, lo que puede ser útil en equipos con menos potencia.
3. **Seguridad Adicional**: Incluye características de privacidad y seguridad adicionales, como cifrado y anonimato.
4. **Herramientas Preinstaladas**: También viene con una amplia gama de herramientas para pentesting y seguridad informática.

![Kali_parrot](https://cdn.discordapp.com/attachments/914613587715182622/1249393900129620139/Kali_vs_Parrot.png?ex=6667243e&is=6665d2be&hm=6abffa17b055f200fa1bac05bc0b3a091623ea6ebd96030043ae67b014536ba1&)


### Uso de Windows para Pentesting (no recomendado)

Aunque Windows puede usarse para pentesting, presenta varias desventajas en comparación con Kali Linux y Parrot OS:

1. **Menos Herramientas Nativas**: Windows no viene preconfigurado con herramientas de pentesting, por lo que hay que instalarlas manualmente, lo que puede ser tedioso.
2. **Compatibilidad**: Algunas herramientas de pentesting están diseñadas específicamente para Linux y pueden no funcionar bien en Windows o requerir adaptaciones.
3. **Entorno de Trabajo**: La gestión de redes, scripts y automatización en Linux es más fluida gracias a la línea de comandos (bash) y scripts, mientras que en Windows puede ser más complicado.
4. **Recursos y Soporte**: Hay menos documentación y comunidad de pentesters utilizando Windows en comparación con Linux, lo que puede dificultar la resolución de problemas y el aprendizaje.
5. **Virtualización y Subsistema Linux**: Aunque Windows 10 y 11 incluyen el Subsistema de Windows para Linux (WSL), que permite ejecutar un entorno Linux dentro de Windows, no es tan eficiente y completo como utilizar un sistema Linux nativo.


## Pasos para descargar parrot OS

1. Lo primero que haremos será entrar en el siguiente [link](https://parrotsec.org/download/)
 el cual nos redirigrá a la página principal del sistema operativo parrot en el apartado de descargas *(a 09/06/2024 se ve de la siguiente manera)*

![Texto alternativo](https://cdn.discordapp.com/attachments/914613587715182622/1249441841762271283/image.png?ex=666750e4&is=6665ff64&hm=8a026507c730cc390a32e8115e0c90347bd3e40b414f643df9bbc425329cd9b2&)

En este apartado deberemos elegir el apartado que más nos convenga en función de lo que queramos, aquí una breve explicación

- **Live**:
   - Es la versión completa del sistema operativo que se puede ejecutar desde un dispositivo de almacenamiento extraíble sin necesidad de instalación. Esta edición permite instalar Parrot en el ordenador.

- **Virtual**:
   - Optimizada para ejecutarse en máquinas virtuales, perfecta para entornos virtualizados. Compatible con VirtualBox, VMware y UTM.

- **IoT**:
   - Diseñada para dispositivos integrados y plataformas de IoT como Raspberry Pi. 

- **Docker**:
   - Imagen de Docker preempaquetada del sistema operativo Parrot. Disponible en ediciones Core, Home y Security.

- **Debian Conversion Script**:
   - Script rápido para convertir una instalación existente de Debian a Parrot (todas las ediciones).

- **WSL**:
   - Permite usar todo el poder del sistema operativo Parrot en Windows mediante el Subsistema de Windows para Linux.

**En nuestro caso vamos a elegir la opción virtual ya que lo vamos a instalar en una máquina virtual.**

2. Ahora tendremos que elegir la edición correspondiente, en nuestro caso elegiremos la **security**, la opción *home* está pensada de cara a un uso más domestico.

![Texto alternativo](https://cdn.discordapp.com/attachments/914613587715182622/1249454587639758930/image.png?ex=66675cc3&is=66660b43&hm=76599274531485fa5db5ca0f8b3f82ba4a6338ca7a992be987cd484ae1ab2f47&)

3. Por último deberemos de elegir el tipo de arquitectura, nosotros como norma general elegiremos el tipo de arquitectura **AMD64**, pero dependerá del uso.

![Texto alternativo](https://cdn.discordapp.com/attachments/914613587715182622/1249460388395880560/image.png?ex=6667622a&is=666610aa&hm=54f1feeb820c04d8265fdd6be5b324bc1c975af70d2375d257d36ab98e1af5ce&)

Para determinar qué opción deberías elegir entre AMD64 y ARM64, debes considerar el tipo de procesador que tiene tu dispositivo.

1. **AMD64**:
   - Esta opción es para sistemas con arquitectura de 64 bits de AMD o Intel, que son los procesadores más comunes en ordenadores de escritorio y portátiles modernos. Si tu dispositivo es una ordenador estándar con un procesador Intel o AMD reciente, deberías elegir esta opción.

2. **ARM64**:
   - Esta opción está diseñada para dispositivos con procesadores basados en ARM, que son comúnmente utilizados en dispositivos móviles, tablets y algunos dispositivos de Internet de las Cosas (IoT). También es la arquitectura usada por algunos modelos de Raspberry Pi y otros dispositivos embebidos. Si estás usando una Raspberry Pi u otro dispositivo similar con un procesador ARM de 64 bits, esta es la opción adecuada para ti.

Una vez finalizados todos los pasos anteriores aparece lo siguiente: 

![Texto alternativo](https://cdn.discordapp.com/attachments/914613587715182622/1249462606314606785/image.png?ex=6667643b&is=666612bb&hm=c0e9cbe27d2d03c6362ce014158c1f3793d444e34354c50b576de1b2f98106b7&)

Basicamente es una breve descripción de la versión que vamos a descargar, nos da diferentes opciones para ejecutar la descarga y **nos dice las credenciales de serie para nuestro sistema**

```
user: parrot
password: parrot
```

Cuando le damos al botón de *download* vemos que nos encontramos con diferentes opciones.

![Texto alternativo](https://cdn.discordapp.com/attachments/914613587715182622/1249618807484452865/image.png?ex=6667f5b4&is=6666a434&hm=5d02d49bfb527e48091d9ae3f015dac0935265021296c471a4410cbfdb158ef1&)

Le daremos a la opción que corresponda que es donde lo vamos a emular, en mi caso usaré vmware así que le daré al botón de **VirtualBox**.

## Descarga de VirtualBox

Para ejecutar una máquina virtual existen diferentes aplicaciones, en mi caso he decidido hacer usar **VirtualBox** porque es de código abierto y permite ejecutar varias máquinas a la vez, si que es verdad que existen otras opciones como **Vmware**, pero las versiones gratis son algo más limitadas ya que solo permiten ejecutar una máquina a la vez.

1. Para ejecutar la descargar de VirtualBox nos dirigiremos al siguiente [link](https://www.virtualbox.org/wiki/Downloads) ***a 10/06/24 se ve de la siguiente manera:***

![Texto alternativo](https://media.discordapp.net/attachments/914613587715182622/1249618498938863680/image.png?ex=6667f56a&is=6666a3ea&hm=d5b8f3c5785373299149f56ea228bbd40a0a36268e11d01adc85e6daebd10004&=&format=webp&quality=lossless)

2. Si ahora nos dirigimos al apartado de descargas, nos encontraremos con que deberemos de tener estos 2 archivos  *(el instalador de virutalbox y la máquina parrot)*.

![Texto alternativo](https://cdn.discordapp.com/attachments/914613587715182622/1249621062761713745/image.png?ex=6667f7ce&is=6666a64e&hm=2abcc94e28c383843eb2b92c5d90c5629095b3404e0ed6eba260de200aab38fb&)

3. Le daremos doble click al ejecutable de virtualbox y nos aparecerá una ventana emergente como la siguiente en la que deberemos darle a **NEXT** en todos los pasos y por último le daremos a **FINISH**:

![Texto alternativo](https://cdn.discordapp.com/attachments/914613587715182622/1249622550284337194/image.png?ex=6667f930&is=6666a7b0&hm=2bfe3c2f21c2bcdb1c77b0be38e3872dcb7ef5de6ea0672f28b788156fd116e9&)


4. Si se ha instalado correctamente nos debería de aparecer la siguiente ventana emergente

![Texto alternativo](https://cdn.discordapp.com/attachments/914613587715182622/1249625634037039185/image.png?ex=6667fc10&is=6666aa90&hm=3c64d6bfecf26fb385c5a04fd190e7dcf1f4f654c772c8249ce6f7754a8e3511&)

**EN CASO DE QUERER CONFIGURAR LA RUTA DE INSTALACIÓN O EN CASO DE DUDA, CONSULTAR UN TUTORIAL EN YOUTUBE QUE HAY MUCHOS SOBRE INSTALACIÓN DE VIRTUAL BOX**

**EN CASO DE QUE NO FUNCIONE LA MÁQUINA LO MÁS SEGURO ES QUE NECESITEIS ACTIVAR LA VIRTUALIZACIÓN EN LA BIOS, CONSULTAR COMO HACERLO YA QUE DEPENDE DE CADA FABRICANTE, A ALGUNOS YA VIENE ACTIVADA DE SERIE**

## INSTALACIÓN DE LA MÁQUINA PARROT EN VIRTUALBOX

Lo que tendremos que hacer es añadir la máquina de parrot, desde la propia aplicación de parrot ***se te ve baja una máquina directamente, no una ISO*** por lo que tendremos que hacer en VirtualBox es añadir una máquina no crear una nueva *(esto sería en caso de que nos hubieran dado una ISO)*.

1. En el apartado de descargas, donde tenemos la máquina **Parrot-security-6.1_amd64** le daremos click derecho y le daremos a **ABRIR** *(debería aparecer el icono de VirtualBox, no adjunto captura porque no me deja)*:

![Texto alternativo](https://cdn.discordapp.com/attachments/914613587715182622/1249629863699157085/image.png?ex=66680000&is=6666ae80&hm=9096851e48ada88106876b8519eb7faeb6c39e7713451af7ca0dcca11d069327&)

2. Ahora nos debería de salir una ventana emergente en el virtualBox en la cual nos pone una resumen de las características de la máquina que vamos a agregar y la ubicación de la carpeta base de la máquina, y le daremos a terminar.

![Texto alternativo](https://cdn.discordapp.com/attachments/914613587715182622/1249630543495172187/image.png?ex=666800a2&is=6666af22&hm=f05503ac098dbcb4c706faaf124819a28ed58117dadd40fb8b677fe4d1e7a373&)

3. Ahora nos debería de aparecer otra ventana emergente en la que nos solicitará que aceptemos los terminos y condiciones, le daremos a **ACEPTAR**

![Texto alternativo](https://cdn.discordapp.com/attachments/914613587715182622/1249631681414041691/image.png?ex=666801b1&is=6666b031&hm=1711c1e8f1f4e815745af8d4e08bec7c73c35521467f0d25223ad7e42914e1b6&)

4. En la parte derecha de VirtualBox nos aparecerá una  barra de progreso en el que se inidica el tanto por ciento de importación realizada.

![Texto alternativo](https://cdn.discordapp.com/attachments/914613587715182622/1249633376617627708/image.png?ex=66680346&is=6666b1c6&hm=6dbe357f793cb49ec027e02e83b88d0115efbadbc5bc8be20e91cd5a7f1c5b11&)

5. Si todo lo anterior ha transcurrido correctamente se nos debería de haber agregado la máquina correctamente y deberiamos de ver el VirtualBox de la siguiente manera.

![Texto alternativo](https://cdn.discordapp.com/attachments/914613587715182622/1249633811860291604/image.png?ex=666803ad&is=6666b22d&hm=572c6d32569a193568ad8c726b26a721db939dc7d752e00bdec2e9138fa361bd&)


