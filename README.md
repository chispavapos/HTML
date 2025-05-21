<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ChispaVapos - ELFBAR ICE KING 40K</title>
    <style>
        /* Estilos actualizados */
        body {
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 0;
            background-color: #f5f5f5;
            color: #333;
        }
        
        header {
            background-color: #1a1a2e;
            color: white;
            padding: 1.5rem 0;
            text-align: center;
        }
        
        .logo {
            font-size: 2.5rem;
            font-weight: bold;
            color: #e94560;
            margin-bottom: 0.5rem;
        }
        
        .age-verification {
            background-color: #e94560;
            color: white;
            padding: 1.5rem;
            text-align: center;
            display: none;
            border-radius: 5px;
            margin: 1rem auto;
            max-width: 600px;
        }
        
        nav {
            background-color: #16213e;
            padding: 0.8rem;
        }
        
        nav ul {
            list-style: none;
            padding: 0;
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
        }
        
        nav ul li {
            margin: 0 1.5rem;
        }
        
        nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: bold;
            transition: color 0.3s;
        }
        
        nav ul li a:hover {
            color: #e94560;
        }
        
        .products {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
            gap: 1.5rem;
            padding: 2rem;
            max-width: 1200px;
            margin: 0 auto;
        }
        
        .product-card {
            background: white;
            border: 1px solid #ddd;
            border-radius: 8px;
            padding: 1.5rem;
            text-align: center;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
            transition: transform 0.3s;
        }
        
        .product-card:hover {
            transform: translateY(-5px);
        }
        
        .product-card img {
            max-width: 100%;
            height: 180px;
            object-fit: contain;
            margin-bottom: 1rem;
        }
        
        .flavor-badge {
            display: inline-block;
            background-color: #e94560;
            color: white;
            padding: 0.3rem 0.6rem;
            border-radius: 20px;
            font-size: 0.8rem;
            margin: 0.3rem;
        }
        
        .price {
            font-weight: bold;
            color: #e94560;
            font-size: 1.4rem;
            margin: 0.5rem 0;
        }
        
        .promo {
            background-color: #16213e;
            color: white;
            padding: 0.5rem;
            border-radius: 5px;
            margin: 0.5rem 0;
            font-weight: bold;
        }
        
        button {
            background-color: #e94560;
            color: white;
            border: none;
            padding: 0.7rem 1.5rem;
            border-radius: 5px;
            cursor: pointer;
            font-weight: bold;
            transition: background-color 0.3s;
            margin-top: 0.5rem;
        }
        
        button:hover {
            background-color: #d13354;
        }
        
        .whatsapp-button {
            background-color: #25D366;
            display: inline-flex;
            align-items: center;
            justify-content: center;
            gap: 0.5rem;
        }
        
        .whatsapp-button:hover {
            background-color: #128C7E;
        }
        
        footer {
            background-color: #1a1a2e;
            color: white;
            text-align: center;
            padding: 1.5rem;
            margin-top: 2rem;
        }
        
        .warning {
            background-color: #f39c12;
            color: white;
            padding: 1rem;
            text-align: center;
            font-size: 0.9rem;
            margin: 1rem auto;
            max-width: 1200px;
            border-radius: 5px;
        }
        
        .contact-info {
            background-color: white;
            padding: 2rem;
            text-align: center;
            margin: 1rem auto;
            max-width: 600px;
            border-radius: 8px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }
        
        .contact-info a {
            color: #e94560;
            text-decoration: none;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <!-- Verificación de edad -->
    <div class="age-verification" id="ageVerification">
        <h2>VERIFICACIÓN DE EDAD</h2>
        <p>Para acceder a ChispaVapos, debes ser mayor de 18 años.</p>
        <div style="display: flex; justify-content: center; gap: 1rem; margin-top: 1rem;">
            <button onclick="verifyAge(true)">SOY MAYOR DE 18 AÑOS</button>
            <button onclick="verifyAge(false)">SOY MENOR DE EDAD</button>
        </div>
    </div>
    
    <!-- Contenido principal -->
    <div id="mainContent" style="display: none;">
        <header>
            <div class="logo">CHISPAVAPOS</div>
            <p>Vapeadores Premium en Buenos Aires</p>
        </header>
        
        <nav>
            <ul>
                <li><a href="#productos">PRODUCTOS</a></li>
                <li><a href="#sabores">SABORES</a></li>
                <li><a href="#contacto">CONTACTO</a></li>
            </ul>
        </nav>
        
        <div class="warning">
            <p>ADVERTENCIA: Este producto contiene nicotina. La nicotina es un alcaloide adictivo. No recomendado para no fumadores. Prohibida su venta a menores de 18 años.</p>
        </div>
        
        <section id="productos" class="products">
            <div class="product-card">
                <img src="https://via.placeholder.com/300x300?text=ELFBAR+ICE+KING+40K" alt="ELFBAR ICE KING 40K">
                <h2>ELFBAR ICE KING 40K</h2>
                <p>Dispositivo desechable premium con hasta 40.000 puffs</p>
                
                <div class="price">$26.000 ARS</div>
                <div class="promo">¡PROMO! 2 por $50.000 ARS</div>
                
                <button class="whatsapp-button" onclick="openWhatsApp()">
                    <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" viewBox="0 0 16 16">
                        <path d="M13.601 2.326A7.854 7.854 0 0 0 7.994 0C3.627 0 .068 3.558.064 7.926c0 1.399.366 2.76 1.057 3.965L0 16l4.204-1.102a7.933 7.933 0 0 0 3.79.965h.004c4.368 0 7.926-3.558 7.93-7.93A7.898 7.898 0 0 0 13.6 2.326zM7.994 14.521a6.573 6.573 0 0 1-3.356-.92l-.24-.144-2.494.654.666-2.433-.156-.251a6.56 6.56 0 0 1-1.007-3.505c0-3.626 2.957-6.584 6.591-6.584a6.56 6.56 0 0 1 4.66 1.931 6.557 6.557 0 0 1 1.928 4.66c-.004 3.639-2.961 6.592-6.592 6.592zm3.615-4.934c-.197-.099-1.17-.578-1.353-.646-.182-.065-.315-.099-.445.099-.133.197-.513.646-.627.775-.114.133-.232.148-.43.05-.197-.1-.836-.308-1.592-.985-.588-.525-.985-1.175-1.103-1.372-.114-.198-.011-.304.088-.403.087-.088.197-.232.296-.346.1-.114.133-.198.198-.33.065-.134.034-.248-.015-.347-.05-.099-.445-1.076-.612-1.47-.16-.389-.323-.335-.445-.34-.114-.007-.247-.007-.38-.007a.729.729 0 0 0-.529.247c-.182.198-.691.677-.691 1.654 0 .977.71 1.916.81 2.049.098.133 1.394 2.132 3.383 2.992.47.205.84.326 1.129.418.475.152.904.129 1.246.08.38-.058 1.171-.48 1.338-.943.164-.464.164-.86.114-.943-.049-.084-.182-.133-.38-.232z"/>
                    </svg>
                    COMPRAR POR WHATSAPP
                </button>
            </div>
        </section>
        
        <section id="sabores" style="padding: 2rem; max-width: 1200px; margin: 0 auto;">
            <h2 style="text-align: center; margin-bottom: 1.5rem;">SABORES DISPONIBLES</h2>
            <div style="display: flex; flex-wrap: wrap; justify-content: center; gap: 0.5rem;">
                <span class="flavor-badge">CHERRY FUSE</span>
                <span class="flavor-badge">STRAWBERRY ICE</span>
                <span class="flavor-badge">WATERMELON ICE</span>
                <span class="flavor-badge">GRAPE ICE</span>
                <span class="flavor-badge">STRAWBERRY WATERMELON</span>
                <span class="flavor-badge">STRAWBERRY DRAGONFRUIT</span>
                <span class="flavor-badge">DOUBLE APPLE ICE</span>
                <span class="flavor-badge">MIAMI MINT</span>
                <span class="flavor-badge">MANGO MAGIC</span>
                <span class="flavor-badge">PEACH</span>
                <span class="flavor-badge">CHERRY STRAZZ</span>
                <span class="flavor-badge">GREEN APPLE ICE</span>
            </div>
        </section>
        
        <section id="contacto" class="contact-info">
            <h2>CONTACTO</h2>
            <p>Realizá tu pedido directamente por WhatsApp:</p>
            <p style="font-size: 1.2rem; margin: 1rem 0;">
                <a href="https://wa.me/541127141148" target="_blank">11 2714-1148</a>
            </p>
            <p>Horario de atención: Lunes a Viernes de 10:00 a 20:00 hs</p>
            <p>Envíos a todo Buenos Aires</p>
        </section>
        
        <footer>
            <p>&copy; 2023 CHISPAVAPOS. Todos los derechos reservados.</p>
            <p style="font-size: 0.8rem; margin-top: 0.5rem;">Venta exclusiva para mayores de 18 años. Al realizar una compra, declarás que cumplís con los requisitos de edad.</p>
        </footer>
    </div>
    
    <script>
        // Verificación de edad
        document.addEventListener('DOMContentLoaded', function() {
            document.getElementById('ageVerification').style.display = 'block';
        });
        
        function verifyAge(isAdult) {
            if (isAdult) {
                document.getElementById('ageVerification').style.display = 'none';
                document.getElementById('mainContent').style.display = 'block';
                // Guardar en localStorage que el usuario verificó su edad
                localStorage.setItem('ageVerified', 'true');
            } else {
                window.location.href = 'https://www.google.com';
            }
        }
        
        // Verificar si ya había confirmado edad
        if (localStorage.getItem('ageVerified') === 'true') {
            document.getElementById('ageVerification').style.display = 'none';
            document.getElementById('mainContent').style.display = 'block';
        }
        
        // Función para WhatsApp
        function openWhatsApp() {
            const message = encodeURIComponent(`Hola ChispaVapos! Estoy interesado en comprar ELFBAR ICE KING 40K. Sabores: `);
            window.open(`https://wa.me/541127141148?text=${message}`, '_blank');
        }
        
        // Botones de compra
        document.querySelectorAll('.whatsapp-button').forEach(button => {
            button.addEventListener('click', openWhatsApp);
        });
    </script>
</body>
</html>