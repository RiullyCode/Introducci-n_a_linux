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

![Texto alternativo](https://cdn.discordapp.com/attachments/914613587715182622/1249706018863321258/image.png?ex=666846ed&is=6666f56d&hm=dde34a2ed28111e33c650eae980cc2bbb942287ce31792ba2a46e266c87682df&)

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

**En nuestro caso vamos a elegir la opción LIVE.**
(Lo vamos a instalar en un máquina virtual pero si nos bajamos la opción virtual vendrá ya la máquina preconfigurada cosa que no queremos)

2. Ahora tendremos que elegir la edición correspondiente, en nuestro caso elegiremos la **SECURITY**, la opción *home* está pensada de cara a un uso más domestico.

![Texto alternativo](https://cdn.discordapp.com/attachments/914613587715182622/1249707943759446076/image.png?ex=666848b8&is=6666f738&hm=e258120c981d33bcd0433a68a659aefde2d51efc2c03f1c952df9b3939cc6601&)

3. Por último deberemos de elegir el tipo de arquitectura **AMD64**.

![Texto alternativo](https://media.discordapp.net/attachments/914613587715182622/1249709853577056266/image.png?ex=66684a7f&is=6666f8ff&hm=7f61fa9d43791a9362875e28cb11a23f55deca9698cb3ac3dfc4476ddbf16150&=&format=webp&quality=lossless&width=720&height=216&)



Una vez finalizados todos los pasos anteriores aparece lo siguiente: 

![Texto alternativo](https://cdn.discordapp.com/attachments/914613587715182622/1249710369883291678/image.png?ex=66684afa&is=6666f97a&hm=e4de6c083bed15f1385b5564772cce90d061c8b3b797e664c93cee2a28720b5b&)

Basicamente es una breve descripción de la versión que vamos a descargar, nos da diferentes opciones para ejecutar la descarga y **nos dice las credenciales de serie para nuestro sistema**

```
user: parrot
password: parrot
```


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

Lo que tendremos que hacer es *CREAR UNA MÁQUINA NUEVA*, desde la propia aplicación web de Parrot ***se te ve baja una ISO*** por lo que tendremos que hacer en VirtualBox es añadir crear una máquina nueva.

1. En el apartado de descargas, Deberemos de tener la ISO **Parrot-security-6.1_amd64**.

![Texto alternativo](https://cdn.discordapp.com/attachments/914613587715182622/1249722420558958622/image.png?ex=66685633&is=666704b3&hm=3e0314e5524bcbd76bc3ce72ca062c043847e3792aa2f41668e6eeec39977c79&)

2. Ahora dentro de virtualBox, en el apartado superior nos deberíamos encontrar un menú, en el cual le deberemos dar a **NUEVA** (*es una especie de estrella azul*).

![Texto alternativo](https://media.discordapp.net/attachments/914613587715182622/1249719798494138480/image.png?ex=666853c2&is=66670242&hm=b6059f4f9f2eb21805035a245a301a558d801ac07770515001cd8be784c99592&=&format=webp&quality=lossless)

3. Ahora nos debería de aparecer una ventana emergente en la que nos solicitará un nombre para la máquina, la carpeta en que se instalará la máquina y la ubicación de la imagen ISO que hemos descargado anteriormente (el resto de campos se autocompletaran al poner la ISO). Por último le daremos a **SIGUIENTE**.

![Texto alternativo](https://cdn.discordapp.com/attachments/914613587715182622/1249724260776149032/image.png?ex=666857ea&is=6667066a&hm=bcf78b1312850073a5d2138fb9e73897c1108981f149f25f23003896bb8af8fa&)

4. La ventana emergente cambiará y ahora tendremos que ajustar la memoria RAM que utilizará la máquina y el número de procesadores que usará. En mi caso pondré **8192MB Y 3CPUs**. Cabe recalcar que no hace falta tanta potencia pero en mi caso tengo un equipo relativamente potente y no hay problema.

![Texto alternativo](https://cdn.discordapp.com/attachments/914613587715182622/1249725520573235331/image.png?ex=66685916&is=66670796&hm=9bec2d6682aafa86216fa4bb2ebe3fc8111fa23ec05d76fa57ac8de77b1b0c9c&)

5. La ventana emergente cambiará y ahora deberemos indicar el tamaño del disco duro virtual, que será donde se almacenen los datos de la máquina, pondremos **60 GB** y le daremos a **SIGUIENTE**.

![Texto alternativo](https://cdn.discordapp.com/attachments/914613587715182622/1249727810709356603/image.png?ex=66685b38&is=666709b8&hm=3ed792edb12144d5d89361472b4869d2e1803a65fae23c0fbc90650a69afc6d8&)

6. Por último nos aparecerá un breve resumen de la configuración que hemos realizado en la máquina virtual, si vemos todo correcto, le daremos al botón de **TERMINAR.**

![Texto alternativo](https://media.discordapp.net/attachments/914613587715182622/1249729444780970007/image.png?ex=66685cbe&is=66670b3e&hm=69875a02c9e1b26390efe7a3c39d5f144557ed874301f2d8b4afa907a2af6279&=&format=webp&quality=lossless&width=720&height=371)

## Arranque de la máquina PARROT

1. Una vez que hemos realizado todos los pasos anteriores con éxito le daremos a **INICIAR** que es el botón que se encuentra en la parte superior derecha que tiene el icono de una flecha apuntando hacia la derecha *(si aparece la foto de linux en blanco y negro es normal)*.

![Texto alternativo](https://media.discordapp.net/attachments/914613587715182622/1249729686062370916/image.png?ex=66685cf8&is=66670b78&hm=089ca0605d89aeb6eb841ca05253c99e852de928cae4117910562855612d4542&=&format=webp&quality=lossless&width=720&height=275)

2. Al darle a iniciar, nos encontraremos con la siguiente ventana, en la que deberemos darle a **TRY INSTALL**

![Texto alternativo](https://media.discordapp.net/attachments/914613587715182622/1249730928868196462/image.png?ex=66685e20&is=66670ca0&hm=4f572955f3805fa4b68b0a160d589d90dd8a11a640aac73e732941ef34e5c63e&=&format=webp&quality=lossless)

3. Después se instalará el sistema operativo, y apareceremos en el escritorio.

![Texto alternativo](https://cdn.discordapp.com/attachments/914613587715182622/1249732469133938799/image.png?ex=66685f8f&is=66670e0f&hm=c2448f8fa89195aff40556fcfdae63b3f5f89544259a51cc15b9cccf7c71f7d6&)

4. Si nos fijamos vienen 5 accesos directos en el escritorio, hay uno que se llama **INSTALL PARROT**

![Texto alternativo](https://media.discordapp.net/attachments/914613587715182622/1249733366773710931/image.png?ex=66686065&is=66670ee5&hm=551465d8aaa0cfeb1aa141868c887b138559afa6fad2fddd9b5ea9ffe672b6e9&=&format=webp&quality=lossless)

5. Hacemos doble click y se nos abrirá la siguiente ventana emergente en la que deberemos configurar el sistema operativo. Lo primero hace referencia al idioma, pondremos **ESPAÑOL DE ESPAÑA** y le daremos a **SIGUIENTE**.

![Texto alternativo](https://cdn.discordapp.com/attachments/914613587715182622/1249734643662454896/image.png?ex=66686195&is=66671015&hm=5bae3791ff3e08fa80aef8b27df1c3ec7ad2c9cb4858545427b3c13ce077422a&)

6. El siguiente apartado hace referencia a la ubicación, le daremos **EUROPE**,a **MADRID** y le daremos a **SIGUIENTE**.

![Texto alternativo](https://cdn.discordapp.com/attachments/914613587715182622/1249735060995706880/image.png?ex=666861f9&is=66671079&hm=ba2fb3058165e3afe6ee72c3758851459d212d80e1e00c7586eb45cf6f71d0f1&)

7. El siguiente apartado hace referencia a la distribución del teclado, le daremos a **SPANISH** y **DEFAULT**, podemos probar que se ha aplicado correctamente y le daremos a siguiente

![Texto alternativo](https://cdn.discordapp.com/attachments/914613587715182622/1249736178790301746/image.png?ex=66686303&is=66671183&hm=209c011dcafe8a31b988cc281ccfcf0394402a495b175177dee56c8f9aade8aa&)