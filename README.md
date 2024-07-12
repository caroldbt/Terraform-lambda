
# Proyecto de Servidor Web con Apache, PHP, Lambda en Python y Slack hecha con Terraform

## Descripción
Este proyecto implementa un servidor web con Apache y PHP en una instancia EC2 de AWS. El servidor web incluye un formulario de contacto que envía datos a un tema SNS de AWS, el cual a su vez desencadena una función Lambda en Python que envía notificaciones a Slack.

## Archivo
```plaintext
.
├── README.md
├── main.tf
├── submit.php
├── install_apache.sh
├── install_php.sh
├── index.html
├── hello_lambda.py
└── ssh.pem
```
1. main.tf: Configuración de Terraform para aprovisionar recursos en AWS. Debera realizar los cambios necesarios, como el email de la subscription.
2. submit.php: Script PHP para manejar las solicitudes POST del formulario y publicar mensajes en el tema SNS. Recuerda cambiar el 'snsTopicArn por el tuyo correspondiente'.
3. install_apache.sh: Script de instalación y configuración de Apache.
4. install_php.sh: Script de instalación y configuración de PHP.
5. index.html: Página HTML con el formulario de contacto.
6. hello_lambda.py: Función Lambda en Python para enviar mensajes a Slack. Se debe realizar los cambios de la url por el slack donde desea enviar los mensajes.
7. ssh.pem: Clave privada para acceso SSH a la instancia EC2.
