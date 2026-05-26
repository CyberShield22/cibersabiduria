---
title: Sistemas Operativos
description: Apuntes, prácticas, ejercicio del curso de especialización de ciberseguridad. Arkime, blue team, seguridad devensiva, análisis de red, escáner de red, bastionado de redes y sistemas.
---
# Sistemas Operativos

## ¿Qué es un sistema operativo?

Un sistema operativo (SO) es el software encargado de gestionar los recursos de hardware y permitir la ejecución de aplicaciones. Actúa como intermediario entre el usuario y el equipo, facilitando la comunicación con componentes como la CPU, la memoria, el disco o los dispositivos de entrada y salida.

Además de ejecutar programas, el sistema operativo controla procesos, organiza archivos, administra memoria y garantiza la seguridad y estabilidad del sistema.

---

## Funciones principales

Las funciones más importantes de un sistema operativo son:

- Gestión de procesos y multitarea
- Administración de memoria
- Gestión del sistema de archivos
- Control de dispositivos de entrada y salida
- Seguridad y permisos
- Proporcionar interfaces de usuario (CLI y GUI)

Gracias a estas funciones, varias aplicaciones pueden ejecutarse simultáneamente de forma estable y segura.

---

## Tipos de sistemas operativos

### Sistemas de escritorio

Son los utilizados en ordenadores personales y estaciones de trabajo. Están diseñados para facilitar la interacción con el usuario mediante interfaces gráficas.

Ejemplos:

- Windows
- Linux
- macOS

### Sistemas de servidor

Optimizados para ofrecer servicios de red, almacenamiento, virtualización o aplicaciones empresariales con alta disponibilidad y estabilidad.

### Sistemas embebidos

Diseñados para dispositivos específicos con recursos limitados, como routers, electrodomésticos o dispositivos IoT.

### Sistemas en tiempo real (RTOS)

Garantizan respuestas dentro de tiempos concretos y se utilizan en entornos industriales, aeronáuticos o médicos.

### Sistemas distribuidos

Permiten que múltiples equipos trabajen de forma coordinada compartiendo recursos y tareas a través de una red.

### Hipervisores

Sistemas especializados en ejecutar máquinas virtuales y administrar entornos virtualizados.

---

## Historia de los sistemas operativos

Los primeros ordenadores no utilizaban sistemas operativos. Los programas se ejecutaban directamente sobre el hardware mediante tarjetas perforadas y lenguaje máquina.

Con la aparición de los mainframes en los años 50 y 60 comenzaron a desarrollarse sistemas capaces de automatizar tareas como la carga de programas o la gestión de entrada y salida.

Uno de los grandes hitos fue UNIX, cuyo diseño influyó profundamente en los sistemas modernos. A partir de él surgieron estándares como POSIX y sistemas derivados como BSD o Linux.

Actualmente, Linux domina gran parte de servidores, centros de datos, cloud computing y dispositivos Android.

---

## Componentes principales

### Kernel

El kernel es el núcleo del sistema operativo. Se encarga de gestionar el acceso al hardware, controlar procesos, administrar memoria y coordinar dispositivos.

Es el componente más importante del sistema.

### Procesos e hilos

Un proceso es un programa en ejecución. Los sistemas modernos permiten ejecutar múltiples procesos simultáneamente mediante multitarea.

Los hilos (threads) permiten dividir tareas dentro de un mismo proceso para mejorar el rendimiento.

### Gestión de memoria

El sistema operativo administra la memoria RAM y evita que los procesos interfieran entre sí.

También utiliza memoria virtual para ampliar la memoria disponible mediante swap o paginación.

### Sistema de archivos

Permite organizar y almacenar información en archivos y directorios.

Además, controla permisos, acceso a datos y mecanismos de protección frente a errores.

### Entrada y salida (I/O)

Gestiona la comunicación con dispositivos como discos, teclados, ratones o tarjetas de red mediante controladores e interrupciones.

---

## Seguridad

Los sistemas operativos modernos incorporan mecanismos de seguridad para proteger datos y procesos.

Entre ellos destacan:

- Gestión de usuarios y permisos
- Aislamiento entre procesos
- Protección de memoria
- Control de privilegios
- Autenticación y auditoría

El objetivo es garantizar la confidencialidad, integridad y disponibilidad del sistema.

---

## Interfaz de usuario

Los sistemas operativos pueden ofrecer:

### CLI (Command Line Interface)

Interacción mediante comandos de texto. Muy utilizada en administración de sistemas y automatización.

### GUI (Graphical User Interface)

Interfaz gráfica basada en ventanas, iconos y menús, más sencilla para usuarios generales.

---

## Portabilidad y compatibilidad

No todos los sistemas operativos utilizan las mismas APIs o llamadas al sistema, por lo que una aplicación puede requerir adaptaciones para funcionar en diferentes plataformas.

Para mejorar la compatibilidad se utilizan estándares como:

- POSIX
- JVM (Java Virtual Machine)
- Frameworks multiplataforma como Qt

Estas tecnologías permiten desarrollar software portable entre distintos sistemas.