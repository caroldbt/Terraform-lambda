
# Proyecto de Servidor Web con Apache, PHP, Lambda en Python y Slack hecha con Terraform

## Descripción
Este proyecto implementa un servidor web con Apache y PHP en una instancia EC2 de AWS. El servidor web incluye un formulario de contacto que envía datos a un tema SNS de AWS, el cual a su vez desencadena una función Lambda en Python que envía notificaciones a Slack.

## Archivos
.
├── README.md
├── main.tf
├── submit.php
├── install_apache.sh
├── install_php.sh
├── index.html
├── hello_lambda.py
└── ssh.pem
