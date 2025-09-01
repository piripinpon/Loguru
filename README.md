# Loguru
¿Que es loguru?
Loguru es una librería de Python diseñada para simplificar el manejo de logs y errores.
Se creó para reemplazar al módulo estándar logging, haciéndolo mucho más fácil, intuitivo y potente.
¿Para que sirve?
Registrar mensajes de tu programa (info, advertencias, errores, depuración).
Capturar errores y excepciones automáticamente con stack trace completo.
Guardar logs en archivos, con rotación automática y filtros por tamaño o tiempo.
Personalizar el formato de los logs, mostrando solo lo que te interesa.
Funciona tanto para pequeños scripts como para aplicaciones grandes.

Para explicar loguru de forma sencilla, es que, creara un archivo donde mandara el error y el stack trace completo,
lo guardara en el mismo archivo y podras ver los errores accediendo a el.

<img width="656" height="355" alt="image" src="https://github.com/user-attachments/assets/a3c2d0c4-4de9-43f6-a38c-401f47249e50" />

logger.add("errores.log", rotation="1 MB")
Este se encarga de crear el archivo, donde cuando pase de 1mb va a rotar y creara otro archivo para seguir almacenando.

try:
    ciudad = datos_usuario["ciudad"]
    print("Ciudad:", ciudad)
    
Aqui intentara acceder a una clave que no existe, donde saltara el error, creara el archivo y tendra esto en el.

<img width="831" height="414" alt="image" src="https://github.com/user-attachments/assets/f570a831-1c7f-45c4-bae1-dbba619dac92" />
El trace completo
