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

                                                     Comandos Básicos de Docker 

docker run: Correr un contenedor

docker ps: Contenedores que están corriendo

(-- name serverweb): Colocar un nombre y sirve para identificar el docker y donde está corriendo

80:80: Maquina anfitriona

-d: Permite seguir ocupando la línea de comandos, si usamos el proceso pasa a segundo plano

                            Clase #2 Acceder al contenedor ejecutado y modificar el index.html
-Creamos un documento en github (documento html)
[![imagen-2022-10-24-111356115.png](https://i.postimg.cc/zDkQHdg0/imagen-2022-10-24-111356115.png)](https://postimg.cc/bdsgK9Lt)
-Regresamos a la linea de comandos y escribimos wget https://github.com/dimendieta/Tendencias-Tecnologicas/blob/main/index2.html
[![imagen-2022-10-24-112351315.png](https://i.postimg.cc/ydTXrbhd/imagen-2022-10-24-112351315.png)](https://postimg.cc/G8Hy4z5w)
-Para verificar si se descargo correctamente escribimos el comando ls
[![imagen-2022-10-24-112300998.png](https://i.postimg.cc/T1V8SG7b/imagen-2022-10-24-112300998.png)](https://postimg.cc/Pv5FvGkf)
-Ingresamos el comando docker cp index2.html nginx:/usr/share/nginx/html/index2.html (se extrae o se añade la informacion del html que se creo en el repositorio) ---> (Presionamos Open Port y ponemos el puerto 80)

                         EN CASO DE QUE NO SE EJECUTE O PRESENTE ERROR DEBERIAMOS CLONAR EL REPOSITORIO
-Ingresar el comando : git clone https://github.com/dimendieta/Tendencias-Tecnologicas
-Ingresar el comando ls para ver si se cargo
-Ejecutar el comando docker cp index2.html serverweb:/usr/share/nginx/html/index.html
[![imagen-2022-10-24-115254393.png](https://i.postimg.cc/bJ4Q7KCH/imagen-2022-10-24-115254393.png)](https://postimg.cc/FdgdcnQ7)
                                   
                          Ingresar el puerto 80 en Open Port y al final de la direccion ponemos /index2.html 
[![imagen-2022-10-24-122501655.png](https://i.postimg.cc/SxtGhTKs/imagen-2022-10-24-122501655.png)](https://postimg.cc/yDcRhTc4)
                                   



