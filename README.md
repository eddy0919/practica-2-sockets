Practica 2 - sockets

Manuel Alejandro Salazar - 1329107
Mateo Salazar Munera - 1323142
Edilberto Moreno Valencia - 1326907


Paquete Socket utils

- basics-01.py: Se crea un socket, con el cual se puede determinar el nombre del servidor donde se esta ejecutando el codigo fuente.

- basics-02.py: Muestra la funcion 'gethostbyname' la cual permite obtener la ip de un servidor dado su nombre.

- basics-03.py: Hace uso de la funcion 'getservbyport', la cual permite obtener el nombre de un servicio de red, dado el numero del puerto y nombre del protocolo que usa.


Paquete NTP Client

- basics-04.py: Hace uso de la libreria 'ntplib' para hacerle una peticion al servidor NTP(pool.ntp.org), el cual como respuesta a la peticion retornará la hora actual.

- basics-05.py: Le envia una peticion al servidor NTP sin hacer uso de librerias externas, sino realizandolo con las funciones y metodos asociados al protocolo UDP.

Paquete HTTP Client

- socket-01.py: Se crea un socket TCP e informa si se creo correctamente o se presentó algún error.

- socket-02.py: Se crea un socket TCP, luego se hace uso de la funcion 'gethostmyname' para mostrar la direccion ip de 'www.google.com'.

- socket-03.py: Se crea un socket TCP, luego se hace uso de la funcion 'gethostmyname' para mostrar la direccion ip de 'www.google.com'. Además se hace uso del metodo 'connect' para conectar el socket TCP con el servidor de 'www.google.com'.

- socket-04.py: Se crea un socket TCP, luego se hace uso de la funcion 'gethostmyname' para mostrar la direccion ip de 'www.google.com'. Se hace uso del metodo 'connect' para conectar el socket TCP con el servidor de 'www.google.com'. Y posteriormente se envia una petición HTTP por medio del socket TCP haciendo uso del metodo 'sendall'.

- socket-05.py: Se crea un socket TCP, luego se hace uso de la funcion 'gethostmyname' para mostrar la direccion ip de 'www.google.com'. Se hace uso del metodo 'connect' para conectar el socket TCP con el servidor de 'www.google.com'. Y posteriormente se envia una petición HTTP por medio del socket TCP haciendo uso del metodo 'sendall'. Por último se hace uso de la funcion 'recv' para recibir la respuesta del servidor 'www.google.com' a la peticion HTTP.

Paquete Socket server

- server-01.py:

- server-02.py:

- server-03.py:

- server-04.py:

- server-05.py:
