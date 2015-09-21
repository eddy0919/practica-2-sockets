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

- server-01.py: Se crea un socket TCP y luego se hace uso del metodo 'bind' para asociar el socket a un ip y un puerto.

- server-02.py: Se crea un socket TCP y luego se hace uso del metodo 'bind' para asociar el socket a un ip y un puerto. Luego se hace uso del metodo 'listen' para limitar el numero de conexiones posibles a ese socket, finalemente se espera por una conexion con el metodo 'accept' el cual bloqueara la ejecucion del programa, hasta que no se acepte una conexion.

- server-03.py: Se crea un socket TCP y luego se hace uso del metodo 'bind' para asociar el socket a un ip y un puerto. Se hace uso del metodo 'listen' para limitar el numero de conexiones posibles a ese socket, luego se espera por una conexion con el metodo 'accept' el cual bloqueara la ejecucion del programa, hasta que no se acepte una conexion. Y finalmente se guarda el mensaje enviado por el cliente con el metodo 'recv' y se reenvia al cliente con el metodo 'sendall'.

- server-04.py: Se crea un socket TCP y luego se hace uso del metodo 'bind' para asociar el socket a un ip y un puerto. Se hace uso del metodo 'listen' para limitar el numero de conexiones posibles a ese socket. Posteriormente se abre un ciclo para recibir conexiones las cuales se aceptan por medio del metodo 'accept', el ciclo permite que el servidor reciba hasta 10 conexiones, solo una al tiempo, siempre y cuando ninguno de los clientes le envie al sevidor un mensaje vacio.

- server-05.py: Se crea un socket TCP y luego se hace uso del metodo 'bind' para asociar el socket a un ip y un puerto. Se hace uso del metodo 'listen' para limitar el numero de conexiones posibles a ese socket. Posteriormente se abre un ciclo de escucha de clientes con el cual se van a aceptar conexiones de clientes y para cada uno se le va a asociar un hilo con la comunicacion a ese cliente en especifico. El hilo asociado al cliente se crea haciendo uso de la funcion 'start_new_thread' a la cual se le debe pasar una funcion creada por el programador que en este caso es 'clientthread'. clientthread, es una funcion que permite crear un ciclo de escucha de mensajes para un cliente en especifico.

- 


