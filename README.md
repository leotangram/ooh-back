# ooh-back

Para usar este proyecto seguir los siguientes pasos:

## 1.
Clonar el poyecto.

https://raw.githubusercontent.com/leotangram/ooh-back/master/assets/images/1.png

## 2.
En la terminal usar "npm i" o "yarn install".

## 3. Iniciar la base de datos.
Para esto debes tener MongoDB instalado en tu PC. https://www.mongodb.com/download-center/community.
### En mac
Puedes usar el comando "mongod" en la terminal y dejarlo correr.
### En windows
Puedes correr el archivo mongod.exe y mongo.exe

## 4.
En la terminar usa el comando "npm start"

## 5. Postman
Cuando la base de datos y el proyecto estén corriendo, usar postman o insomnia, etc... (Yo usaré postman).
### 5.1 GET ALL PRODUCTS
Para ver el arreglo de productos usar el verbo get con la siguiente dirección: http://localhost:3000/api/product
### 5.2 POST
Para guardar un producto puedes usar la siguiente dirección: http://localhost:3000/api/product con el verbo POST, ir a la sección Body, luego seleccionar "x.wwww-form-urlencoded".
en el key escribir: name, picture, price, category, description. Y en value escribir lo que quieras teniendo en cuenta que name es de tipo string; picture es de tipo string; price es de tipo number; category es de tipo string, pero tiene una restricción: Solo puedes agregar "computers", "phones" o "accesories"; description es de tipo string.
### 5.2 PATCH
Para actualizar un producto, debes agregarle el id correspondiente al producto de esta manera en la dirección: http://localhost:3000/api/product/5ccd95a684f1f70a7fc8bb9a.
Luego cambias el campo que quieras y listo.
### 5.3 GET A PRODUCT
Para ver un producto específico debes agregar la misma url que en patch, pero con el verbo GET.
