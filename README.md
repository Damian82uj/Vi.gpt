<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Empresa Futurista</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Arial, sans-serif;
        }

        body {
            background: linear-gradient(135deg, #0f172a, #1e293b);
            color: white;
            text-align: center;
            padding: 50px 20px;
        }

        .contenedor {
            max-width: 600px;
            margin: auto;
            background: rgba(255, 255, 255, 0.1);
            padding: 20px;
            border-radius: 15px;
            box-shadow: 0px 0px 15px rgba(255, 255, 255, 0.2);
        }

        h1 {
            font-size: 28px;
            margin-bottom: 15px;
            text-transform: uppercase;
            letter-spacing: 2px;
        }

        .estadisticas {
            display: flex;
            justify-content: space-around;
            margin: 20px 0;
        }

        .caja {
            background: rgba(255, 255, 255, 0.2);
            padding: 15px;
            border-radius: 10px;
            box-shadow: 0px 0px 10px rgba(255, 255, 255, 0.3);
            width: 30%;
        }

        .numero {
            font-size: 24px;
            font-weight: bold;
            margin-top: 5px;
        }

        .instagram {
            margin-top: 20px;
            padding: 10px;
            display: inline-block;
            background: #E1306C;
            color: white;
            text-decoration: none;
            border-radius: 5px;
            font-size: 18px;
            font-weight: bold;
            transition: 0.3s;
        }

        .instagram:hover {
            background: #ff4d94;
        }
    </style>
</head>
<body>
    <div class="contenedor">
        <h1>Bienvenido a Nuestra Empresa</h1>
        <p>Información en tiempo real</p>

        <div class="estadisticas">
            <div class="caja">
                <p>Personas en la página</p>
                <div class="numero" id="personas">0</div>
            </div>
            <div class="caja">
                <p>Likes</p>
                <div class="numero" id="likes">0</div>
            </div>
            <div class="caja">
                <p>Usuarios activos</p>
                <div class="numero" id="usuarios">0</div>
            </div>
        </div>

        <a class="instagram" href="https://www.instagram.com/damian_vendedor?igsh=aW1uYzRlbWp2c2Q4" target="_blank">
            Visita mi Instagram
        </a>
    </div>

    <script>
        // Generar números falsos de forma aleatoria
        function actualizarDatos() {
            document.getElementById('personas').innerText = Math.floor(Math.random() * 500) + 50;
            document.getElementById('likes').innerText = Math.floor(Math.random() * 1000) + 200;
            document.getElementById('usuarios').innerText = Math.floor(Math.random() * 200) + 10;
        }

        actualizarDatos();
        setInterval(actualizarDatos, 5000); // Actualiza cada 5 segundos
    </script>
</body>
</html>
