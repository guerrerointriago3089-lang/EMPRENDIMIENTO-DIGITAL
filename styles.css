<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Vesta Aura Boutique - Emprendimiento Digital</title>
    <!-- Tailwind CSS para el diseño premium y fluido -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Google Fonts: Inter -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
    <!-- FontAwesome para iconos limpios de e-commerce -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        body {
            font-family: 'Inter', sans-serif;
            scroll-behavior: smooth;
        }
        /* Animaciones personalizadas */
        .fade-in {
            animation: fadeIn 0.4s ease-out forwards;
        }
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }
        .pulse-live {
            animation: pulseLive 1.5s infinite;
        }
        @keyframes pulseLive {
            0%, 100% { opacity: 1; }
            50% { opacity: 0.4; }
        }
    </style>
</head>
<body class="bg-slate-50 text-slate-800 flex flex-col min-h-screen">

    <!-- CABECERA Y NAVEGACIÓN -->
    <header class="bg-white/80 backdrop-blur-md sticky top-0 z-40 border-b border-slate-100 transition-all duration-300">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex items-center justify-between h-20">
                
                <!-- Logo inspirado en Emprendimiento Digital -->
                <div class="flex items-center gap-3">
                    <div class="bg-gradient-to-r from-purple-600 to-pink-500 text-white p-2.5 rounded-xl shadow-md">
                        <i class="fa-solid fa-shirt text-xl"></i>
                    </div>
                    <div>
                        <span class="text-xl font-extrabold tracking-tight bg-gradient-to-r from-purple-600 to-pink-500 bg-clip-text text-transparent">VESTA AURA</span>
                        <p class="text-[10px] text-slate-400 font-semibold uppercase tracking-wider">Digital Boutique</p>
                    </div>
                </div>

                <!-- Menú de Navegación de Escritorio -->
                <nav class="hidden md:flex space-x-8 text-sm font-medium">
                    <button onclick="changeTab('catalog')" class="nav-btn text-purple-600 hover:text-purple-700 transition" id="nav-catalog">Catálogo</button>
                    <button onclick="changeTab('live')" class="nav-btn text-slate-600 hover:text-purple-600 transition flex items-center gap-1.5" id="nav-live">
                        <span class="h-2 w-2 rounded-full bg-red-500 pulse-live"></span> Live Shopping
                    </button>
                    <button onclick="changeTab('vip')" class="nav-btn text-slate-600 hover:text-purple-600 transition" id="nav-vip">Club VIP</button>
                    <button onclick="changeTab('tracking')" class="nav-btn text-slate-600 hover:text-purple-600 transition" id="nav-tracking">Logística & Envíos</button>
                    <button onclick="changeTab('affiliates')" class="nav-btn text-slate-600 hover:text-purple-600 transition" id="nav-affiliates">Afiliados</button>
                </nav>

                <!-- Acciones Rápidas (Búsqueda, Carrito) -->
                <div class="flex items-center gap-4">
                    <!-- Botón Carrito -->
                    <button onclick="toggleCartDrawer()" class="relative p-2.5 bg-slate-100 hover:bg-slate-200 text-slate-700 rounded-xl transition">
                        <i class="fa-solid fa-bag-shopping text-lg"></i>
                        <span id="cart-count" class="absolute -top-1.5 -right-1.5 bg-purple-600 text-white text-[11px] font-bold h-5 w-5 rounded-full flex items-center justify-center border-2 border-white scale-100 transition-transform duration-300">0</span>
                    </button>
                    
                    <!-- Botón Menú Móvil -->
                    <button onclick="toggleMobileMenu()" class="md:hidden p-2 text-slate-600 hover:text-purple-600 focus:outline-none">
                        <i class="fa-solid fa-bars text-xl" id="menu-icon"></i>
                    </button>
                </div>
            </div>
        </div>

        <!-- Menú Móvil Expandido -->
        <div id="mobile-menu" class="hidden md:hidden bg-white border-b border-slate-100 py-4 px-6 space-y-3">
            <button onclick="changeTab('catalog'); toggleMobileMenu()" class="block w-full text-left py-2 font-medium text-slate-700 hover:text-purple-600">Catálogo</button>
            <button onclick="changeTab('live'); toggleMobileMenu()" class="block w-full text-left py-2 font-medium text-slate-700 hover:text-purple-600 flex items-center gap-2">
                <span class="h-2 w-2 rounded-full bg-red-500 pulse-live"></span> Venta Flash En Vivo
            </button>
            <button onclick="changeTab('vip'); toggleMobileMenu()" class="block w-full text-left py-2 font-medium text-slate-700 hover:text-purple-600">Membresía VIP</button>
            <button onclick="changeTab('tracking'); toggleMobileMenu()" class="block w-full text-left py-2 font-medium text-slate-700 hover:text-purple-600">Seguimiento de Logística</button>
            <button onclick="changeTab('affiliates'); toggleMobileMenu()" class="block w-full text-left py-2 font-medium text-slate-700 hover:text-purple-600">Programa de Afiliados</button>
        </div>
    </header>

    <!-- NOTIFICADOR MODERNO -->
    <div id="toast" class="fixed bottom-6 right-6 z-50 bg-slate-900 text-white px-5 py-3.5 rounded-2xl shadow-xl flex items-center gap-3 transition-all duration-300 transform translate-y-24 opacity-0 pointer-events-none">
        <span class="p-1 bg-green-500 rounded-full text-white text-xs"><i class="fa-solid fa-check px-0.5"></i></span>
        <span id="toast-msg" class="text-sm font-medium">Producto añadido al carrito</span>
    </div>

    <!-- NOTA DE RESPALDO TEÓRICO (PROYECTO DE EMPRENDIMIENTO DIGITAL) -->
    <div class="bg-gradient-to-r from-purple-100 via-pink-50 to-purple-50 py-3 px-4 border-b border-purple-100 text-center text-xs text-purple-800 font-medium flex flex-wrap justify-center items-center gap-2">
        <span class="bg-purple-600 text-white font-bold px-2 py-0.5 rounded-full text-[10px]">DISEÑO CONCEPTUAL</span>
        <span>Basado en apuntes del <b>09 de julio de 2026</b> sobre Emprendimiento Digital de Esmeraldas (imagen_a8779d.jpg)</span>
        <span class="text-slate-400 hidden sm:inline">|</span>
        <span class="text-slate-600">Catálogo • Carrito • Pasarela • Seguridad • Logística • Monetizaciones Avanzadas</span>
    </div>

    <!-- CONTENIDO PRINCIPAL -->
    <main class="flex-grow">
        
        <!-- SECCIÓN: CATALOGO (DEFAULT) -->
        <section id="tab-catalog" class="tab-content fade-in">
            <!-- Hero Banner -->
            <div class="relative bg-slate-900 overflow-hidden min-h-[360px] sm:min-h-[420px] flex items-center">
                <div class="absolute inset-0 z-0 opacity-40 mix-blend-overlay">
                    <img src="https://images.unsplash.com/photo-1441986300917-64674bd600d8?auto=format&fit=crop&w=1500&q=80" alt="Boutique Banner" class="w-full h-full object-cover" onerror="this.src='https://placehold.co/1200x500/1e293b/ffffff?text=Premium+Collection'">
                </div>
                <!-- Círculos decorativos de fondo -->
                <div class="absolute -top-24 -left-24 w-96 h-96 bg-purple-500 rounded-full filter blur-3xl opacity-30"></div>
                <div class="absolute -bottom-24 -right-24 w-96 h-96 bg-pink-500 rounded-full filter blur-3xl opacity-30"></div>

                <div class="relative max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 z-10 py-12 text-white">
                    <span class="inline-block bg-purple-600/30 backdrop-blur-md border border-purple-400/40 text-purple-200 text-xs font-bold px-3 py-1.5 rounded-full mb-4 tracking-wide uppercase">Temporada Verano-Otoño 2026</span>
                    <h1 class="text-4xl sm:text-6xl font-black tracking-tight leading-none mb-4">La revolución de la<br><span class="bg-gradient-to-r from-purple-400 to-pink-300 bg-clip-text text-transparent">moda inteligente</span></h1>
                    <p class="text-slate-300 text-base sm:text-lg max-w-xl mb-8 leading-relaxed">Explora diseños premium fabricados con materiales sustentables de la más alta calidad y equipados con pasarela digital ultra segura.</p>
                    <div class="flex flex-wrap gap-4">
                        <a href="#catalogo-seccion" class="bg-white text-slate-900 font-bold px-7 py-3.5 rounded-xl shadow-lg hover:shadow-white/10 hover:bg-slate-100 transition duration-300">Ver Catálogo</a>
                        <button onclick="changeTab('live')" class="bg-red-600 hover:bg-red-700 text-white font-bold px-7 py-3.5 rounded-xl shadow-lg transition duration-300 flex items-center gap-2">
                            <span class="h-2.5 w-2.5 rounded-full bg-white pulse-live"></span> Venta en Vivo
                        </button>
                    </div>
                </div>
            </div>

            <!-- Área de Catálogo -->
            <div id="catalogo-seccion" class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-12">
                <div class="flex flex-col md:flex-row md:items-center justify-between gap-6 mb-10">
                    <div>
                        <h2 class="text-3xl font-extrabold text-slate-900 tracking-tight">Colección Exclusiva</h2>
                        <p class="text-slate-500 mt-1">Filtra por categorías y encuentra tu look ideal.</p>
                    </div>
                    
                    <!-- Barra de Búsqueda Interactiva -->
                    <div class="relative w-full md:w-80">
                        <i class="fa-solid fa-magnifying-glass absolute left-4 top-3.5 text-slate-400"></i>
                        <input oninput="filterProducts()" id="search-input" type="text" placeholder="Buscar prenda..." class="w-full pl-11 pr-4 py-3 bg-white border border-slate-200 rounded-xl focus:outline-none focus:ring-2 focus:ring-purple-500 focus:border-purple-500 text-sm shadow-sm transition">
                    </div>
                </div>

                <!-- Categorías de Ropa -->
                <div class="flex flex-wrap gap-2.5 mb-8">
                    <button onclick="filterCategory('all')" id="cat-all" class="cat-pill bg-purple-600 text-white font-bold px-5 py-2.5 rounded-xl text-sm transition shadow-sm">Todos</button>
                    <button onclick="filterCategory('formal')" id="cat-formal" class="cat-pill bg-white hover:bg-slate-100 text-slate-700 font-semibold px-5 py-2.5 rounded-xl text-sm border border-slate-200/80 transition shadow-sm">Formal</button>
                    <button onclick="filterCategory('casual')" id="cat-casual" class="cat-pill bg-white hover:bg-slate-100 text-slate-700 font-semibold px-5 py-2.5 rounded-xl text-sm border border-slate-200/80 transition shadow-sm">Casual</button>
                    <button onclick="filterCategory('deportivo')" id="cat-deportivo" class="cat-pill bg-white hover:bg-slate-100 text-slate-700 font-semibold px-5 py-2.5 rounded-xl text-sm border border-slate-200/80 transition shadow-sm">Deportivo</button>
                    <button onclick="filterCategory('accesorios')" id="cat-accesorios" class="cat-pill bg-white hover:bg-slate-100 text-slate-700 font-semibold px-5 py-2.5 rounded-xl text-sm border border-slate-200/80 transition shadow-sm">Accesorios</button>
                </div>

                <!-- Cuadrícula de Productos -->
                <div id="product-grid" class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-8">
                    <!-- Los productos se inyectan dinámicamente mediante JS -->
                </div>
            </div>
        </section>

        <!-- SECCIÓN: LIVE SHOPPING (VENTA FLASH - BASADO EN APUNTES) -->
        <section id="tab-live" class="tab-content hidden fade-in max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-12">
            <div class="bg-gradient-to-r from-purple-900 to-indigo-900 rounded-3xl p-6 sm:p-10 text-white shadow-xl overflow-hidden relative mb-12">
                <!-- Decoración -->
                <div class="absolute right-0 top-0 w-80 h-80 bg-pink-500 rounded-full filter blur-[100px] opacity-20"></div>
                
                <div class="relative z-10 flex flex-col lg:flex-row gap-10 items-center">
                    <!-- Simulación de Video Streaming -->
                    <div class="w-full lg:w-3/5 bg-slate-950 rounded-2xl aspect-video overflow-hidden border border-purple-500/30 relative shadow-2xl flex flex-col justify-between p-4">
                        <!-- Animación del host de la pasarela digital -->
                        <div class="absolute inset-0 bg-gradient-to-tr from-purple-950/70 via-indigo-900/60 to-slate-950 flex items-center justify-center">
                            <!-- Visualizador de ondas de audio y mockup de pasarela en vivo -->
                            <div class="text-center p-6">
                                <div class="relative inline-block mb-4">
                                    <div class="absolute inset-0 bg-purple-500 rounded-full blur-xl opacity-60 scale-125 pulse-live"></div>
                                    <div class="relative bg-gradient-to-r from-purple-600 to-pink-500 p-6 rounded-full inline-flex items-center justify-center text-3xl">
                                        <i class="fa-solid fa-video text-white animate-bounce"></i>
                                    </div>
                                </div>
                                <h3 class="text-2xl font-black mb-1">MÉTRICAS & PASARELA DE MODA DIGITAL</h3>
                                <p class="text-purple-200 text-sm max-w-md mx-auto">Nuestros presentadores están modelando los conjuntos de temporada en vivo. Selecciona las piezas abajo.</p>
                                
                                <!-- Simulación de chat -->
                                <div class="mt-6 text-left max-w-xs mx-auto space-y-1.5 text-xs bg-black/40 p-3 rounded-xl border border-white/10">
                                    <p class="text-purple-300"><strong class="text-white">Sofía_M:</strong> ¿Tienen la chaqueta denim en talla M?</p>
                                    <p class="text-pink-300"><strong class="text-white">Carlos_Digital:</strong> ¡Ese saco ejecutivo se ve espectacular!</p>
                                    <p class="text-green-300"><strong class="text-white">Host Aura:</strong> ¡Hola! Sí, la chaqueta cuenta con stock en todas las tallas.</p>
                                </div>
                            </div>
                        </div>

                        <!-- Barra Superior del Streaming -->
                        <div class="z-10 flex justify-between items-center w-full">
                            <span class="bg-red-600 text-white text-[11px] font-bold px-3 py-1 rounded-full flex items-center gap-1.5 tracking-wider uppercase shadow-md pulse-live">
                                <span class="h-2 w-2 rounded-full bg-white"></span> EN VIVO
                            </span>
                            <span class="bg-black/50 backdrop-blur-md text-white text-xs px-2.5 py-1 rounded-full flex items-center gap-1.5">
                                <i class="fa-solid fa-eye"></i> <span id="viewers-count">1,248</span> viéndolo ya
                            </span>
                        </div>

                        <!-- Barra Inferior del Streaming -->
                        <div class="z-10 w-full flex justify-between items-end bg-gradient-to-t from-black/80 to-transparent p-4 -mx-4 -mb-4 rounded-b-2xl">
                            <div>
                                <h4 class="font-bold text-base">Colección de Pasarela 2026</h4>
                                <p class="text-xs text-slate-300">Descuentos exclusivos solo durante la transmisión</p>
                            </div>
                            <!-- Cronómetro de la Venta Flash -->
                            <div class="bg-white/15 backdrop-blur-md px-3.5 py-1.5 rounded-xl border border-white/10 text-right">
                                <p class="text-[9px] uppercase tracking-wider text-purple-200 font-bold">Cierra en:</p>
                                <p class="font-mono text-sm font-black text-pink-300" id="live-timer">29:45</p>
                            </div>
                        </div>
                    </div>

                    <!-- Productos que aparecen en la transmisión actual -->
                    <div class="w-full lg:w-2/5 flex flex-col justify-between self-stretch">
                        <div>
                            <span class="text-pink-400 font-extrabold uppercase tracking-widest text-xs">Venta Flash de la Semana</span>
                            <h2 class="text-3xl font-black mt-1 mb-4 leading-none">Compra el Look de Pasarela</h2>
                            <p class="text-slate-300 text-sm mb-6 leading-relaxed">Adquiere de forma directa las prendas más destacadas que se están mostrando en la pasarela virtual en este momento, con un <b>15% de descuento directo</b>.</p>
                        </div>

                        <!-- Lista de productos de pasarela -->
                        <div class="space-y-4 mb-6">
                            <!-- Producto En Vivo 1 -->
                            <div class="flex items-center gap-4 bg-slate-800/50 p-3 rounded-2xl border border-white/10 hover:border-purple-500/40 transition">
                                <img src="https://images.unsplash.com/photo-1539109136881-3be0616acf4b?auto=format&fit=crop&w=300&q=80" alt="Saco" class="w-16 h-16 object-cover rounded-xl" onerror="this.src='https://placehold.co/100x100'">
                                <div class="flex-grow">
                                    <span class="text-[10px] text-pink-400 font-bold uppercase tracking-wider">Presente en video</span>
                                    <h4 class="font-bold text-sm text-white">Saco Ejecutivo Premium</h4>
                                    <p class="text-xs text-slate-300"><span class="line-through text-slate-500">$129.99</span> <span class="text-emerald-400 font-bold font-mono">$110.49</span></p>
                                </div>
                                <button onclick="addToCartDirect(1, 'Saco Ejecutivo Premium', 110.49, 'https://images.unsplash.com/photo-1539109136881-3be0616acf4b?auto=format&fit=crop&w=300&q=80')" class="bg-gradient-to-r from-purple-500 to-pink-500 hover:from-purple-600 hover:to-pink-600 text-white text-xs font-bold px-4 py-2.5 rounded-xl shadow-lg transition">
                                    Adquirir Look
                                </button>
                            </div>

                            <!-- Producto En Vivo 2 -->
                            <div class="flex items-center gap-4 bg-slate-800/50 p-3 rounded-2xl border border-white/10 hover:border-purple-500/40 transition">
                                <img src="https://images.unsplash.com/photo-1595950653106-6c9ebd614d3a?auto=format&fit=crop&w=300&q=80" alt="Lentes" class="w-16 h-16 object-cover rounded-xl" onerror="this.src='https://placehold.co/100x100'">
                                <div class="flex-grow">
                                    <span class="text-[10px] text-pink-400 font-bold uppercase tracking-wider">Próximo Look</span>
                                    <h4 class="font-bold text-sm text-white">Lentes de Sol Aviador</h4>
                                    <p class="text-xs text-slate-300"><span class="line-through text-slate-500">$35.00</span> <span class="text-emerald-400 font-bold font-mono">$29.75</span></p>
                                </div>
                                <button onclick="addToCartDirect(7, 'Lentes de Sol Aviador', 29.75, 'https://images.unsplash.com/photo-1595950653106-6c9ebd614d3a?auto=format&fit=crop&w=300&q=80')" class="bg-slate-700 hover:bg-slate-600 text-white text-xs font-bold px-4 py-2.5 rounded-xl transition">
                                    Adquirir Look
                                </button>
                            </div>
                        </div>

                        <div class="text-xs text-purple-300 flex items-center gap-2">
                            <i class="fa-solid fa-circle-info"></i> El descuento especial se aplica automáticamente al añadir la prenda desde este panel de Venta Flash.
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- SECCIÓN: MEMBRESÍA VIP (SUBSCRIPCIONES - BASADO EN APUNTES) -->
        <section id="tab-vip" class="tab-content hidden fade-in max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-12">
            <div class="text-center max-w-3xl mx-auto mb-12">
                <span class="bg-gradient-to-r from-yellow-500 to-amber-600 text-white text-[11px] font-bold px-3 py-1 rounded-full uppercase tracking-widest shadow-sm">Modelos de Monetización</span>
                <h2 class="text-4xl font-extrabold text-slate-900 tracking-tight mt-3 mb-4">Vesta VIP Club</h2>
                <p class="text-slate-600 text-base">Subscríbete para recibir mensualmente cajas seleccionadas con ropa curada por diseñadores profesionales directas a tu puerta, con descuentos infinitos.</p>
            </div>

            <!-- Planes de Subscripción -->
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8 max-w-5xl mx-auto">
                <!-- Plan Bronce -->
                <div class="bg-white rounded-3xl p-8 border border-slate-200/80 shadow-sm hover:shadow-md transition flex flex-col justify-between">
                    <div>
                        <h3 class="font-bold text-xl text-slate-800">Box Esencial</h3>
                        <p class="text-slate-500 text-xs mt-1">Lo básico para refrescar tu look</p>
                        <div class="mt-5 mb-6">
                            <span class="text-4xl font-black text-slate-900">$29</span>
                            <span class="text-slate-500 text-sm font-medium">/mes</span>
                        </div>
                        <hr class="border-slate-100 mb-6">
                        <ul class="space-y-4 text-slate-600 text-sm mb-8">
                            <li class="flex items-center gap-3"><i class="fa-solid fa-check text-purple-600"></i> 1 Prenda curada al mes</li>
                            <li class="flex items-center gap-3"><i class="fa-solid fa-check text-purple-600"></i> 10% de descuento en catálogo</li>
                            <li class="flex items-center gap-3"><i class="fa-solid fa-check text-purple-600"></i> Envío gratis estándar</li>
                            <li class="text-slate-400 flex items-center gap-3"><i class="fa-solid fa-xmark"></i> Acceso a pasarelas privadas</li>
                        </ul>
                    </div>
                    <button onclick="subscribeVIP('Box Esencial')" class="w-full bg-slate-900 hover:bg-slate-800 text-white font-bold py-3.5 rounded-2xl shadow-lg transition">Suscribirme</button>
                </div>

                <!-- Plan Gold (Destacado) -->
                <div class="bg-white rounded-3xl p-8 border-2 border-purple-500 shadow-xl relative flex flex-col justify-between transform -translate-y-2 md:-translate-y-4">
                    <div class="absolute -top-4 left-1/2 -translate-x-1/2 bg-gradient-to-r from-purple-600 to-pink-500 text-white font-bold text-xs px-4 py-1.5 rounded-full uppercase tracking-wider shadow-md">El Más Recomendado</div>
                    <div>
                        <h3 class="font-bold text-xl text-slate-800 mt-2">Box Premium VIP</h3>
                        <p class="text-slate-500 text-xs mt-1">La experiencia completa de alta moda</p>
                        <div class="mt-5 mb-6">
                            <span class="text-4xl font-black text-purple-600">$59</span>
                            <span class="text-slate-500 text-sm font-medium">/mes</span>
                        </div>
                        <hr class="border-slate-100 mb-6">
                        <ul class="space-y-4 text-slate-600 text-sm mb-8">
                            <li class="flex items-center gap-3"><i class="fa-solid fa-check text-purple-600"></i> 2 a 3 Prendas curadas al mes</li>
                            <li class="flex items-center gap-3"><i class="fa-solid fa-check text-purple-600"></i> 20% de descuento en catálogo</li>
                            <li class="flex items-center gap-3"><i class="fa-solid fa-check text-purple-600"></i> Envío Express prioritario</li>
                            <li class="flex items-center gap-3"><i class="fa-solid fa-check text-purple-600"></i> Acceso prioritario a Live Shopping</li>
                        </ul>
                    </div>
                    <button onclick="subscribeVIP('Box Premium VIP')" class="w-full bg-gradient-to-r from-purple-600 to-pink-500 hover:from-purple-700 hover:to-pink-600 text-white font-bold py-3.5 rounded-2xl shadow-lg transition">Suscribirme</button>
                </div>

                <!-- Plan Platinum -->
                <div class="bg-white rounded-3xl p-8 border border-slate-200/80 shadow-sm hover:shadow-md transition flex flex-col justify-between">
                    <div>
                        <h3 class="font-bold text-xl text-slate-800">Box Coleccionista</h3>
                        <p class="text-slate-500 text-xs mt-1">Moda exclusiva y premium ilimitada</p>
                        <div class="mt-5 mb-6">
                            <span class="text-4xl font-black text-slate-900">$99</span>
                            <span class="text-slate-500 text-sm font-medium">/mes</span>
                        </div>
                        <hr class="border-slate-100 mb-6">
                        <ul class="space-y-4 text-slate-600 text-sm mb-8">
                            <li class="flex items-center gap-3"><i class="fa-solid fa-check text-purple-600"></i> 4+ Prendas exclusivas al mes</li>
                            <li class="flex items-center gap-3"><i class="fa-solid fa-check text-purple-600"></i> 30% de descuento en catálogo</li>
                            <li class="flex items-center gap-3"><i class="fa-solid fa-check text-purple-600"></i> Envío ultra-rápido en 24 horas</li>
                            <li class="flex items-center gap-3"><i class="fa-solid fa-check text-purple-600"></i> Caja personalizada por tu estilista</li>
                        </ul>
                    </div>
                    <button onclick="subscribeVIP('Box Coleccionista')" class="w-full bg-slate-900 hover:bg-slate-800 text-white font-bold py-3.5 rounded-2xl shadow-lg transition">Suscribirme</button>
                </div>
            </div>
        </section>

        <!-- SECCIÓN: LOGÍSTICA & SEGUIMIENTO (BASADO EN APUNTES) -->
        <section id="tab-tracking" class="tab-content hidden fade-in max-w-3xl mx-auto px-4 sm:px-6 lg:px-8 py-12">
            <div class="bg-white rounded-3xl p-6 sm:p-10 border border-slate-150 shadow-xl">
                <div class="text-center mb-8">
                    <span class="bg-purple-100 text-purple-700 text-xs font-bold px-3 py-1.5 rounded-full uppercase tracking-wider"><i class="fa-solid fa-truck-fast"></i> Logística de Envíos</span>
                    <h2 class="text-3xl font-bold mt-3 text-slate-900">Rastrea tu Pedido</h2>
                    <p class="text-slate-500 text-sm mt-1">Conoce el estado del despacho de tus compras de moda en tiempo real.</p>
                </div>

                <!-- Campo de Entrada para Rastreo -->
                <div class="flex flex-col sm:flex-row gap-3 mb-8">
                    <input id="tracking-input" type="text" placeholder="Introduce el ID de rastreo (ej: TRK-2026-X1Y)" class="flex-grow px-5 py-4 bg-slate-50 border border-slate-200 rounded-2xl focus:outline-none focus:ring-2 focus:ring-purple-500 focus:border-purple-500 text-sm transition">
                    <button onclick="trackOrder()" class="bg-purple-600 hover:bg-purple-700 text-white font-bold px-8 py-4 rounded-2xl shadow-lg shadow-purple-500/15 transition flex items-center justify-center gap-2">
                        <i class="fa-solid fa-magnifying-glass"></i> Consultar
                    </button>
                </div>

                <!-- Línea de Tiempo de Envíos (Logística) -->
                <div id="tracking-result" class="hidden">
                    <hr class="border-slate-100 mb-8">
                    
                    <div class="flex items-center justify-between mb-8">
                        <div>
                            <p class="text-xs text-slate-400 font-bold uppercase tracking-wider">Orden ID</p>
                            <p class="font-mono font-bold text-slate-800" id="result-order-id">TRK-2026-X1Y</p>
                        </div>
                        <div class="text-right">
                            <p class="text-xs text-slate-400 font-bold uppercase tracking-wider">Método de Envío</p>
                            <p class="font-semibold text-slate-800 text-sm">Aura Logística Premium</p>
                        </div>
                    </div>

                    <!-- Estructura visual de pasos de Logística -->
                    <div class="space-y-8 relative before:absolute before:inset-0 before:left-3.5 before:top-2 before:w-0.5 before:bg-slate-200 before:h-[85%]">
                        
                        <!-- Paso 1: Procesado -->
                        <div class="flex items-start gap-4 relative">
                            <div class="h-8 w-8 rounded-full bg-purple-600 text-white flex items-center justify-center text-xs z-10 font-bold shadow-md shadow-purple-500/30" id="step1-icon">
                                <i class="fa-solid fa-check"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-slate-800" id="step1-title">Pedido Confirmado</h4>
                                <p class="text-xs text-slate-500" id="step1-time">Hoy - 12:35 PM</p>
                                <p class="text-sm text-slate-600 mt-0.5">El pago ha sido procesado de manera segura en nuestra pasarela.</p>
                            </div>
                        </div>

                        <!-- Paso 2: Empacado -->
                        <div class="flex items-start gap-4 relative">
                            <div class="h-8 w-8 rounded-full bg-slate-200 text-slate-600 flex items-center justify-center text-xs z-10 font-bold" id="step2-icon">
                                <i class="fa-solid fa-box"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-slate-400" id="step2-title">Preparación y Empaque</h4>
                                <p class="text-xs text-slate-400" id="step2-time">Pendiente</p>
                                <p class="text-sm text-slate-400 mt-0.5">Nuestra bodega está seleccionando las mejores prendas de tu orden.</p>
                            </div>
                        </div>

                        <!-- Paso 3: En camino -->
                        <div class="flex items-start gap-4 relative">
                            <div class="h-8 w-8 rounded-full bg-slate-200 text-slate-600 flex items-center justify-center text-xs z-10 font-bold" id="step3-icon">
                                <i class="fa-solid fa-truck-ramp-box"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-slate-400" id="step3-title">En Ruta de Despacho</h4>
                                <p class="text-xs text-slate-400" id="step3-time">Pendiente</p>
                                <p class="text-sm text-slate-400 mt-0.5">El paquete fue entregado al operador logístico para su envío express.</p>
                            </div>
                        </div>

                        <!-- Paso 4: Entregado -->
                        <div class="flex items-start gap-4 relative">
                            <div class="h-8 w-8 rounded-full bg-slate-200 text-slate-600 flex items-center justify-center text-xs z-10 font-bold" id="step4-icon">
                                <i class="fa-solid fa-house-chimney"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-slate-400" id="step4-title">Entregado con Éxito</h4>
                                <p class="text-xs text-slate-400" id="step4-time">Pendiente</p>
                                <p class="text-sm text-slate-400 mt-0.5">El repartidor ha completado la entrega de forma segura.</p>
                            </div>
                        </div>

                    </div>
                </div>
            </div>
        </section>

        <!-- SECCIÓN: AFILIADOS (BASADO EN APUNTES) -->
        <section id="tab-affiliates" class="tab-content hidden fade-in max-w-4xl mx-auto px-4 sm:px-6 lg:px-8 py-12">
            <div class="bg-white rounded-3xl p-6 sm:p-10 border border-slate-150 shadow-xl overflow-hidden relative">
                <div class="absolute -right-12 -top-12 w-64 h-64 bg-purple-100 rounded-full opacity-40"></div>
                
                <div class="relative z-10">
                    <span class="bg-purple-100 text-purple-700 text-xs font-bold px-3 py-1.5 rounded-full uppercase tracking-wider"><i class="fa-solid fa-users"></i> Programa de Afiliación</span>
                    <h2 class="text-3xl font-extrabold text-slate-900 mt-3 mb-2">Gana recomendando nuestra moda</h2>
                    <p class="text-slate-500 text-sm max-w-xl">Genera tu ID de seguimiento personalizado. Coloca este enlace en tus redes y recibe un <b>10% de comisión</b> por cada venta realizada a través de tu link.</p>

                    <!-- Generador de Link de Afiliado -->
                    <div class="mt-8 bg-slate-50 p-6 rounded-2xl border border-slate-100">
                        <h3 class="font-bold text-sm text-slate-700 mb-4 uppercase tracking-wide">Generador de Enlace Personalizado</h3>
                        <div class="flex flex-col sm:flex-row gap-3">
                            <input id="affiliate-name" type="text" placeholder="Escribe tu Nombre / Red Social (ej: MariaInfluencer)" class="flex-grow px-5 py-3.5 bg-white border border-slate-200 rounded-xl focus:outline-none focus:ring-2 focus:ring-purple-500 text-sm transition">
                            <button onclick="generateAffiliateLink()" class="bg-slate-900 hover:bg-slate-800 text-white font-bold px-6 py-3.5 rounded-xl text-sm shadow-md transition">
                                Generar Enlace
                            </button>
                        </div>

                        <!-- Enlace Generado -->
                        <div id="affiliate-link-container" class="hidden mt-6 pt-6 border-t border-slate-200/60">
                            <p class="text-xs text-slate-400 font-bold uppercase mb-2">Tu Enlace de Seguimiento de Afiliados</p>
                            <div class="flex items-center gap-2">
                                <input id="generated-link" type="text" readonly class="flex-grow px-4 py-3 bg-slate-100 border border-slate-200 rounded-lg text-xs font-mono text-slate-600 focus:outline-none">
                                <button onclick="copyAffiliateLink()" class="bg-purple-600 hover:bg-purple-700 text-white font-bold px-4 py-3 rounded-lg text-xs transition flex items-center gap-1.5">
                                    <i class="fa-regular fa-copy"></i> Copiar
                                </button>
                            </div>
                        </div>
                    </div>

                    <!-- Métricas de Afiliados de Ejemplo -->
                    <div class="grid grid-cols-1 sm:grid-cols-3 gap-6 mt-10">
                        <div class="bg-purple-50/50 p-5 rounded-2xl border border-purple-100/50 text-center">
                            <p class="text-[10px] text-purple-400 font-bold uppercase tracking-wider">Clics Totales</p>
                            <p class="text-2xl font-black text-purple-700 mt-1">452</p>
                        </div>
                        <div class="bg-pink-50/50 p-5 rounded-2xl border border-pink-100/50 text-center">
                            <p class="text-[10px] text-pink-400 font-bold uppercase tracking-wider">Ventas Convertidas</p>
                            <p class="text-2xl font-black text-pink-700 mt-1">18</p>
                        </div>
                        <div class="bg-emerald-50/50 p-5 rounded-2xl border border-emerald-100/50 text-center">
                            <p class="text-[10px] text-emerald-400 font-bold uppercase tracking-wider">Comisiones Pendientes</p>
                            <p class="text-2xl font-black text-emerald-700 mt-1">$95.80</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>

    </main>

    <!-- CARRITO DE COMPRAS DESLIZANTE (DRAWER) -->
    <div id="cart-drawer" class="fixed inset-0 z-50 bg-black/60 backdrop-blur-sm hidden transition-opacity duration-300">
        <div class="absolute right-0 top-0 bottom-0 w-full max-w-md bg-white shadow-2xl flex flex-col justify-between transform translate-x-full transition-transform duration-300" id="cart-panel">
            
            <!-- Cabecera Carrito -->
            <div class="p-6 border-b border-slate-100 flex justify-between items-center bg-slate-50">
                <div class="flex items-center gap-2.5">
                    <i class="fa-solid fa-cart-shopping text-purple-600 text-lg"></i>
                    <h3 class="font-extrabold text-lg text-slate-900">Tu Carrito de Ropa</h3>
                </div>
                <button onclick="toggleCartDrawer()" class="p-2 hover:bg-slate-200 text-slate-400 hover:text-slate-700 rounded-xl transition">
                    <i class="fa-solid fa-xmark text-lg"></i>
                </button>
            </div>

            <!-- Listado de Productos en el Carrito -->
            <div class="flex-grow overflow-y-auto p-6 space-y-4" id="cart-items-container">
                <!-- Se inyecta por JavaScript o muestra mensaje de vacío -->
                <div class="text-center py-20 text-slate-400">
                    <i class="fa-solid fa-bag-shopping text-5xl mb-4 text-slate-200"></i>
                    <p class="text-sm">Tu carrito está esperando por tus outfits.</p>
                </div>
            </div>

            <!-- Resumen de Costos y Acciones -->
            <div class="p-6 border-t border-slate-100 bg-slate-50 space-y-4">
                <div class="flex justify-between items-center text-sm text-slate-500">
                    <span>Subtotal</span>
                    <span class="font-mono text-slate-800" id="cart-subtotal">$0.00</span>
                </div>
                <div class="flex justify-between items-center text-sm text-slate-500">
                    <span>Envío</span>
                    <span class="font-bold text-emerald-600">Gratis</span>
                </div>
                <div class="flex justify-between items-center text-base font-bold text-slate-900">
                    <span>Total estimado</span>
                    <span class="font-mono text-lg" id="cart-total">$0.00</span>
                </div>

                <div class="pt-2">
                    <button id="checkout-btn" onclick="openPaymentGateway()" disabled class="w-full bg-gradient-to-r from-purple-600 to-pink-500 disabled:from-slate-300 disabled:to-slate-300 disabled:cursor-not-allowed text-white font-bold py-4 rounded-2xl shadow-lg shadow-purple-500/10 hover:shadow-purple-500/20 hover:scale-[1.01] active:scale-100 transition duration-150 flex items-center justify-center gap-2">
                        <i class="fa-solid fa-lock text-sm"></i> Proceder al Pago Seguro
                    </button>
                </div>
            </div>

        </div>
    </div>

    <!-- MODAL: PASARELA DE PAGO SEGURA (CON COMPONENTES DE SEGURIDAD DIGITAL) -->
    <div id="payment-modal" class="fixed inset-0 z-50 bg-black/70 backdrop-blur-sm hidden flex items-center justify-center p-4">
        <div class="bg-white rounded-3xl max-w-lg w-full overflow-hidden shadow-2xl border border-slate-100 transform scale-95 transition-all duration-300" id="payment-panel">
            
            <!-- Cabecera de Pasarela Segura -->
            <div class="bg-gradient-to-r from-emerald-600 to-teal-600 p-6 text-white">
                <div class="flex justify-between items-center mb-2">
                    <span class="bg-white/20 text-white text-[10px] font-bold px-2.5 py-1 rounded-full uppercase tracking-widest flex items-center gap-1">
                        <i class="fa-solid fa-shield-halved"></i> SSL Encrypted 256-bit
                    </span>
                    <button onclick="closePaymentGateway()" class="text-white/80 hover:text-white p-1 rounded-lg hover:bg-white/10 transition">
                        <i class="fa-solid fa-xmark text-lg"></i>
                    </button>
                </div>
                <h3 class="text-xl font-bold">Pasarela de Pago Segura</h3>
                <p class="text-xs text-emerald-100">Transacción protegida por protocolos de criptografía avanzada.</p>
            </div>

            <!-- Formulario de la Pasarela de Pago -->
            <div class="p-6 space-y-6">
                <!-- Información del Monto -->
                <div class="bg-slate-50 p-4 rounded-2xl flex justify-between items-center border border-slate-100">
                    <div>
                        <p class="text-xs text-slate-400 font-bold uppercase">Monto Neto a Pagar</p>
                        <p class="text-slate-800 text-xs font-semibold" id="checkout-items-summary">Cargando prendas...</p>
                    </div>
                    <span class="text-2xl font-mono font-black text-slate-900" id="checkout-total-price">$00.00</span>
                </div>

                <div class="space-y-4">
                    <!-- Titular de Tarjeta -->
                    <div>
                        <label class="block text-xs font-bold text-slate-600 uppercase mb-1.5">Nombre del Titular</label>
                        <input id="card-name" type="text" placeholder="Ej: Esmeraldas Informática" class="w-full px-4 py-3 bg-slate-50 border border-slate-200 rounded-xl focus:outline-none focus:ring-2 focus:ring-purple-500 text-sm transition">
                    </div>

                    <!-- Número de Tarjeta -->
                    <div>
                        <label class="block text-xs font-bold text-slate-600 uppercase mb-1.5">Número de Tarjeta</label>
                        <div class="relative">
                            <input id="card-number" type="text" maxlength="19" placeholder="4000 1234 5678 9010" oninput="formatCardNumber(this)" class="w-full pl-4 pr-12 py-3 bg-slate-50 border border-slate-200 rounded-xl focus:outline-none focus:ring-2 focus:ring-purple-500 text-sm font-mono tracking-wider transition">
                            <div class="absolute right-3.5 top-3.5 text-slate-400">
                                <i class="fa-brands fa-cc-visa text-lg"></i>
                            </div>
                        </div>
                    </div>

                    <!-- Caducidad & CVC -->
                    <div class="grid grid-cols-2 gap-4">
                        <div>
                            <label class="block text-xs font-bold text-slate-600 uppercase mb-1.5">Expiración</label>
                            <input id="card-expiry" type="text" maxlength="5" placeholder="MM/AA" oninput="formatExpiry(this)" class="w-full px-4 py-3 bg-slate-50 border border-slate-200 rounded-xl focus:outline-none focus:ring-2 focus:ring-purple-500 text-sm font-mono transition">
                        </div>
                        <div>
                            <label class="block text-xs font-bold text-slate-600 uppercase mb-1.5">CVC / Código de Seguridad</label>
                            <input id="card-cvc" type="password" maxlength="3" placeholder="•••" class="w-full px-4 py-3 bg-slate-50 border border-slate-200 rounded-xl focus:outline-none focus:ring-2 focus:ring-purple-500 text-sm font-mono tracking-widest transition">
                        </div>
                    </div>
                </div>

                <!-- Botón de Envío y Animación de Seguridad -->
                <button onclick="processSecurePayment()" class="w-full bg-emerald-600 hover:bg-emerald-700 text-white font-bold py-4 rounded-2xl shadow-lg shadow-emerald-600/10 transition flex items-center justify-center gap-2 text-sm" id="pay-submit-btn">
                    <i class="fa-solid fa-lock text-xs"></i> Autorizar Pago Seguro
                </button>

                <!-- Animación de Carga de Pago -->
                <div id="payment-loading" class="hidden text-center py-4">
                    <div class="inline-block animate-spin rounded-full h-8 w-8 border-4 border-emerald-500 border-t-transparent mb-2"></div>
                    <p class="text-xs text-slate-500 font-medium">Validando seguridad criptográfica SSL con servidor bancario...</p>
                </div>
            </div>
        </div>
    </div>

    <!-- PIE DE PÁGINA (FOOTER) -->
    <footer class="bg-slate-900 text-slate-400 pt-16 pb-12 border-t border-slate-800">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-1 md:grid-cols-4 gap-8 mb-12">
                <!-- Columna Marca -->
                <div class="space-y-4">
                    <div class="flex items-center gap-3">
                        <div class="bg-gradient-to-r from-purple-600 to-pink-500 text-white p-2 rounded-lg">
                            <i class="fa-solid fa-shirt text-sm"></i>
                        </div>
                        <span class="text-white font-extrabold tracking-tight text-lg">VESTA AURA</span>
                    </div>
                    <p class="text-xs text-slate-400 leading-relaxed">Emprendimiento digital que conjuga la última vanguardia en moda sustentable con la arquitectura de e-commerce más robusta del mercado.</p>
                    <div class="flex gap-3 pt-2">
                        <a href="#" class="h-8 w-8 rounded-lg bg-slate-800 hover:bg-purple-600 hover:text-white flex items-center justify-center transition"><i class="fa-brands fa-facebook-f text-sm"></i></a>
                        <a href="#" class="h-8 w-8 rounded-lg bg-slate-800 hover:bg-purple-600 hover:text-white flex items-center justify-center transition"><i class="fa-brands fa-instagram text-sm"></i></a>
                        <a href="#" class="h-8 w-8 rounded-lg bg-slate-800 hover:bg-purple-600 hover:text-white flex items-center justify-center transition"><i class="fa-brands fa-tiktok text-sm"></i></a>
                    </div>
                </div>

                <!-- Columna Arquitectura E-commerce (Referencia de Clase) -->
                <div>
                    <h4 class="text-white font-bold text-sm mb-4 uppercase tracking-wider">Arquitectura</h4>
                    <ul class="space-y-2.5 text-xs text-slate-400">
                        <li><span class="hover:text-purple-400 transition cursor-pointer" onclick="changeTab('catalog')">Catálogo Dinámico</span></li>
                        <li><span class="hover:text-purple-400 transition cursor-pointer" onclick="toggleCartDrawer()">Carrito de Compra Inteligente</span></li>
                        <li><span class="hover:text-purple-400 transition cursor-pointer" onclick="openPaymentGateway()">Pasarela de Pago Segura</span></li>
                        <li><span class="hover:text-purple-400 transition cursor-pointer" onclick="changeTab('tracking')">Logística Integrada</span></li>
                    </ul>
                </div>

                <!-- Columna Monetización (Referencia de Clase) -->
                <div>
                    <h4 class="text-white font-bold text-sm mb-4 uppercase tracking-wider">Modelos Avanzados</h4>
                    <ul class="space-y-2.5 text-xs text-slate-400">
                        <li><span class="hover:text-purple-400 transition cursor-pointer" onclick="changeTab('live')">Live Shopping (Venta Flash)</span></li>
                        <li><span class="hover:text-purple-400 transition cursor-pointer" onclick="changeTab('vip')">Subscripción (Membresías VIP)</span></li>
                        <li><span class="hover:text-purple-400 transition cursor-pointer" onclick="changeTab('affiliates')">Marketing de Afiliados</span></li>
                        <li><span class="hover:text-purple-400 transition cursor-pointer">Sponsorships & Patrocinios</span></li>
                    </ul>
                </div>

                <!-- Sellos de Seguridad (Seguridad) -->
                <div class="space-y-4">
                    <h4 class="text-white font-bold text-sm mb-4 uppercase tracking-wider">Seguridad Digital</h4>
                    <p class="text-xs text-slate-400">Toda transacción está cifrada mediante algoritmos SSL de última generación de extremo a extremo.</p>
                    <div class="flex items-center gap-2 pt-2">
                        <div class="bg-slate-800 px-3 py-1.5 rounded-lg border border-slate-700/60 flex items-center gap-1.5 text-[10px] text-white">
                            <i class="fa-solid fa-lock text-emerald-500"></i> HTTPS SECURE
                        </div>
                        <div class="bg-slate-800 px-3 py-1.5 rounded-lg border border-slate-700/60 flex items-center gap-1.5 text-[10px] text-white">
                            <i class="fa-brands fa-cc-stripe text-indigo-400 text-xs"></i> STRIPE
                        </div>
                    </div>
                </div>
            </div>

            <hr class="border-slate-800 mb-8">

            <div class="flex flex-col sm:flex-row justify-between items-center gap-4 text-xs">
                <p>&copy; 2026 Vesta Aura Boutique. Todos los derechos reservados.</p>
                <p>Esmeraldas, Ecuador. Informática de Negocios.</p>
            </div>
        </div>
    </footer>

    <!-- COMPORTAMIENTO DINÁMICO EN JAVASCRIPT -->
    <script>
        // Listado de Productos Oficial (8 prendas premium divididas por categoría con precios variados)
        const products = [
            {
                id: 1,
                name: "Saco Ejecutivo Premium",
                category: "formal",
                price: 129.99,
                badge: "Elegante",
                image: "https://images.unsplash.com/photo-1539109136881-3be0616acf4b?auto=format&fit=crop&w=600&q=80"
            },
            {
                id: 2,
                name: "Vestido de Gala 'Sienna'",
                category: "formal",
                price: 189.50,
                badge: "Exclusivo",
                image: "https://images.unsplash.com/photo-1595777457583-95e059d581b8?auto=format&fit=crop&w=600&q=80"
            },
            {
                id: 3,
                name: "Chaqueta Denim Vintage",
                category: "casual",
                price: 75.00,
                badge: "Más Vendido",
                image: "https://images.unsplash.com/photo-1576995853123-5a10305d93c0?auto=format&fit=crop&w=600&q=80"
            },
            {
                id: 4,
                name: "Camisa de Lino Soft",
                category: "casual",
                price: 45.90,
                badge: "Nuevo",
                image: "https://images.unsplash.com/photo-1603252109303-2751441dd157?auto=format&fit=crop&w=600&q=80"
            },
            {
                id: 5,
                name: "Set Active-Fit Pro",
                category: "deportivo",
                price: 85.00,
                badge: "Flex Confort",
                image: "https://images.unsplash.com/photo-1518310383802-640c2de311b2?auto=format&fit=crop&w=600&q=80"
            },
            {
                id: 6,
                name: "Jogger Urbano Premium",
                category: "deportivo",
                price: 59.90,
                badge: "Tendencia",
                image: "https://images.unsplash.com/photo-1551854838-212c50b4c184?auto=format&fit=crop&w=600&q=80"
            },
            {
                id: 7,
                name: "Lentes de Sol Aviador",
                category: "accesorios",
                price: 35.00,
                badge: "Eco-Friendly",
                image: "https://images.unsplash.com/photo-1595950653106-6c9ebd614d3a?auto=format&fit=crop&w=600&q=80"
            },
            {
                id: 8,
                name: "Bolso de Cuero Minimalista",
                category: "accesorios",
                price: 110.00,
                badge: "Elegante",
                image: "https://images.unsplash.com/photo-1548036328-c9fa89d128fa?auto=format&fit=crop&w=600&q=80"
            }
        ];

        // Estado del Carrito y Aplicación
        let cart = [];
        let currentCategory = 'all';

        // Al cargar la página, inicializa catálogo y timers
        window.onload = function() {
            renderProducts(products);
            startLiveStreamSimulation();
        }

        // Renderizar catálogo en la cuadrícula de productos
        function renderProducts(productsList) {
            const grid = document.getElementById('product-grid');
            grid.innerHTML = '';

            if (productsList.length === 0) {
                grid.innerHTML = `
                    <div class="col-span-full text-center py-16 text-slate-400">
                        <i class="fa-solid fa-cloud-showers-heavy text-5xl mb-4"></i>
                        <p class="font-medium text-slate-500">No encontramos resultados para tu búsqueda.</p>
                    </div>
                `;
                return;
            }

            productsList.forEach(product => {
                const card = document.createElement('div');
                card.className = "bg-white rounded-3xl border border-slate-200/60 overflow-hidden shadow-sm hover:shadow-xl hover:border-purple-200 group transition duration-300 flex flex-col justify-between";
                card.innerHTML = `
                    <div class="relative overflow-hidden aspect-[4/5] bg-slate-100">
                        <span class="absolute top-4 left-4 bg-white/90 backdrop-blur-md text-slate-800 text-[10px] font-bold px-2.5 py-1.5 rounded-full z-10 shadow-sm uppercase tracking-wide border border-slate-100">
                            ${product.badge}
                        </span>
                        <img src="${product.image}" alt="${product.name}" class="w-full h-full object-cover group-hover:scale-105 transition duration-500" onerror="this.src='https://placehold.co/400x500/slate/ffffff?text=${encodeURIComponent(product.name)}'">
                        <div class="absolute inset-x-0 bottom-0 p-4 bg-gradient-to-t from-black/60 to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex justify-end">
                            <button onclick="addToCart(${product.id})" class="bg-white text-slate-900 p-3 rounded-full shadow-lg hover:bg-purple-600 hover:text-white transition">
                                <i class="fa-solid fa-cart-plus"></i>
                            </button>
                        </div>
                    </div>
                    <div class="p-5 flex-grow flex flex-col justify-between">
                        <div>
                            <span class="text-[10px] text-purple-600 font-extrabold uppercase tracking-widest">${product.category}</span>
                            <h3 class="font-bold text-slate-800 text-sm mt-1 leading-snug group-hover:text-purple-600 transition">${product.name}</h3>
                        </div>
                        <div class="flex items-center justify-between mt-4">
                            <span class="text-lg font-black font-mono text-slate-900">$${product.price.toFixed(2)}</span>
                            <button onclick="addToCart(${product.id})" class="bg-slate-50 hover:bg-purple-50 hover:text-purple-600 text-slate-800 text-xs font-bold px-3.5 py-2 rounded-xl border border-slate-150 transition flex items-center gap-1.5">
                                <i class="fa-solid fa-plus text-[10px]"></i> Añadir
                            </button>
                        </div>
                    </div>
                `;
                grid.appendChild(card);
            });
        }

        // Filtrar productos por categoría
        function filterCategory(category) {
            currentCategory = category;
            
            // Actualizar apariencia visual de píldoras
            document.querySelectorAll('.cat-pill').forEach(pill => {
                pill.className = "cat-pill bg-white hover:bg-slate-100 text-slate-700 font-semibold px-5 py-2.5 rounded-xl text-sm border border-slate-200/80 transition shadow-sm";
            });
            const activePill = document.getElementById(`cat-${category}`);
            if (activePill) {
                activePill.className = "cat-pill bg-purple-600 text-white font-bold px-5 py-2.5 rounded-xl text-sm transition shadow-sm";
            }

            filterProducts();
        }

        // Filtrar productos combinando categoría y entrada de búsqueda
        function filterProducts() {
            const searchVal = document.getElementById('search-input').value.toLowerCase();
            let filtered = products;

            if (currentCategory !== 'all') {
                filtered = filtered.filter(p => p.category === currentCategory);
            }

            if (searchVal) {
                filtered = filtered.filter(p => p.name.toLowerCase().includes(searchVal));
            }

            renderProducts(filtered);
        }

        // Controladores del Carrito (Add, UI, Delete)
        function toggleCartDrawer() {
            const drawer = document.getElementById('cart-drawer');
            const panel = document.getElementById('cart-panel');
            
            if (drawer.classList.contains('hidden')) {
                drawer.classList.remove('hidden');
                setTimeout(() => {
                    panel.classList.remove('translate-x-full');
                }, 50);
            } else {
                panel.classList.add('translate-x-full');
                setTimeout(() => {
                    drawer.classList.add('hidden');
                }, 300);
            }
        }

        function addToCart(productId) {
            const product = products.find(p => p.id === productId);
            if (!product) return;

            const existingItem = cart.find(item => item.id === productId);
            if (existingItem) {
                existingItem.quantity += 1;
            } else {
                cart.push({ ...product, quantity: 1 });
            }

            updateCartUI();
            showToast(`Añadido: ${product.name}`);
        }

        function addToCartDirect(productId, name, price, img) {
            const existingItem = cart.find(item => item.id === productId);
            if (existingItem) {
                existingItem.quantity += 1;
            } else {
                cart.push({ id: productId, name, price, image: img, quantity: 1 });
            }
            updateCartUI();
            showToast(`Añadido: ${name} (Look en Vivo)`);
            toggleCartDrawer();
        }

        function updateCartUI() {
            const itemsContainer = document.getElementById('cart-items-container');
            const cartCountElement = document.getElementById('cart-count');
            const checkoutBtn = document.getElementById('checkout-btn');
            
            // Totalizadores
            let totalQty = 0;
            let subtotal = 0;

            itemsContainer.innerHTML = '';

            if (cart.length === 0) {
                itemsContainer.innerHTML = `
                    <div class="text-center py-20 text-slate-400">
                        <i class="fa-solid fa-bag-shopping text-5xl mb-4 text-slate-200"></i>
                        <p class="text-sm">Tu carrito está esperando por tus outfits.</p>
                    </div>
                `;
                checkoutBtn.disabled = true;
            } else {
                checkoutBtn.disabled = false;
                cart.forEach(item => {
                    totalQty += item.quantity;
                    subtotal += item.price * item.quantity;

                    const itemRow = document.createElement('div');
                    itemRow.className = "flex items-center gap-4 bg-slate-50 p-3 rounded-2xl border border-slate-100";
                    itemRow.innerHTML = `
                        <img src="${item.image}" alt="${item.name}" class="w-16 h-16 object-cover rounded-xl bg-slate-200" onerror="this.src='https://placehold.co/100x100'">
                        <div class="flex-grow">
                            <h4 class="font-bold text-slate-800 text-sm line-clamp-1">${item.name}</h4>
                            <p class="text-slate-500 text-xs font-mono mt-0.5">$${item.price.toFixed(2)}</p>
                            <div class="flex items-center gap-2 mt-2">
                                <button onclick="changeQty(${item.id}, -1)" class="h-6 w-6 bg-white hover:bg-slate-200 text-slate-600 rounded flex items-center justify-center border border-slate-200 text-xs">-</button>
                                <span class="font-mono text-xs font-bold text-slate-800 w-5 text-center">${item.quantity}</span>
                                <button onclick="changeQty(${item.id}, 1)" class="h-6 w-6 bg-white hover:bg-slate-200 text-slate-600 rounded flex items-center justify-center border border-slate-200 text-xs">+</button>
                            </div>
                        </div>
                        <button onclick="removeFromCart(${item.id})" class="text-slate-400 hover:text-red-500 p-2 rounded-xl transition">
                            <i class="fa-regular fa-trash-can"></i>
                        </button>
                    `;
                    itemsContainer.appendChild(itemRow);
                });
            }

            cartCountElement.innerText = totalQty;
            document.getElementById('cart-subtotal').innerText = `$${subtotal.toFixed(2)}`;
            document.getElementById('cart-total').innerText = `$${subtotal.toFixed(2)}`;
        }

        function changeQty(productId, amount) {
            const item = cart.find(i => i.id === productId);
            if (!item) return;

            item.quantity += amount;
            if (item.quantity <= 0) {
                removeFromCart(productId);
            } else {
                updateCartUI();
            }
        }

        function removeFromCart(productId) {
            cart = cart.filter(item => item.id !== productId);
            updateCartUI();
            showToast("Prenda eliminada del carrito");
        }

        // SISTEMA DE PASARELA DE PAGO (SIMULACIÓN SEGURA)
        function openPaymentGateway() {
            // Cerrar primero el Drawer para no sobreponer
            toggleCartDrawer();

            const modal = document.getElementById('payment-modal');
            const panel = document.getElementById('payment-panel');
            
            // Llenar información de checkout
            const subtotalText = document.getElementById('cart-subtotal').innerText;
            document.getElementById('checkout-total-price').innerText = subtotalText;
            
            const summaryText = cart.map(item => `${item.name} (x${item.quantity})`).join(', ');
            document.getElementById('checkout-items-summary').innerText = summaryText;

            modal.classList.remove('hidden');
            setTimeout(() => {
                panel.classList.remove('scale-95');
                panel.classList.add('scale-100');
            }, 50);
        }

        function closePaymentGateway() {
            const modal = document.getElementById('payment-modal');
            const panel = document.getElementById('payment-panel');
            
            panel.classList.remove('scale-100');
            panel.classList.add('scale-95');
            setTimeout(() => {
                modal.classList.add('hidden');
            }, 200);
        }

        // Validación y Estilización del formulario de Tarjeta
        function formatCardNumber(input) {
            let v = input.value.replace(/\D/g, '');
            let matches = v.match(/\d{4,16}/g);
            let match = matches && matches[0] || '';
            let parts = [];

            for (let i=0, len=match.length; i<len; i+=4) {
                parts.push(match.substring(i, i+4));
            }

            if (parts.length > 0) {
                input.value = parts.join(' ');
            } else {
                input.value = v;
            }
        }

        function formatExpiry(input) {
            let v = input.value.replace(/\D/g, '');
            if (v.length > 2) {
                input.value = v.substring(0, 2) + '/' + v.substring(2, 4);
            } else {
                input.value = v;
            }
        }

        function processSecurePayment() {
            const name = document.getElementById('card-name').value;
            const number = document.getElementById('card-number').value;
            const expiry = document.getElementById('card-expiry').value;
            const cvc = document.getElementById('card-cvc').value;

            // Validación de Datos de Entrada
            if (!name || number.length < 16 || expiry.length < 5 || cvc.length < 3) {
                showToast("Por favor complete los detalles de pago de forma válida.");
                return;
            }

            // Iniciar animación de procesamiento de seguridad
            document.getElementById('pay-submit-btn').classList.add('hidden');
            document.getElementById('payment-loading').classList.remove('hidden');

            setTimeout(() => {
                // Generar ID de Logística Aleatorio
                const randTrackId = "TRK-2026-" + Math.random().toString(36).substring(2, 7).toUpperCase();
                
                // Limpiar Carrito
                cart = [];
                updateCartUI();

                // Cerrar pasarela y mostrar éxito
                closePaymentGateway();
                
                // Restablecer el botón para el siguiente uso
                document.getElementById('pay-submit-btn').classList.remove('hidden');
                document.getElementById('payment-loading').classList.add('hidden');

                // Enviar al usuario directamente a la pestaña de Logística para ver su pedido
                changeTab('tracking');
                document.getElementById('tracking-input').value = randTrackId;
                
                // Inyectar datos en la línea de tiempo
                document.getElementById('tracking-result').classList.remove('hidden');
                document.getElementById('result-order-id').innerText = randTrackId;
                
                // Registrar hora actual simulada
                const now = new Date();
                document.getElementById('step1-time').innerText = `Hoy - ${now.toLocaleTimeString([], {hour: '2-digit', minute:'2-digit'})}`;

                // Notificar éxito sin usar alerts dañinos
                showToast("¡Transacción Exitosa! Pago procesado con seguridad.");
            }, 3000);
        }

        // LOGÍSTICA & SEGUIMIENTO (Búsqueda interactiva de Orden)
        function trackOrder() {
            const inputVal = document.getElementById('tracking-input').value.trim();
            if (!inputVal) {
                showToast("Por favor ingresa un código de envío.");
                return;
            }

            // Mostrar resultado simulado
            document.getElementById('tracking-result').classList.remove('hidden');
            document.getElementById('result-order-id').innerText = inputVal;
            
            // Simular actualizaciones basadas en el código
            if (inputVal.startsWith("TRK-2026-F")) {
                // Pedido simulado avanzado
                setTrackingStatus(3);
            } else {
                setTrackingStatus(1);
            }
        }

        function setTrackingStatus(activeStep) {
            // Pasos de Logística
            const steps = [
                { id: 1, title: "Pedido Confirmado", icon: "fa-check" },
                { id: 2, title: "Preparación y Empaque", icon: "fa-box" },
                { id: 3, title: "En Ruta de Despacho", icon: "fa-truck-ramp-box" },
                { id: 4, title: "Entregado con Éxito", icon: "fa-house-chimney" }
            ];

            steps.forEach(step => {
                const iconElement = document.getElementById(`step${step.id}-icon`);
                const titleElement = document.getElementById(`step${step.id}-title`);
                const timeElement = document.getElementById(`step${step.id}-time`);

                if (step.id <= activeStep) {
                    iconElement.className = "h-8 w-8 rounded-full bg-purple-600 text-white flex items-center justify-center text-xs z-10 font-bold shadow-md shadow-purple-500/30";
                    iconElement.innerHTML = `<i class="fa-solid fa-check"></i>`;
                    titleElement.className = "font-bold text-slate-800";
                    if (step.id === activeStep) {
                        timeElement.innerText = "Hace un momento";
                    } else {
                        timeElement.innerText = "Completado";
                    }
                } else {
                    iconElement.className = "h-8 w-8 rounded-full bg-slate-200 text-slate-600 flex items-center justify-center text-xs z-10 font-bold";
                    iconElement.innerHTML = `<i class="fa-solid ${step.icon}"></i>`;
                    titleElement.className = "font-bold text-slate-400";
                    timeElement.innerText = "Pendiente";
                }
            });
        }

        // MARKETING DE AFILIADOS Y SUBSCRIPCIONES
        function generateAffiliateLink() {
            const name = document.getElementById('affiliate-name').value.trim();
            if (!name) {
                showToast("Ingresa un identificador válido.");
                return;
            }

            const cleanName = name.replace(/[^a-zA-Z0-9]/g, '');
            const generatedUrl = `${window.location.origin}${window.location.pathname}?ref=${cleanName}`;
            
            document.getElementById('generated-link').value = generatedUrl;
            document.getElementById('affiliate-link-container').classList.remove('hidden');
            showToast("¡Enlace de afiliado generado!");
        }

        function copyAffiliateLink() {
            const copyText = document.getElementById('generated-link');
            copyText.select();
            copyText.setSelectionRange(0, 99999);
            
            // Respaldo de portapapeles seguro de iFrame
            document.execCommand('copy');
            showToast("¡Copiado al portapapeles!");
        }

        function subscribeVIP(planName) {
            showToast(`¡Suscrito con éxito a: ${planName}!`);
        }

        // CONTROLADOR DE NAVEGACIÓN ENTRE SECCIONES (SPA)
        function changeTab(tabName) {
            // Esconder todas las pestañas
            document.querySelectorAll('.tab-content').forEach(tab => {
                tab.classList.add('hidden');
            });
            // Remover estilos activos de los botones
            document.querySelectorAll('.nav-btn').forEach(btn => {
                btn.className = "nav-btn text-slate-600 hover:text-purple-600 transition";
            });

            // Mostrar pestaña activa
            document.getElementById(`tab-${tabName}`).classList.remove('hidden');
            
            // Asignar estilo activo
            const activeBtn = document.getElementById(`nav-${tabName}`);
            if (activeBtn) {
                if (tabName === 'live') {
                    activeBtn.className = "nav-btn text-red-600 font-bold transition flex items-center gap-1.5";
                } else {
                    activeBtn.className = "nav-btn text-purple-600 font-bold transition";
                }
            }
        }

        function toggleMobileMenu() {
            const menu = document.getElementById('mobile-menu');
            const icon = document.getElementById('menu-icon');
            
            if (menu.classList.contains('hidden')) {
                menu.classList.remove('hidden');
                icon.className = "fa-solid fa-xmark text-xl";
            } else {
                menu.classList.add('hidden');
                icon.className = "fa-solid fa-bars text-xl";
            }
        }

        // SIMULADOR DE STREAMING DE VENTA FLASH (CONTEO REGRESIVO)
        function startLiveStreamSimulation() {
            let minutes = 29;
            let seconds = 45;
            const timerElement = document.getElementById('live-timer');
            const viewersElement = document.getElementById('viewers-count');

            setInterval(() => {
                if (seconds === 0) {
                    if (minutes === 0) {
                        minutes = 30; // Reset
                        seconds = 0;
                    } else {
                        minutes--;
                        seconds = 59;
                    }
                } else {
                    seconds--;
                }

                // Dar formato
                const minStr = minutes < 10 ? '0' + minutes : minutes;
                const secStr = seconds < 10 ? '0' + seconds : seconds;
                timerElement.innerText = `${minStr}:${secStr}`;

                // Variar el contador de espectadores de manera realista
                const delta = Math.floor(Math.random() * 11) - 5;
                let currentViewers = parseInt(viewersElement.innerText.replace(',', ''));
                viewersElement.innerText = (currentViewers + delta).toLocaleString();

            }, 1000);
        }

        // Mostrar notificación de toast elegante
        function showToast(message) {
            const toast = document.getElementById('toast');
            const msg = document.getElementById('toast-msg');
            
            msg.innerText = message;
            toast.classList.remove('translate-y-24', 'opacity-0', 'pointer-events-none');
            toast.classList.add('translate-y-0', 'opacity-100');

            setTimeout(() => {
                toast.classList.add('translate-y-24', 'opacity-0', 'pointer-events-none');
                toast.classList.remove('translate-y-0', 'opacity-100');
            }, 3000);
        }
    </script>
</body>
</html>