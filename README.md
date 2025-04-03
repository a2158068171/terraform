# Despliegue de AWS mediante Terraform

Este es un proyecto para desplegar instancias en **Amazon Web Services** mediante el uso de **Terraform**

--------

## 📂 Estructura 


```
.
├── README.md             # Documentación de todo el proyecto
├── main.tf               # Configuración para el despliegue de la instancia en AWS
├── variables.tf          # Variables para la instancia 
├── outputs.tf            # Configuración de salida
└── terraform.tfstate     # Informacion de estado de insfraestructura (No se incluye, informacion privada)
```

------

## 📋​ Preequisitos

- **Terraform** Descargar e instalar [Terraform](https://developer.hashicorp.com/terraform/downloads).

- **Cuenta de AWS** Cuenta de **Amazon Web Services** con acceso IAM [AWS](https://aws.amazon.com/es/).

- **Instalacion de AWS CLI** Descargar e instalar el CLI de AWS ademas de configurarlo [AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-welcome.html)
  
- **Powershell** Utilizaremos el powershell de windows 10 los comandos de **AWS** y **Terraform**

------

## 🦮​ Guia

1. **Clonar el repositorio**:

   ```
   git clone https://github.com/a2158068171/terraform.git
   ```

2. **Configurar AWS**:

   Crea una persona en IAM en AWS con clave de acceso [IAM](https://aws.amazon.com/es/iam/)

3. **Configurar AWS CLI**

   Una vez creado una persona en AWS, configuraremos el Access Key ID y el Secret Access Key

   ```
   aws configure 
   ```
   Introduciremos el Access Key ID y el Secret Access Key que nos genero de la persona de IAM de AWS

4. **Inicializar Terraform**:

   ```
   terraform init
   ```
   Descarga e instala los proveedores de la configuración e inicializa el directorio de trabajo de Terraform

4. **Planificar la ejecución**:

   ```
   terraform plan
   ```

  - Validar los cambios de configuración contra el estado remoto y los recursos en la nube
  - Revisar y validar los cambios antes de que se apliquen a la infraestructura de producción 
  - Identificar y abordar los posibles problemas antes de que interrumpan los servicios 
  - Planificar y ejecutar los cambios en la infraestructura de manera metódica 

5. **Aplicar el plan**:

   ```bash
   terraform apply
   ```

  - Verifica la configuración y el estado actual de la infraestructura 
  - Genera un plan de ejecución para revisar los cambios 
  - Aplica los cambios necesarios para alcanzar el estado deseado de la infraestructura 

------


## 📚 Recursos adicionales

- [Documentación oficial de Terraform](https://developer.hashicorp.com/terraform/docs)
- [Guía de oficial de AWS de Terraform](https://developer.hashicorp.com/terraform/tutorials/aws-get-started/install-cli)

------
