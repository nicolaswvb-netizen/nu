<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>DRAWS POI - Dibujamos tus sentimientos</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        brand: {
                            terracotta: '#B33B24',
                            mustard: '#D99B26',
                            blue: '#1E82D2',
                            pink: '#E85D75',
                            cream: '#FDF8EE',
                            cardBg: '#FFFDF9',
                            dark: '#2D221E'
                        }
                    },
                    fontFamily: {
                        sans: ['Comic Sans MS', 'Chalkboard SE', 'Fredoka', 'sans-serif'],
                        serif: ['Georgia', 'serif']
                    }
                }
            }
        }
    </script>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css" rel="stylesheet">
    <style>
        .paper-texture {
            background-color: #FDF8EE;
            background-image: radial-gradient(#E8DFCE 0.75px, transparent 0.75px), radial-gradient(#E8DFCE 0.75px, #FDF8EE 0.75px);
            background-size: 30px 30px;
            background-position: 0 0, 15px 15px;
        }
        .hand-drawn-border {
            border-radius: 255px 15px 225px 15px/15px 225px 15px 255px;
        }
        .sketch-shadow {
            box-shadow: 5px 5px 0px 0px #2D221E;
        }
        .sketch-shadow-hover:hover {
            box-shadow: 8px 8px 0px 0px #B33B24;
            transform: translateY(-3px);
        }
    </style>
</head>
<body class="paper-texture text-brand-dark antialiased font-sans flex flex-col min-h-screen">

    <!-- NAV -->
    <nav class="sticky top-0 z-50 bg-[#FDF8EE]/90 backdrop-blur-md border-b-2 border-brand-dark/10 py-3 px-4">
        <div class="max-w-6xl mx-auto flex justify-between items-center">
            <div class="flex items-center gap-3">
                <div class="w-10 h-10 bg-brand-terracotta rounded-full flex items-center justify-center text-white text-xl font-bold border-2 border-brand-dark">
                    🎨
                </div>
                <div>
                    <span class="text-2xl font-black text-brand-terracotta tracking-wider">DRAWS POI</span>
                    <span class="block text-xs font-semibold text-brand-blue -mt-1">Dibujamos tus sentimientos</span>
                </div>
            </div>
            <div class="hidden md:flex gap-6 font-bold text-sm">
                <a href="#quienes-somos" class="hover:text-brand-terracotta transition-colors">Quiénes Somos</a>
                <a href="#que-hacemos" class="hover:text-brand-terracotta transition-colors">Qué Hacemos</a>
                <a href="#mision-vision" class="hover:text-brand-terracotta transition-colors">Misión y Visión</a>
                <a href="#catalogo" class="hover:text-brand-terracotta transition-colors">Catálogo</a>
                <a href="#codigo-qr" class="hover:text-brand-terracotta transition-colors">Código QR</a>
            </div>
            <a href="https://wa.me/573000000000?text=Hola%20Draws%20Poi,%20quiero%20hacer%20un%20pedido" target="_blank" class="bg-brand-mustard hover:bg-brand-terracotta text-white font-bold py-2 px-4 rounded-full border-2 border-brand-dark sketch-shadow text-xs md:text-sm transition-all flex items-center gap-2">
                <i class="fab fa-whatsapp"></i> Haz tu pedido
            </a>
        </div>
    </nav>

    <!-- HERO -->
    <header class="py-12 px-4 max-w-6xl mx-auto text-center">
        <div class="inline-block bg-brand-pink/10 border border-brand-pink text-brand-pink font-bold text-xs uppercase px-3 py-1 rounded-full mb-4">
            ✨ Arte & Regalos Personalizados
        </div>
        <h1 class="text-4xl md:text-6xl font-black text-brand-terracotta mb-4">
            Convertimos tus recuerdos en obras de arte ✏️❤️
        </h1>
        <p class="text-lg md:text-xl text-brand-dark/80 max-w-2xl mx-auto mb-8 font-serif italic">
            "Dibujamos tus sentimientos"
        </p>
    </header>

    <!-- QUIÉNES SOMOS -->
    <section id="quienes-somos" class="py-10 px-4 max-w-5xl mx-auto">
        <div class="bg-brand-cardBg border-4 border-brand-dark p-6 md:p-10 hand-drawn-border sketch-shadow">
            <h2 class="text-3xl font-black text-brand-terracotta mb-4 flex items-center gap-3">
                <span>🎨</span> Quiénes Somos
            </h2>
            <p class="text-base md:text-lg leading-relaxed text-brand-dark/90">
                En <strong>DRAWS POI</strong> nos apasiona capturar emociones, momentos especiales y conexiones únicas a través del dibujo y la pintura. Somos una marca dedicada a crear regalos significativos y personalizados con un toque completamente hecho a mano. Creemos firmemente que cada trazo cuenta una historia y cada regalo debe hacer sonreír a quien lo recibe.
            </p>
        </div>
    </section>

    <!-- QUÉ HACEMOS PARA TI (4 Recuadros) -->
    <section id="que-hacemos" class="py-12 px-4 max-w-6xl mx-auto">
        <h2 class="text-3xl md:text-4xl font-black text-center text-brand-terracotta mb-8">
            ¿Qué hacemos para ti?
        </h2>
        <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-6">
            <div class="bg-brand-cardBg border-3 border-brand-dark p-6 rounded-2xl sketch-shadow sketch-shadow-hover transition-all text-center flex flex-col justify-center items-center">
                <div class="w-16 h-16 bg-brand-mustard/20 text-brand-mustard text-3xl rounded-full flex items-center justify-center mb-4">🐶</div>
                <h3 class="font-black text-xl text-brand-dark mb-2">Dibujos de animales y personajes</h3>
                <p class="text-xs text-brand-dark/70">Tus mascotas queridas o personajes favoritos plasmados con todo el detalle.</p>
            </div>
            <div class="bg-brand-cardBg border-3 border-brand-dark p-6 rounded-2xl sketch-shadow sketch-shadow-hover transition-all text-center flex flex-col justify-center items-center">
                <div class="w-16 h-16 bg-brand-pink/20 text-brand-pink text-3xl rounded-full flex items-center justify-center mb-4">👩‍❤️‍👨</div>
                <h3 class="font-black text-xl text-brand-dark mb-2">Dibujos de parejas</h3>
                <p class="text-xs text-brand-dark/70">Ilustraciones románticas e inolvidables para aniversarios y fechas especiales.</p>
            </div>
            <div class="bg-brand-cardBg border-3 border-brand-dark p-6 rounded-2xl sketch-shadow sketch-shadow-hover transition-all text-center flex flex-col justify-center items-center">
                <div class="w-16 h-16 bg-brand-blue/20 text-brand-blue text-3xl rounded-full flex items-center justify-center mb-4">🎨</div>
                <h3 class="font-black text-xl text-brand-dark mb-2">Pinturas</h3>
                <p class="text-xs text-brand-dark/70">Obras a color en diversas técnicas artísticas llenas de vida y expresión.</p>
            </div>
            <div class="bg-brand-cardBg border-3 border-brand-dark p-6 rounded-2xl sketch-shadow sketch-shadow-hover transition-all text-center flex flex-col justify-center items-center">
                <div class="w-16 h-16 bg-brand-terracotta/20 text-brand-terracotta text-3xl rounded-full flex items-center justify-center mb-4">🖼️</div>
                <h3 class="font-black text-xl text-brand-dark mb-2">Retratos</h3>
                <p class="text-xs text-brand-dark/70">Retratos artísticos detallados para inmortalizar tus mejores fotos.</p>
            </div>
        </div>
    </section>

    <!-- MISIÓN Y VISIÓN -->
    <section id="mision-vision" class="py-12 px-4 max-w-6xl mx-auto">
        <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
            <div class="bg-white border-3 border-brand-dark p-8 rounded-3xl sketch-shadow">
                <div class="text-4xl mb-3">🎯</div>
                <h3 class="text-2xl font-black text-brand-terracotta mb-3">Nuestra Misión</h3>
                <p class="text-brand-dark/80 leading-relaxed text-sm md:text-base">
                    Crear arte accesible y personalizado que transforme los sentimientos, historias y recuerdos inolvidables de nuestros clientes en dibujos y pinturas de alta calidad estética y emocional.
                </p>
            </div>
            <div class="bg-white border-3 border-brand-dark p-8 rounded-3xl sketch-shadow">
                <div class="text-4xl mb-3">🌟</div>
                <h3 class="text-2xl font-black text-brand-blue mb-3">Nuestra Visión</h3>
                <p class="text-brand-dark/80 leading-relaxed text-sm md:text-base">
                    Ser la marca referente de regalos personalizados y arte por encargo más querida, destacándonos por la autenticidad, sensibilidad y dedicación en cada detalle.
                </p>
            </div>
        </div>
    </section>

    <!-- CATÁLOGO DE REGALOS -->
    <section id="catalogo" class="py-12 px-4 max-w-6xl mx-auto">
        <h2 class="text-3xl md:text-4xl font-black text-center text-brand-terracotta mb-2">
            Catálogo de Regalos DRAWS POI
        </h2>
        <p class="text-center text-brand-dark/70 mb-8 font-bold">Explora nuestros productos y sus precios en COP</p>

        <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6">
            <!-- Item 1: Dibujos -->
            <div class="bg-white border-3 border-brand-dark rounded-2xl overflow-hidden sketch-shadow sketch-shadow-hover transition-all">
                <div class="h-56 bg-gray-100 overflow-hidden relative">
                    <img src="https://lh3.googleusercontent.com/d/1Ssk2g89jE1AylZ_6e8_0qV3HwJmO6_1Y" alt="Dibujos a lápiz" class="w-full h-full object-cover">
                    <span class="absolute top-3 right-3 bg-brand-terracotta text-white font-black text-xs px-3 py-1 rounded-full border border-brand-dark">
                        $6.000 COP
                    </span>
                </div>
                <div class="p-5">
                    <h3 class="font-black text-lg text-brand-dark mb-1">Dibujos</h3>
                    <p class="text-xs text-brand-dark/70 mb-4">Ilustraciones a lápiz o tinta con tus elementos o bocetos favoritos.</p>
                    <a href="https://wa.me/573202239202?text=Hola,%20quiero%20pedir%20el%20producto:%20Dibujos%20(6.000%20COP)" target="_blank" class="block text-center w-full bg-brand-mustard text-white font-bold py-2 rounded-xl border-2 border-brand-dark hover:bg-brand-terracotta transition-colors text-xs">
                        Pedir por WhatsApp
                    </a>
                </div>
            </div>

            <!-- Item 2: Dibujos de animales -->
            <div class="bg-white border-3 border-brand-dark rounded-2xl overflow-hidden sketch-shadow sketch-shadow-hover transition-all">
                <div class="h-56 bg-brand-cream/50 flex items-center justify-center relative text-6xl">
                    🐶🐱
                    <span class="absolute top-3 right-3 bg-brand-terracotta text-white font-black text-xs px-3 py-1 rounded-full border border-brand-dark">
                        $7.000 COP
                    </span>
                </div>
                <div class="p-5">
                    <h3 class="font-black text-lg text-brand-dark mb-1">Dibujos de animales</h3>
                    <p class="text-xs text-brand-dark/70 mb-4">Retratos adorables y detallados de tus queridas mascotas.</p>
                    <a href="https://wa.me/573202239202?text=Hola,%20quiero%20pedir%20el%20producto:%20Dibujos%20de%20animales%20(7.000%20COP)" target="_blank" class="block text-center w-full bg-brand-mustard text-white font-bold py-2 rounded-xl border-2 border-brand-dark hover:bg-brand-terracotta transition-colors text-xs">
                        Pedir por WhatsApp
                    </a>
                </div>
            </div>

            <!-- Item 3: Dibujos de personajes -->
            <div class="bg-white border-3 border-brand-dark rounded-2xl overflow-hidden sketch-shadow sketch-shadow-hover transition-all">
                <div class="h-56 bg-brand-cream/50 flex items-center justify-center relative text-6xl">
                    🦸‍♂️🎨
                    <span class="absolute top-3 right-3 bg-brand-terracotta text-white font-black text-xs px-3 py-1 rounded-full border border-brand-dark">
                        $7.000 COP
                    </span>
                </div>
                <div class="p-5">
                    <h3 class="font-black text-lg text-brand-dark mb-1">Dibujos de personajes</h3>
                    <p class="text-xs text-brand-dark/70 mb-4">Tus personajes de ánime, películas o series favoritos a pedido.</p>
                    <a href="https://wa.me/573202239202?text=Hola,%20quiero%20pedir%20el%20producto:%20Dibujos%20de%20personajes%20(7.000%20COP)" target="_blank" class="block text-center w-full bg-brand-mustard text-white font-bold py-2 rounded-xl border-2 border-brand-dark hover:bg-brand-terracotta transition-colors text-xs">
                        Pedir por WhatsApp
                    </a>
                </div>
            </div>

            <!-- Item 4: Dibujos de parejas -->
            <div class="bg-white border-3 border-brand-dark rounded-2xl overflow-hidden sketch-shadow sketch-shadow-hover transition-all">
                <div class="h-56 bg-brand-cream/50 flex items-center justify-center relative text-6xl">
                    👩‍❤️‍👨💖
                    <span class="absolute top-3 right-3 bg-brand-terracotta text-white font-black text-xs px-3 py-1 rounded-full border border-brand-dark">
                        $8.000 COP
                    </span>
                </div>
                <div class="p-5">
                    <h3 class="font-black text-lg text-brand-dark mb-1">Dibujos de parejas</h3>
                    <p class="text-xs text-brand-dark/70 mb-4">Un recuerdo romántico y especial para inmortalizar momentos juntos.</p>
                    <a href="https://wa.me/573202239202?text=Hola,%20quiero%20pedir%20el%20producto:%20Dibujos%20de%20parejas%20(8.000%20COP)" target="_blank" class="block text-center w-full bg-brand-mustard text-white font-bold py-2 rounded-xl border-2 border-brand-dark hover:bg-brand-terracotta transition-colors text-xs">
                        Pedir por WhatsApp
                    </a>
                </div>
            </div>

            <!-- Item 5: Pinturas -->
            <div class="bg-white border-3 border-brand-dark rounded-2xl overflow-hidden sketch-shadow sketch-shadow-hover transition-all">
                <div class="h-56 bg-brand-cream/50 flex items-center justify-center relative text-6xl">
                    🖼️✨
                    <span class="absolute top-3 right-3 bg-brand-terracotta text-white font-black text-xs px-3 py-1 rounded-full border border-brand-dark">
                        $10.000 COP
                    </span>
                </div>
                <div class="p-5">
                    <h3 class="font-black text-lg text-brand-dark mb-1">Pinturas</h3>
                    <p class="text-xs text-brand-dark/70 mb-4">Obras a todo color elaboradas en lienzo o papel técnico de alta calidad.</p>
                    <a href="https://wa.me/573202239202?text=Hola,%20quiero%20pedir%20el%20producto:%20Pinturas%20(10.000%20COP)" target="_blank" class="block text-center w-full bg-brand-mustard text-white font-bold py-2 rounded-xl border-2 border-brand-dark hover:bg-brand-terracotta transition-colors text-xs">
                        Pedir por WhatsApp
                    </a>
                </div>
            </div>

            <!-- Item 6: Retratos para parejas -->
            <div class="bg-white border-3 border-brand-dark rounded-2xl overflow-hidden sketch-shadow sketch-shadow-hover transition-all">
                <div class="h-56 bg-brand-cream/50 flex items-center justify-center relative text-6xl">
                    💑🎨
                    <span class="absolute top-3 right-3 bg-brand-terracotta text-white font-black text-xs px-3 py-1 rounded-full border border-brand-dark">
                        $10.500 COP
                    </span>
                </div>
                <div class="p-5">
                    <h3 class="font-black text-lg text-brand-dark mb-1">Retratos para parejas</h3>
                    <p class="text-xs text-brand-dark/70 mb-4">Retratos artísticos acabados con máximo detalle expresivo para regalar.</p>
                    <a href="https://wa.me/573202239202?text=Hola,%20quiero%20pedir%20el%20producto:%20Retratos%20para%20parejas%20(10.500%20COP)" target="_blank" class="block text-center w-full bg-brand-mustard text-white font-bold py-2 rounded-xl border-2 border-brand-dark hover:bg-brand-terracotta transition-colors text-xs">
                        Pedir por WhatsApp
                    </a>
                </div>
            </div>
        </div>
    </section>

<!-- CÓDIGO QR PARA TU SITIO WEB O WHATSAPP -->
<div style="text-align: center; padding: 20px; background-color: #FFFDF9; border: 2px solid #2D221E; border-radius: 16px; max-width: 300px; margin: 20px auto;">
    <h3 style="color: #B33B24; margin-bottom: 10px; font-family: sans-serif;">¡Escanéanos! 📲</h3>
    
    <!-- Imagen del código QR -->
    <img src="https://api.qrserver.com/v1/create-qr-code/?size=200x200&data=https://wa.me/573202239202?text=Hola%20Draws%20Poi,%20quiero%20hacer%20un%20pedido" 
         alt="Código QR DRAWS POI" 
         style="width: 180px; height: 180px; border-radius: 8px; border: 1px solid #ccc; padding: 5px; background: white;">
    
    <p style="font-size: 12px; color: #555; margin-top: 10px; font-family: sans-serif;">
        Abre la cámara de tu celular para hacer tu pedido directo.
    </p>
</div>
</html>
