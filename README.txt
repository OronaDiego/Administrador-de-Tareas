Pasos para utilizar la APP

1)-Abrir la terminal, posicionarse en el proyecto que tiene que estar ubicado en la carpeta htdocs en XAMPP
que es el paquete que yo use para gestionar la BDD y el servidor 

2)- tendras que generar tu propia base de datos para que la app pueda guardar las tareas en una BDD y despues poder borrarlas. 

3)-Pasos para crear la BDD y configurarla
        *abrir XAMPP -> Admin -> nos abre una url donde nos muestra nuestras BDD
        *crear la base de datos, dandole el nombre de app (o el que prefieras yo use ese)
        *En el archivo .env modificar los datos necesarios como: 
            -DB_CONNECTION=mysql
            -DB_HOST= (tu host)
            -DB_PORT=(tu port)
            -DB_DATABASE=(nombre de la base creado anteriormente --app-)
            -DB_USERNAME=root
            -DB_PASSWORD=

        *usamos el comando (php artisan migrate) para migrar esos datos y crear la coneccion con la BDD.

4)-usamos el comando php artisan server para levantar un servidor y nos va a dar la ruta de acceso en el localHost donde podemos probar la App

5)-Todos estos pasos contemplan que ya tienes instalado XAMPP,LARAVEL,PHP,Composer con sus correspondientes versiones