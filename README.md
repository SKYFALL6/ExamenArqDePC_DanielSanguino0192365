# Examen Final Arquitectura de Computadores
**Estudiante:** Daniel Alexis Sanguino Rodríguez
**Código:** 0192365

## Objetivo del proyecto
Diseñar, versionar, desplegar y eliminar de manera automatizada una máquina virtual en AWS utilizando CloudFormation y GitHub Actions bajo las buenas prácticas de Git Flow.

## Tecnologías utilizadas
* AWS (EC2, CloudFormation, IAM)
* GitHub Actions (CI/CD)
* Git & Git Flow
* HTML / CSS / JS

## Funcionalidad de Deploy
El workflow `Deploy Infrastructure` se encarga de validar el template de CloudFormation y desplegar de forma automática un Stack en AWS que aprovisiona una instancia EC2 con su respectivo Security Group (puerto 80 abierto). Adicionalmente, ejecuta el bloque de UserData para instalar Apache y levantar la página web informativa.

## Funcionalidad de Destroy
El workflow `Destroy Infrastructure` automatiza la eliminación completa del Stack de CloudFormation, asegurando el borrado inmediato de la instancia EC2 y los recursos asociados para evitar costos residuales en la cuenta de AWS.

## Objetivo del template EC2 creado
Definir la Infraestructura como Código (IaC) requerida para configurar un servidor virtual basado en Amazon Linux, garantizando que el entorno web sea estandarizado, seguro y fácilmente replicable.