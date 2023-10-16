<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Leer archivos JSON desde GitHub</title>
</head>
<body>
    <h1>Leer archivos JSON desde GitHub</h1>
    <p>Este es un ejemplo de cómo leer archivos JSON que están alojados en el mismo repositorio de GitHub.</p>

    <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.6.0/jquery.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/json5/2.2.0/json5.min.js"></script>

    <script>
        $(document).ready(function() {
            // Obtenemos la ruta del archivo JSON
            var rutaArchivo = "archivos/datos.json";

            // Leemos el archivo JSON
            $.getJSON(rutaArchivo, function(datos) {
                // Imprimimos los datos del archivo JSON
                console.log(datos);
            });
        });
    </script>
</body>
</html>
