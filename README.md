# De número a letras

Este código te permite convertir números a letras.

## Forma de uso

Guarde el archivo ```numeroaLetras.js``` y luego utilice la función ```NumeroALetras(valor)``` pasando como parámetro el número a convertir.


## Limitantes

Este código solo puede convertir cifras desde 0.01 centavos, hasta 999 millones.

## Ejemplo práctico

```html
<!DOCTYPE html>
<html lang="es">

    <head>
        <meta http-equiv="Content-Type" content="text/html; charset=utf-8">

        <title>Convertir numeros a letras</title>

        <style>
            #numero {
                padding: 10px;
                text-align: right;
            }
        </style>
    </head>

    <body>
        <h1>Código de número a letras</h1>
        <input type="text" id="numero" placeholder="introduce un numero">
        <span id="texto"></span>

        <script src="numeroaLetras.js"></script>
        <script>
            document.getElementById("numero").addEventListener("keyup", function (e) {
                document.getElementById("texto").innerHTML = NumeroALetras(this.value);
            });
        </script>

    </body>

</html>
```
