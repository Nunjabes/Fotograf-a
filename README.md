# Fotograf-a
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mi Maqueta Web</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>Mi Maqueta Web</h1>
    </header>
    <nav>
        <ul>
            <li><a href="#">Inicio</a></li>
            <li><a href="#">Acerca de</a></li>
            <li><a href="#">Contacto</a></li>
        </ul>
    </nav>
    <main>
        <section>
            <h2>Contenido Principal</h2>
            <p>Bienvenido a mi maqueta web. Esto es el contenido principal.</p>
        </section>
    </main>
    <footer>
        <p>&copy; 2023 Mi Maqueta Web</p>
    </footer>
    <script src="script.js"></script>
</body>
</html>

/* Estilos para la maqueta web */

body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
}

header {
    background-color: #333;
    color: white;
    text-align: center;
    padding: 10px;
}

nav ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
}

nav li {
    display: inline;
    margin-right: 20px;
}

nav a {
    text-decoration: none;
    color: #333;
}

main {
    margin: 20px;
}

footer {
    background-color: #333;
    color: white;
    text-align: center;
    padding: 10px;
}

// Obtener la hora actual
var hora = new Date().getHours();

// Elemento HTML donde mostraremos el mensaje
var mensaje = document.getElementById("saludo");

// Definir el mensaje de saludo
var saludo;

if (hora < 12) {
    saludo = "Buenos días";
} else if (hora < 18) {
    saludo = "Buenas tardes";
} else {
    saludo = "Buenas noches";
}

// Mostrar el mensaje en la página web
mensaje.textContent = saludo;