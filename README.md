# Tendencias-Tecnologicas
                                    Clase #1 Ejecutar comando docker para ejecutar una instancia servidor web nginx.
-Crear una cuenta en Docker Hub
[![imagen-2022-10-24-105055265.png](https://i.postimg.cc/BQh0x72q/imagen-2022-10-24-105055265.png)](https://postimg.cc/zVR6NjdM)
-Ingresar en Play with Docker
[![imagen-2022-10-24-104431975.png](https://i.postimg.cc/gcB3Xmr4/imagen-2022-10-24-104431975.png)](https://postimg.cc/z3Ky4mCR)
-Ingresar el comando : docker run --name nginx -p 80:80 -d nginx 
(Se carga las librerias y el servidor virtual)
[![imagen-2022-10-24-104829774.png](https://i.postimg.cc/x8SGCP6H/imagen-2022-10-24-104829774.png)](https://postimg.cc/62Y4bCJ5)
-Para verificar si el servidor esta funcionando se coloca docker ps -a
[![imagen-2022-10-24-105529626.png](https://i.postimg.cc/YS0zy3nf/imagen-2022-10-24-105529626.png)](https://postimg.cc/67sZ8dNy)

                                                     Comando Básico de Docker 

docker run: Correr un contenedor

docker ps: Contenedores que están corriendo

(-- name serverweb): Colocar un nombre y sirve para identificar el docker y donde está corriendo

80:80: Maquina anfitriona

-d: Permite seguir ocupando la línea de comandos, si usamos el proceso pasa a segundo plano

                                     Clase #2 Acceder al contenedor ejecutado y modificar el index.html


