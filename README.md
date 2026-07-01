<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Costa del Perú - Información</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
            padding: 20px;
        }

        .container {
            max-width: 900px;
            margin: 0 auto;
            background: white;
            border-radius: 20px;
            box-shadow: 0 20px 60px rgba(0,0,0,0.3);
            overflow: hidden;
        }

        .header {
            background: linear-gradient(135deg, #d91023 0%, #c41e3a 100%);
            color: white;
            padding: 40px;
            text-align: center;
            position: relative;
        }

        .header::after {
            content: '';
            position: absolute;
            bottom: -50px;
            left: 0;
            right: 0;
            height: 100px;
            background: white;
            clip-path: polygon(0 50%, 100% 0, 100% 100%, 0% 100%);
        }

        .header h1 {
            font-size: 3em;
            margin-bottom: 10px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
        }

        .header p {
            font-size: 1.2em;
            opacity: 0.9;
        }

        .content {
            padding: 40px;
        }

        .info-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            margin-bottom: 40px;
        }

        .card {
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
            padding: 25px;
            border-radius: 15px;
            border-left: 5px solid #d91023;
            transition: transform 0.3s, box-shadow 0.3s;
        }

        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 30px rgba(0,0,0,0.2);
        }

        .card h3 {
            color: #d91023;
            margin-bottom: 10px;
            font-size: 1.3em;
        }

        .card p, .card ul {
            color: #444;
            line-height: 1.6;
        }

        .card ul {
            list-style: none;
            padding-left: 0;
        }

        .card ul li {
            padding: 5px 0;
            padding-left: 20px;
            position: relative;
        }

        .card ul li::before {
            content: '🇵🇪';
            position: absolute;
            left: 0;
        }

        .map-section {
            margin-top: 40px;
        }

        .map-section h2 {
            text-align: center;
            color: #d91023;
            font-size: 2em;
            margin-bottom: 20px;
        }

        .map-container {
            position: relative;
            padding-bottom: 56.25%;
            height: 0;
            overflow: hidden;
            border-radius: 15px;
            box-shadow: 0 10px 40px rgba(0,0,0,0.2);
        }

        .map-container iframe {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            border: none;
        }

        .stats {
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
            margin: 40px 0;
            gap: 20px;
        }

        .stat-box {
            text-align: center;
            padding: 20px;
            background: #d91023;
            color: white;
            border-radius: 15px;
            min-width: 150px;
        }

        .stat-box .number {
            font-size: 2.5em;
            font-weight: bold;
        }

        .stat-box .label {
            font-size: 0.9em;
            opacity: 0.9;
        }

        .footer {
            background: #1a1a2e;
            color: white;
            text-align: center;
            padding: 20px;
            font-size: 0.9em;
        }

        @media (max-width: 600px) {
            .header h1 {
                font-size: 2em;
            }
            .content {
                padding: 20px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <h1>🇵🇪 Costa del Perú</h1>
            <p>Descubre la maravillosa región costera peruana</p>
        </div>

        <div class="content">
            <div class="stats">
                <div class="stat-box">
                    <div class="number">2,414</div>
                    <div class="label">km de costa</div>
                </div>
                <div class="stat-box">
                    <div class="number">11</div>
                    <div class="label">Regiones</div>
                </div>
                <div class="stat-box">
                    <div class="number">60%</div>
                    <div class="label">Población del país</div>
                </div>
            </div>

            <div class="info-grid">
                <div class="card">
                    <h3>🌊 Ubicación</h3>
                    <p>La costa peruana se extiende a lo largo del Océano Pacífico, desde la frontera con Ecuador (Tumbes) hasta la frontera con Chile (Tacna).</p>
                </div>

                <div class="card">
                    <h3>🌡️ Clima</h3>
                    <p>Predominantemente árido y semiárido con escasas lluvias, excepto en el norte (Tumbes y Piura) donde es tropical seco.</p>
                </div>

                <div class="card">
                    <h3>🏛️ Regiones Costeras</h3>
                    <ul>
                        <li>Tumbes</li>
                        <li>Piura</li>
                        <li>Lambayeque</li>
                        <li>La Libertad</li>
                        <li>Ancash</li>
                        <li>Lima</li>
                        <li>Callao</li>
                        <li>Ica</li>
                        <li>Arequipa</li>
                        <li>Moquegua</li>
                        <li>Tacna</li>
                    </ul>
                </div>

                <div class="card">
                    <h3>💰 Economía</h3>
                    <p>Principal centro económico del país. Actividades principales:</p>
                    <ul>
                        <li>Pesca e industria pesquera</li>
                        <li>Agricultura en valles costeros</li>
                        <li>Industria manufacturera</li>
                        <li>Comercio y servicios</li>
                        <li>Turismo</li>
                    </ul>
                </div>

                <div class="card">
                    <h3>🏙️ Ciudades Principales</h3>
                    <ul>
                        <li>Lima (Capital)</li>
                        <li>Trujillo</li>
                        <li>Chiclayo</li>
                        <li>Arequipa</li>
                        <li>Piura</li>
                        <li>Ica</li>
                        <li>Chimbote</li>
                    </ul>
                </div>

                <div class="card">
                    <h3>✨ Atractivos Turísticos</h3>
                    <ul>
                        <li>Líneas de Nazca</li>
                        <li>Huacas del Sol y Luna</li>
                        <li>Chan Chan</li>
                        <li>Huacachina</li>
                        <li>Reserva Nacional de Paracas</li>
                        <li>Playa Waikiki</li>
                        <li>Máncora</li>
                    </ul>
                </div>
            </div>

            <div class="map-section">
                <h2>🗺️ Mapa del Perú</h2>
                <div class="map-container">
                    <iframe 
                        src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d4087598.263943662!2d-81.32968359375!3d-9.189967!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x9105c850c87e5d1f%3A0x2d991b089fca71e9!2sPer%C3%BA!5e0!3m2!1ses!2spe!4v1704067200000!5m2!1ses!2spe" 
                        allowfullscreen="" 
                        loading="lazy" 
                        referrerpolicy="no-referrer-when-downgrade">
                    </iframe>
                </div>
            </div>
        </div>

        <div class="footer">
            <p>🇵🇪 Hecho con orgullo peruano | Costa del Perú 2024</p>
        </div>
    </div>
</body>
</html>
