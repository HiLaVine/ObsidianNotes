Un sistema operativo es la interfaz entre el hardware de la computadora y el usuario. 

## Como funciona un sistema operativo

El siguiente diagrama explica la cadena de sucesos que sigue un sistema operativo para funcionar. 

```mermaid
graph LR
    User --> Application
    Application --> OS
    OS --> Hardware
    Hardware --> OS
    OS --> Application
    Application --> User
```

Como vemos primero esta el usuario: Que lleva a cabo las tareas y usa aplicaciones en la computadora. 

Luego las aplicaciones, que son programas que se encargan de llevar a cabo una tarea especifica. 

Esta aplicación hace la petición al SO que interpreta la petición y se encarga de enviarla al componente apropiado de hardware. 

Y en el hardware pasa la magia. Como el uso de memoria, el teclado, mouse, cámara, etc. 

## BIOS y UEFI

La BIOS (Basic Input Output System) es un microchip que contiene instrucciones de carga para la computadora y que es común en los sistemas mas antiguos. 

UEFI (Unified Extensible Firmware Interface) es un microchip que contiene instrucciones de carga para la computadora y reemplaza al BIOS en los sistemas más modernos. 

## Asignación de recursos 

El SO también es el encargado de gestionar los recursos del sistema. Esta gran tarea requiere mucho equilibrio para que todos los recursos de la computadora se usen eficientemente. 

## GUI frente a  CLI

La interfaz de usuario es un programa que permite al usuario controlar las funciones del sistema operativo. 

Hay dos interfaces de usuario:
- GUI (Grafic User Interface): Utiliza iconos para gestionar varias tareas y la mayoría de sistemas operativos tienen una. 
- CLI (Comand Line Interface): Es una interfaz basada en texto que usa comandos para interactuar con la computadora. Estos comandos se comunican con el sistema operativo y ejecutan las tareas. 
