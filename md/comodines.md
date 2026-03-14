## Comodines

Si los parámetros son nombres de ficheros podemos utilizar caracteres comodines. Los comodines son:

!!! tip
	Asterisco (\*): **sustituye a cero o más caracteres**, Interrogante (?): **sustituye a un carácter**

Vamos a ver algunos ejemplos en los que utilizaremos el comando copy. Se trata de un comando de Windows que permite copiar archivos y al que se le pasan 2 parámetros: el primero el nombre del archivo a copiar y el segundo la ruta donde el copiaremos.

`C:\Users\sergi>copy info*.txt c:\users\sergi\prueba`

Comando de Windows que copia todos los archivos cuyo nombre empieza por "inf" seguido de cualquier carácter y la extensión es "txt" desde el directorio actual en el directorio C:\Users\sergi\prueba (copiará *inf.txt, informe.txt, informacion_junio.txt*, etc pero no *informe.doc, mi_informe.txt*, ...)

`C:\Users\sergi>copy *_junio.doc c:\users\sergi\prueba`

Comando de Windows que copia todos los archivos cuyo nombre termina por "_junio" y la extensión es "doc" desde el directorio actual en el directorio C:\Users\sergi\ prueba (copiará *informe_junio.doc, ventas_junio.doc*, etc pero no *informe_junio_clientes.doc, informe_junio.txt*, ...)

`C:\Users\sergi>copy *.* c:\users\sergi\prueba`

Comando de Windows que copia todos los archivos (con cualquier nombre y extensión) desde el directorio actual en el directorio C:\Users\sergi\prueba

`C:\Users\sergi>copy ma?o.jpg c:\users\sergi\prueba`

Comando de Windows que copia todos los archivos cuyo nombre es "ma", una letra cualquiera y "o" y la extensión es "jpg" desde el directorio actual en el directorio C:\Users\sergi (copiará mano.jpg , mazo.jpg, etc pero no marzo.jpg -2 letras- ni mao.jpg -0 letras-, ni mayo.txt por no cumplir con la extensión).