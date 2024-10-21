<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ecosolar - Energía Solar</title>
    
    <!-- Bootstrap CSS -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
    
    <!-- CSS Externo -->
    <link rel="stylesheet" href="styles.css">
    
    <style>
        /* Estilo adicional para ocultar secciones por defecto */
        section {
            display: none; /* Oculta todas las secciones por defecto */
            opacity: 0; /* Inicializa la opacidad */
            transition: opacity 0.5s ease; /* Añade la transición de opacidad */
        }
        /* Muestra la sección activa */
        .active {
            display: block; /* Muestra solo la sección activa */
            opacity: 1; /* Establece la opacidad al mostrar */
        }

        /* Estilo para las imágenes de productos */
        #productos img {
            width: 80%; /* Ajusta el tamaño de las imágenes */
            border-radius: 15px; /* Bordes redondeados */
        }
    </style>
</head>
<body>

      <!-- Header con el logo de la empresa -->
      <header>
        <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
            <div class="container">
                <a class="navbar-brand" href="#" onclick="showSection('hero')"> <!-- Añadido el evento para mostrar la sección de inicio -->
                    <img src="https://media.discordapp.net/attachments/965566956575019042/1297747469412733010/IMG-20241020-WA02022.jpg?ex=67170d03&is=6715bb83&hm=bb55fe302343d2bcfdc081d974aa6fea5b3b042493da4e34f0cd19553f287f8d&=&format=webp&width=427&height=427" alt="Logo de Ecosolar" width="100">
                </a>
                <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                    <span class="navbar-toggler-icon"></span>
                </button>
                <div class="collapse navbar-collapse" id="navbarNav">
                    <ul class="navbar-nav ms-auto">
                        <li class="nav-item">
                            <a class="nav-link" href="#" onclick="showSection('productos')">Productos</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#" onclick="showSection('informacion')">Información</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#" onclick="showSection('contacto')">Contacto</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#" onclick="showSection('orden')">Orden de Pedido</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#" onclick="showSection('excel')">Excel</a>
                        </li>
                    </ul>
                </div>
            </div>
        </nav>
    </header>

    <!-- Sección Principal con imagen de paneles solares -->
    <main>
        <section id="hero" class="text-center bg-dark text-white py-5 active"> <!-- Sección activa -->
            <div class="container">
                <h1 class="display-4">Bienvenido a Ecosolar</h1>
                <p class="lead">Soluciones de energía solar para un futuro sostenible</p>
                <img src="https://media.istockphoto.com/id/1615152185/es/foto/hombre-relajado-usando-paneles-solares-en-su-casa.jpg?s=1024x1024&w=is&k=20&c=9p2YyMna3Pn3vm_YawMIRBgtQdgQ9QQqw7ZhmW6S3Hc=" class="img-fluid" alt="Imagen de paneles solares">
            </div>
        </section>

        <!-- Productos -->
        <section id="productos" class="py-5 bg-secondary text-white">
            <div class="container text-center">
                <h2 class="mb-4">Nuestros Productos</h2>
                <p>Descubre nuestros paneles solares de alta eficiencia.</p>
                <p>En Ecosolar, nos enorgullece ofrecer productos que cumplen con los más altos estándares de calidad y sostenibilidad. Nuestros paneles solares están diseñados para maximizar la captación de energía solar, adaptándose a las necesidades de hogares y empresas.</p>
                <div class="row">
                    <div class="col-md-6 mb-4">
                        <img src="https://cdn.pixabay.com/photo/2022/01/13/14/45/house-6935453_1280.jpg" class="img-fluid" alt="Panel Solar Hogareño">
                        <p>Panel Solar Hogareño (Pequeño)</p>
                    </div>
                    <div class="col-md-6 mb-4">
                        <img src="https://cdn.pixabay.com/photo/2020/03/30/20/11/solar-panels-4985353_1280.jpg" class="img-fluid" alt="Panel Solar Empresarial">
                        <p>Panel Solar Empresarial (Grande)</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Información de la Empresa -->
        <section id="informacion">
            <div class="container text-center">
                <h2>Sobre Nosotros</h2>
                <p>Ecosolar es una empresa comprometida con la sostenibilidad y la energía limpia. Ofrecemos soluciones energéticas adaptadas a las necesidades de nuestros clientes.</p>
                <p>Con un equipo de expertos en energía renovable, trabajamos incansablemente para proporcionar tecnología de punta que ayude a nuestros clientes a reducir su huella de carbono y contribuir a un planeta más saludable.</p>
            </div>
        </section>

        <!-- Contacto -->
        <section id="contacto">
            <div class="container text-center">
                <h2>Contacto</h2>
                <p>Teléfono: 11 555-1234</p>
                <p>Email: ecosolar@gmail.com</p>
                <p>Dirección: Avenida Siempreviva 742</p>
                <p>Estamos aquí para ayudarle con cualquier consulta. No dude en contactarnos para obtener más información sobre nuestros productos y servicios. Nuestro equipo está listo para atenderle.</p>
            </div>
        </section>

        <!-- Orden de Pedido -->
        <section id="orden">
            <div class="container text-center">
                <h2>Haz tu Pedido</h2>
                <p>Llena el siguiente formulario para solicitar una cotización personalizada.</p>
                <p>Su satisfacción es nuestra prioridad. Asegúrese de proporcionar toda la información necesaria para que podamos atender su solicitud de manera eficiente. Nos comprometemos a responder a su consulta en el menor tiempo posible.</p>
                <form>
                    <label for="nombre">Nombre:</label>
                    <input type="text" id="nombre" name="nombre" required class="form-control mb-3">

                    <label for="email">Email:</label>
                    <input type="email" id="email" name="email" required class="form-control mb-3">

                    <label for="producto">Producto de interés:</label>
                    <select id="producto" name="producto" class="form-control mb-3">
                        <option value="panel-standard">Panel Solar Standard</option>
                        <option value="panel-premium">Panel Solar Premium</option>
                    </select>

                    <label for="mensaje">Mensaje:</label>
                    <textarea id="mensaje" name="mensaje" class="form-control mb-3"></textarea>

                    <button type="submit" class="btn btn-primary">Enviar Pedido</button>
                </form>
            </div>
        </section>

        <!-- Sección Excel -->
        <section id="excel">
            <div class="container text-center">
                <h2>Excel</h2>
                <p>Aquí esta un cuadro de excel en el cual se puede mostrar los ingresos, saldo y gastos:</p>
                <iframe src="https://docs.google.com/spreadsheets/d/e/2PACX-1vSSwTOXZ5qCyI6zKBz65ArMIMdY6Jd5j5s5wdujWozCs7R3M4M6t5-TTVZiD8hn4v5WIJACYxBXsSBX/pubhtml" width="100%" height="500" frameborder="0"></iframe>
            </div>
        </section>
    </main>

    <!-- Footer -->
    <footer>
        <p>&copy; 2024 Ecosolar. Todos los derechos reservados.</p>
    </footer>

    <!-- JavaScript para la navegación -->
    <script>
        function showSection(sectionId) {
            // Oculta todas las secciones
            const sections = document.querySelectorAll('section');
            sections.forEach(section => {
                section.classList.remove('active'); // Remueve la clase activa
            });
            // Muestra la sección seleccionada
            const activeSection = document.getElementById(sectionId);
            activeSection.classList.add('active'); // Añade la clase activa
        }
        
        // Muestra la sección de inicio por defecto
        document.addEventListener('DOMContentLoaded', () => {
            showSection('hero');
        });
    </script>

    <!-- Bootstrap JS Bundle con Popper -->
    <script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.11.6/dist/umd/popper.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.min.js"></script>
</body>
</html>
