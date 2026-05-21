Prueba
## ¿Qué es un sistema operativo?
Un sistema operativo es el software esencial que gestiona los recursos de hardware y software de un ordenador y proporciona servicios básicos para el funcionamiento de las aplicaciones. Actúa como intermediario entre el usuario y la máquina, encargándose de tareas como la gestión de procesos, la memoria, los sistemas de archivos y los dispositivos. Al ocultar la complejidad del hardware, permite que los programas se ejecuten de forma estable y coherente en distintos entornos.

## Tipos de sistemas operativos
### Sistemas operativos multicomputadores
Con multiprocesadores Varias CPU comparten memoria. A multicomputadora o cluster computer tiene varias CPU, cada una de las cuales tiene su propia memoria. Se desarrollaron multicomputadoras porque los multiprocesadores grandes son difíciles de diseñar y prohibitivamente caros. Son universales en computación en la nube debido al tamaño de la máquina necesaria. Las diferentes CPU a menudo necesitan enviarse y recibir mensajes entre sí. Para garantizar un buen rendimiento, los sistemas operativos de estas máquinas deben minimizar esta copia de paquetes. Los sistemas más nuevos suelen serlo multiqueue—separar grupos de usuarios en grupos separados queues—para reducir la necesidad de copiar paquetes y admitir más usuarios simultáneos. Otra técnica es acceso remoto directo a la memoria, que permite a cada CPU acceder a la memoria perteneciente a otras CPU. Los sistemas operativos multicomputadores a menudo admiten llamadas a procedimientos remotos donde una CPU puede llamar a procedimiento en otra CPU o memoria compartida distribuida, en el que utiliza el sistema operativo virtualización para generar memoria compartida que no existe físicamente.

### Sistemas distribuidos
A sistema distribuido es un grupo de distintos, en red computadoras—cada una de las cuales podría tener su propio sistema operativo y sistema de archivos. A diferencia de las multicomputadoras, pueden estar dispersas en cualquier parte del mundo. Middleware, a menudo se utiliza una capa de software adicional entre el sistema operativo y las aplicaciones para mejorar la coherencia. Aunque funciona de manera similar a un sistema operativo, no es un verdadero sistema operativo.

### Incrustado
Sistemas operativos integrados están diseñados para ser utilizados en sistemas informáticos integrados, si lo son Internet de las cosas objetos o no conectados a una red. Los sistemas integrados incluyen muchos electrodomésticos. El factor distintivo es que no cargan el software instalado por el usuario. En consecuencia, no necesitan protección entre diferentes aplicaciones, lo que permite diseños más simples. Los sistemas operativos muy pequeños pueden funcionar en menos de 10 kilobytes y los más pequeños son para tarjetas inteligentes. Los ejemplos incluyen: Linux integrado, QNX, VxWorks, y los sistemas extrapequeños DISTURBIOS y TinyOS.

### Tiempo real
A sistema operativo en tiempo real es un sistema operativo que garantiza el procesamiento eventos o datos por o en un momento específico en el tiempo. Los sistemas duros en tiempo real requieren una sincronización exacta y son comunes en fabricación, aviónica, usos militares y otros usos similares. Con sistemas suaves en tiempo real, es aceptable que se pierda algún evento ocasional; esta categoría a menudo incluye sistemas de audio o multimedia, así como teléfonos inteligentes. Para que los sistemas duros en tiempo real sean lo suficientemente exactos en su sincronización, a menudo son solo una biblioteca sin protección entre aplicaciones, como por ejemplo Cos electrónico.

### Hipervisor
A hipervisor es un sistema operativo que ejecuta un máquina virtual. La máquina virtual es una aplicación que emula hardware; en otras palabras, funciona tanto como sea posible como el hardware real para el que fue diseñado el sistema operativo. Las máquinas virtuales se pueden pausar, guardar y reanudar, lo que las hace útiles para la investigación y el desarrollo de sistemas operativos y depuración. También mejoran la portabilidad al permitir que las aplicaciones se ejecuten en una computadora incluso si no son compatibles con el sistema operativo base.

### Biblioteca
A sistema operativo de biblioteca (libOS) es aquel en el que los servicios que proporciona un sistema operativo típico, como la red, se proporcionan en forma de bibliotecas y compuesto con una única aplicación y código de configuración para construir un unikernel: a especializado (solo se extraen de las bibliotecas los fragmentos de código absolutamente necesarios y se unen entre sí ), espacio de dirección única, imagen de máquina que se puede implementar en entornos integrados o en la nube.

El código del sistema operativo y el código de la aplicación no se ejecutan por separado dominios de protección (solo hay una única aplicación ejecutándose, al menos conceptualmente, por lo que no hay necesidad de evitar interferencias entre aplicaciones) y se accede a los servicios del sistema operativo mediante simples llamadas a la biblioteca (potencialmente inlining ellos basados en umbrales del compilador), sin la sobrecarga habitual de cambios de contexto, de manera similar a los sistemas operativos integrados y en tiempo real. Esta sobrecarga no es despreciable: al coste directo del cambio de modo hay que añadir la contaminación indirecta de importantes estructuras de procesador (como Cachés de CPU, el canalización de instrucciones, y así sucesivamente), lo que afecta tanto al rendimiento en modo usuario como en modo kernel.

## Historia
Los sistemas operativos no siempre existieron como los conocemos hoy. Su evolución ha estado directamente ligada al crecimiento del hardware, la necesidad de automatización y el acceso compartido a los recursos de computación.
### Los primeros sistemas (1940–1950)

Las primeras computadoras de finales de los años 40 y 50 no disponían de sistemas operativos.

La programación se realizaba de forma directa sobre la máquina mediante:

- Lenguaje máquina
- Tarjetas perforadas
- Paneles de conexión física (plugboards)

En este contexto, no existían lenguajes de programación de alto nivel ni abstracciones. El control del sistema era completamente manual, lo que hacía que cada ejecución fuera costosa y lenta.
### La era de los mainframes y los primeros sistemas de control

Con la llegada del **transistor en los años 50**, comenzaron a aparecer los primeros mainframes.

Aunque todavía requerían operadores humanos especializados, empezaron a incluir sistemas rudimentarios encargados de automatizar tareas como:

- Planificación de trabajos (job scheduling)
- Gestión básica de entrada/salida
- Ejecución secuencial de programas

Entre los sistemas más representativos de esta etapa destacan:

- **FMS (Fortran Monitor System)**
- **IBSYS**

Estos sistemas no eran sistemas operativos modernos, pero sentaron las bases de lo que vendría después.
### IBM System/360 y el nacimiento de la multiprogramación

En la década de 1960, IBM introdujo la familia **System/360**, uno de los hitos más importantes en la historia de la computación.

Todos los modelos ejecutaban un sistema operativo común:

- **OS/360**

Este sistema estaba escrito principalmente en lenguaje ensamblador y llegó a tener millones de líneas de código, lo que lo hacía extremadamente complejo.

A pesar de sus problemas, introdujo avances fundamentales como la **multiprogramación**, que permitía:

- Ejecutar varios programas en memoria al mismo tiempo
- Aprovechar la CPU mientras otros procesos esperaban operaciones de entrada/salida

Esto obligó a introducir mecanismos como:

- Gestión de memoria por particiones
- Protección entre procesos
### Tiempo compartido y MULTICS

En paralelo, comenzaron a utilizarse terminales como las teleimpresoras, lo que permitió el acceso simultáneo de múltiples usuarios a un mismo sistema.

El sistema **MULTICS** fue uno de los primeros intentos de construir un sistema multiusuario a gran escala, con el objetivo de dar servicio a cientos de usuarios concurrentes.

Aunque su adopción fue limitada, su diseño influyó profundamente en la evolución de los sistemas modernos y es considerado un precursor conceptual de la **computación en la nube**.
### UNIX: el punto de inflexión

El sistema operativo **UNIX** nació como una alternativa más simple inspirada en MULTICS, inicialmente diseñado para un entorno de un solo usuario.

Su impacto creció rápidamente debido a una característica clave: su código fuente era accesible, lo que permitió su adaptación y evolución en múltiples variantes.

Entre las más importantes destacan:

- **System V (AT&T)**
- **BSD (University of California, Berkeley)**

Para estandarizar la compatibilidad entre sistemas UNIX, el IEEE desarrolló el estándar:

- **POSIX**, que define interfaces de programación comunes (API).
### MINIX y el nacimiento de Linux

**MINIX** fue creado en 1987 como una versión simplificada de UNIX con fines educativos.

Aunque limitado, tuvo un impacto enorme al inspirar el desarrollo de **Linux**, uno de los sistemas operativos más importantes de la actualidad.

Hoy en día:

- MINIX se utiliza en controladores de microchips Intel
- Linux domina servidores, centros de datos y sistemas Android
## Componentes de un sistema operativo
Los sistemas operativos están formados por varios componentes que trabajan juntos para gestionar el hardware y permitir la ejecución de aplicaciones de forma segura y eficiente.
### Kernel (núcleo del sistema)

El **kernel** es el componente central del sistema operativo.

Sus funciones principales son:

- Gestionar el acceso al hardware
- Proteger procesos y usuarios entre sí
- Asignar memoria y recursos
- Controlar dispositivos de entrada/salida

El kernel opera en **modo privilegiado**, mientras que las aplicaciones se ejecutan en **modo usuario**, lo que permite aislar fallos y mejorar la seguridad del sistema.
### Ejecución de programas

Cuando se ejecuta un programa, el sistema operativo:

- Crea un **proceso**
- Asigna memoria y recursos
- Carga el código en memoria
- Establece su prioridad
- Inicia su ejecución

El programa interactúa con el hardware siempre a través del sistema operativo, nunca directamente.
### Interrupciones

Las **interrupciones** permiten al sistema operativo reaccionar a eventos de forma eficiente.

Tipos principales:

- **Hardware**: eventos del dispositivo (teclado, disco, red)
- **Software**: errores o llamadas del sistema
- **Excepciones**: división por cero, accesos inválidos

Cuando ocurre una interrupción:

1. Se guarda el estado del proceso actual
2. Se ejecuta una rutina del kernel
3. Se restaura el proceso o se cambia a otro

Esto permite multitarea y respuesta en tiempo real.
### Gestión de memoria

El sistema operativo se encarga de proteger y organizar la memoria:

- Evita que los procesos se interfieran entre sí
- Detecta accesos no permitidos
- Usa mecanismos como **paginación** y **segmentación**

Si un programa accede a memoria inválida, el sistema genera una excepción y puede terminar el proceso.
### Memoria virtual

La memoria virtual permite que los programas “vean” más memoria de la que realmente existe.

Esto se logra combinando:

- RAM
- Disco (swap)

Beneficios:

- Mejor uso de recursos
- Mayor aislamiento entre procesos
- Posibilidad de ejecutar programas más grandes
### Concurrencia y procesos

Los sistemas operativos modernos pueden ejecutar múltiples tareas a la vez mediante:

- **Procesos**
- **Hilos (threads)**

El sistema reparte el tiempo de CPU entre tareas o las ejecuta en paralelo si hay múltiples núcleos.
### Sistema de archivos

El sistema de archivos organiza la información en:

- Archivos
- Directorios

Permite:

- Guardar y recuperar datos
- Gestionar permisos
- Optimizar acceso mediante caché
- Proteger contra corrupción de datos
### Entrada / salida (I/O)

El sistema operativo gestiona dispositivos como:

- Teclado y ratón
- Disco duro / SSD
- Red

Métodos importantes:

- **Interrupciones**: eventos por dispositivo
- **DMA (Direct Memory Access)**: transferencia sin CPU directa
### Seguridad

La seguridad del sistema operativo se basa en:

- Aislamiento de procesos
- Control de permisos
- Protección de memoria
- Principio de mínimo privilegio

Objetivo: garantizar confidencialidad, integridad y disponibilidad del sistema.
### Interfaz de usuario

Permite la interacción con el sistema:

- **CLI (línea de comandos)**: texto
- **GUI (interfaz gráfica)**: ventanas, iconos, menús

Las GUI son más amigables para usuarios, mientras que la CLI es más eficiente para administradores y desarrolladores.
## Sistemas operativos como hobby (pasatiempo)

Algunos sistemas operativos se desarrollan como proyectos personales o de afición, sin estar basados directamente en sistemas existentes y con comunidades pequeñas o muy activas.

Estos proyectos suelen ser creados por desarrolladores independientes o pequeños grupos con intereses comunes.
### Características principales

Un sistema operativo “de hobby” suele:

- No derivar de sistemas comerciales existentes
- Tener pocos usuarios y desarrolladores
- Ser experimental o educativo

En muchos casos, estos proyectos nacen para hardware específico, como:

- Ordenadores “homebrew”
- Placas simples basadas en microprocesadores (ej. 6502)

También pueden desarrollarse para arquitecturas modernas, ya sea desde cero o inspirándose en sistemas existentes.
### Ejemplos conocidos

Algunos sistemas operativos desarrollados como hobby o proyectos experimentales son:

- **TempleOS**
- **Syllable OS**
## Diversidad de sistemas operativos y portabilidad

Uno de los grandes retos del desarrollo de software es la **portabilidad entre sistemas operativos**.

Una aplicación diseñada para un sistema concreto puede requerir modificaciones al ejecutarse en otro, debido a diferencias en:

- APIs del sistema
- Llamadas al sistema
- Bibliotecas disponibles
- Convenciones internas

Esto genera un coste adicional de adaptación y mantenimiento.
### Soluciones a la portabilidad

Para reducir estos problemas, se utilizan varias estrategias:

#### 1. Plataformas intermedias

Se desarrollan aplicaciones sobre capas de abstracción como:

- **Java Virtual Machine (JVM)**
- **Qt framework**

Estas plataformas actúan como intermediarios entre la aplicación y el sistema operativo.
#### 2. Estándares de compatibilidad

Otra solución es la adopción de estándares comunes, como:

- **POSIX**
- Capas de abstracción del sistema operativo (OS abstraction layers)

Estos estándares facilitan que el mismo software pueda ejecutarse en múltiples sistemas con menos cambios.