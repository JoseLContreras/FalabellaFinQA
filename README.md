# FalabellaFinQA

Instrucciones

•	Descargar el código fuente desde https://github.com/JoseLContreras/FalabellaFinQA e importar en Postman la colección incluida en el repositorio con el nombre
de Test.postman_collection_JLC.json

•	Para ejecutar el código como requisito la máquina debe tener instalado
node.js luego los comandos `npm install` y `npm start` dejarán corriendo un
servidor local, el cual levanta una API REST.

El objetivo de la prueba es realizar un test automatizado que cree un usuario y luego verifique que dicho usuario fue creado con un campo adicional uuid. Dicho test fue creado con la funcionalidad de test Postman, se incluye una imagen de la colección con la entrada y la salida a testear, la cual ya esta incluida en el código.
Poner atención de que se debe dejar corriendo el método POST con el firstname, lastname y age  a incluir y luego hacer la misma consulta en el método GET (es indiferente si sigue haciendo “sending” el método POST.) En el GET vienen incluidas las siguientes pruebas (con assertions en javascript):

1.	Status OK
2.	El tiempo de Response es menor de 1000ms
3.	Existe propiedad lastName
4.	Existe propiedad firstMame
5.	Existe propiedad age
6.	Existe propiedad id
7.	Estado 200



![metodos](https://user-images.githubusercontent.com/39358933/127361358-5495b3d6-7732-4bf9-99b2-7e66a8cc8f90.PNG)

Paso 1: Insertar (POST) datos requeridos en JSON.

![1step](https://user-images.githubusercontent.com/39358933/127361121-4940e717-4c5a-4e1b-81fd-0162b67d1de0.PNG)

Paso 2: Validación de escritura eb BD.

![2step](https://user-images.githubusercontent.com/39358933/127361165-17e785b5-2077-45df-889d-e25772c4570c.PNG)

Paso 3: Obtener (GET) datos con el uuid incluido en el response del body, inyectando JSON anterior.

![3step](https://user-images.githubusercontent.com/39358933/127361186-161991cf-a406-42c6-94f0-1ebf42fafad8.PNG)

Paso 4: Validación de los test contemplados en el GET.

![4step-test](https://user-images.githubusercontent.com/39358933/127361207-67b14fb1-f49e-48bb-b118-4b5cb0bcd81b.PNG)

