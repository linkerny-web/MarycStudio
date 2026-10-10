<!-- Tailwind CSS -->
<script src="https://cdn.tailwindcss.com"></script>
<script>
    tailwind.config = {
        theme: {
            extend: {
                colors: {
                    nude: {
                        50: '#FAF6F0',
                        100: '#F4ECE1',
                        200: '#E8D8C8',
                        300: '#DCC3AF',
                        400: '#D0AF96',
                        500: '#C49B7E',
                    },
                    rosewood: '#A36868',
                    warmgray: '#786C66',
                    blush: '#FDF8F5',
                },
                fontFamily: {
                    serif: ['Playfair Display', 'serif'],
                    sans: ['Plus Jakarta Sans', 'sans-serif'],
                }
            }
        }
    }
</script>
<!-- Fonts Google -->
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,600;1,400&family=Plus+Jakarta+Sans:wght@300;400;500;600&display=swap" rel="stylesheet">
<!-- Lucide Icons -->
<script src="https://unpkg.com/lucide@latest"></script>
<style>
    body {
        font-family: 'Plus Jakarta Sans', sans-serif;
        background-color: #FAF6F0;
        color: #4A423E;
    }
    .font-serif {
        font-family: 'Playfair Display', serif;
    }
    .glass-card {
        background: rgba(255, 255, 255, 0.85);
        backdrop-filter: blur(12px);
        border: 1px solid rgba(228, 216, 200, 0.6);
    }
    .pulse-glow {
        box-shadow: 0 0 0 0 rgba(34, 197, 94, 0.7);
        animation: pulse-green 2s infinite;
    }
    @keyframes pulse-green {
        0% {
            box-shadow: 0 0 0 0 rgba(34, 197, 94, 0.7);
        }
        70% {
            box-shadow: 0 0 0 14px rgba(34, 197, 94, 0);
        }
        100% {
            box-shadow: 0 0 0 0 rgba(34, 197, 94, 0);
        }
    }
</style>

<!-- Header / Navbar -->
<header class="fixed top-0 left-0 right-0 z-50 transition-all duration-300 bg-nude-50/90 backdrop-blur-md border-b border-nude-200/60">
    <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8 h-20 flex items-center justify-between">
        <a href="#" class="flex flex-col">
            <span class="font-serif text-2xl tracking-wide text-gray-800 font-semibold">MaryStudios</span>
            <span class="text-[10px] tracking-[0.25em] uppercase text-rosewood font-medium">Nail Art & Beauty Studio v2.0</span>
        </a>
        
        <!-- Desktop Nav -->
        <nav class="hidden md:flex items-center space-x-8 text-sm font-medium text-warmgray">
            <a href="#sobre-mi" class="hover:text-rosewood transition-colors">Sobre Mí</a>
            <a href="#servicios" class="hover:text-rosewood transition-colors">Servicios</a>
            <a href="#como-agendar" class="hover:text-rosewood transition-colors">¿Cómo Agendar?</a>
            <a href="#galeria" class="hover:text-rosewood transition-colors">Galería</a>
            <a href="#testimonios" class="hover:text-rosewood transition-colors">Opiniones</a>
            <a href="#faq" class="hover:text-rosewood transition-colors">Preguntas</a>
            <a href="#contacto" class="hover:text-rosewood transition-colors">Ubicación</a>
        </nav>

        <div class="hidden md:flex items-center space-x-3">
            <a href="https://wa.me/56975509801?text=Hola%20MaryStudios,%20me%20gustaría%20agendar%20una%20cita" target="_blank" class="px-5 py-2.5 bg-rosewood text-white rounded-full text-xs tracking-wider uppercase hover:bg-rosewood/90 transition-all shadow-md hover:shadow-lg flex items-center gap-2">
                <i data-lucide="calendar" class="w-4 h-4"></i> Agendar Cita
            </a>
        </div>

        <!-- Mobile menu button -->
        <button id="mobile-menu-btn" class="md:hidden p-2 text-warmgray hover:text-gray-900 focus:outline-none" aria-label="Abrir menú">
            <i data-lucide="menu" class="w-6 h-6"></i>
        </button>
    </div>

    <!-- Mobile Navigation Drawer -->
    <div id="mobile-menu" class="hidden md:hidden bg-nude-50/95 backdrop-blur-lg border-b border-nude-200 px-6 py-6 space-y-4">
        <a href="#sobre-mi" class="block text-gray-700 font-medium py-2 hover:text-rosewood">Sobre Mí</a>
        <a href="#servicios" class="block text-gray-700 font-medium py-2 hover:text-rosewood">Servicios</a>
        <a href="#como-agendar" class="block text-gray-700 font-medium py-2 hover:text-rosewood">Pasos para Agendar</a>
        <a href="#galeria" class="block text-gray-700 font-medium py-2 hover:text-rosewood">Galería de Uñas</a>
        <a href="#testimonios" class="block text-gray-700 font-medium py-2 hover:text-rosewood">Opiniones de Clientes</a>
        <a href="#faq" class="block text-gray-700 font-medium py-2 hover:text-rosewood">Preguntas Frecuentes</a>
        <a href="#contacto" class="block text-gray-700 font-medium py-2 hover:text-rosewood">Ubicación & Contacto</a>
        <div class="pt-4 flex flex-col gap-3">
            <a href="https://wa.me/56975509801?text=Hola%20MaryStudios,%20me%20gustaría%20agendar%20una%20cita" target="_blank" class="w-full text-center py-3 bg-rosewood text-white rounded-full text-xs tracking-wider uppercase font-medium flex items-center justify-center gap-2">
                <i data-lucide="message-circle" class="w-4 h-4"></i> Reservar por WhatsApp
            </a>
        </div>
    </div>
</header>

<!-- Hero Section -->
<section class="pt-32 pb-16 md:pt-40 md:pb-24 px-4 sm:px-6 lg:px-8 max-w-6xl mx-auto">
    <div class="grid grid-cols-1 md:grid-cols-12 gap-12 items-center">
        <div class="md:col-span-7 space-y-6 text-left">
            <div class="inline-flex items-center gap-2 px-3 py-1.5 rounded-full bg-nude-200/60 border border-nude-300 text-xs font-medium text-warmgray">
                <span class="w-2 h-2 rounded-full bg-emerald-500 animate-pulse"></span>
                Agenda Abierta · Quilicura
            </div>
            <h1 class="font-serif text-4xl sm:text-5xl lg:text-6xl text-gray-900 font-medium leading-[1.15]">
                Arte, elegancia y cuidado <br class="hidden sm:inline"/>
                <span class="italic font-normal text-rosewood">para tus manos.</span>
            </h1>
            <p class="text-base sm:text-lg text-warmgray font-light leading-relaxed max-w-xl">
                Bienvenida a MaryStudios, un espacio exclusivo donde la estética, la salud de tus uñas y los diseños personalizados más creativos se combinan para realzar tu belleza.
            </p>
            <div class="pt-2 flex flex-wrap gap-4 items-center">
                <a href="https://wa.me/56975509801?text=Hola%20MaryStudios,%20quisiera%20consultar%20por%20disponibilidad" target="_blank" class="px-7 py-3.5 bg-rosewood text-white rounded-full text-sm font-medium hover:bg-rosewood/90 transition-all shadow-lg hover:shadow-xl flex items-center gap-2">
                    <i data-lucide="message-circle" class="w-4 h-4"></i> Consultar Disponibilidad
                </a>
                <a href="https://instagram.com/mary_carmen_garrido" target="_blank" class="px-6 py-3.5 border border-nude-300 hover:border-rosewood text-gray-800 rounded-full text-sm font-medium transition-all flex items-center gap-2 bg-white/50 hover:bg-white">
                    <i data-lucide="instagram" class="w-4 h-4 text-rosewood"></i> Ver Instagram
                </a>
            </div>

            <!-- Metodos de pago aceptados -->
            <div class="pt-4 flex items-center gap-3 text-xs text-warmgray">
                <span class="font-medium">Pagos aceptados:</span>
                <span class="px-2.5 py-1 bg-white rounded-md border border-nude-200 text-gray-700 shadow-sm flex items-center gap-1">
                    <i data-lucide="credit-card" class="w-3.5 h-3.5 text-rosewood"></i> Transferencia
                </span>
                <span class="px-2.5 py-1 bg-white rounded-md border border-nude-200 text-gray-700 shadow-sm flex items-center gap-1">
                    <i data-lucide="banknote" class="w-3.5 h-3.5 text-rosewood"></i> Efectivo
                </span>
            </div>
        </div>

        <div class="md:col-span-5 relative">
            <div class="relative mx-auto max-w-xs sm:max-w-sm md:max-w-none">
                <div class="aspect-[4/5] rounded-3xl overflow-hidden shadow-2xl border-4 border-white">
                    <img src="https://images.unsplash.com/photo-1604654894610-df63bc536371?q=80&w=800&auto=format&fit=crop" 
                         alt="Fotografía de manos con manicura perfecta y diseño delicado en MaryStudios" 
                         class="w-full h-full object-cover transform hover:scale-105 transition-all duration-500">
                </div>
                <!-- Badge superpuesto -->
                <div class="absolute -bottom-6 -left-6 glass-card p-4 rounded-2xl shadow-xl flex items-center gap-3 border border-white">
                    <div class="w-12 h-12 rounded-full bg-nude-200 flex items-center justify-center text-rosewood">
                        <i data-lucide="award" class="w-6 h-6"></i>
                    </div>
                    <div>
                        <p class="text-xs text-warmgray font-medium">Trayectoria profesional</p>
                        <p class="font-serif text-lg font-semibold text-gray-900">+5 Años de Experiencia</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</section>

<!-- Sobre Mí -->
<section id="sobre-mi" class="py-20 bg-nude-100/50 border-y border-nude-200/60">
    <div class="max-w-5xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="grid grid-cols-1 md:grid-cols-12 gap-10 items-center">
            <div class="md:col-span-5 relative">
                <div class="aspect-[4/5] rounded-2xl overflow-hidden shadow-lg border border-white">
                    <img src="https://images.unsplash.com/photo-1607779097040-26e80aa78e66?q=80&w=800&auto=format&fit=crop" 
                         alt="Manos cuidadas con manicura impecable" 
                         class="w-full h-full object-cover">
                </div>
            </div>
            
            <div class="md:col-span-7 space-y-6">
                <div class="space-y-2">
                    <span class="text-rosewood text-xs tracking-widest uppercase font-semibold">Experiencia y Dedicación</span>
                    <h2 class="font-serif text-3xl sm:text-4xl text-gray-900 font-medium">Mary Carmen Garrido</h2>
                    <div class="w-12 h-0.5 bg-rosewood"></div>
                </div>

                <!-- Descripción detallada >40 palabras -->
                <div class="text-gray-700 leading-relaxed font-light text-base space-y-4">
                    <p class="text-lg text-gray-800 font-normal italic">
                        "En MaryStudios cada cita es un momento dedicado a potenciar tu elegancia y brindarle el mejor cuidado a tus manos."
                    </p>
                    <p>
                        Con más de 5 años de constante trayectoria profesional en la estética de uñas, ofrezco una atención totalmente personalizada, enfocada en la comodidad y satisfacción de cada clienta. Mi compromiso primordial es entregarte una experiencia excepcional con insumos de primera calidad, asegurando acabados duraderos, detallistas e impecables que protegen la salud de tus uñas.
                    </p>
                    <p>
                        Especializada en una amplia gama de tendencias modernas y clásicas, realizo cualquier tipo de diseño que te imagines, adaptándome totalmente a tu gusto único para crear obras de arte únicas en tus manos.
                    </p>
                </div>

                <div class="grid grid-cols-3 gap-4 pt-4 border-t border-nude-200">
                    <div>
                        <p class="font-serif text-2xl font-semibold text-rosewood">5+ </p>
                        <p class="text-xs text-warmgray">Años en el Rubro</p>
                    </div>
                    <div>
                        <p class="font-serif text-2xl font-semibold text-rosewood">100%</p>
                        <p class="text-xs text-warmgray">Diseños a Medida</p>
                    </div>
                    <div>
                        <p class="font-serif text-2xl font-semibold text-rosewood">★ 5.0</p>
                        <p class="text-xs text-warmgray">Atención Exclusiva</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</section>

<!-- Servicios Destacados -->
<section id="servicios" class="py-20 max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
    <div class="text-center max-w-2xl mx-auto mb-16 space-y-3">
        <span class="text-rosewood text-xs tracking-widest uppercase font-semibold">Especialidades de MaryStudios</span>
        <h2 class="font-serif text-3xl sm:text-4xl text-gray-900 font-medium">Servicios Destacados</h2>
        <p class="text-warmgray text-sm font-light">
            Trabajamos con una gran variedad de técnicas avanzadas para mantener tus uñas fuertes, saludables y siempre estéticas.
        </p>
    </div>

    <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
        <!-- Servicio 1 -->
        <div class="bg-white p-8 rounded-2xl shadow-sm border border-nude-200 hover:shadow-md transition-all group">
            <div class="w-12 h-12 rounded-xl bg-nude-100 flex items-center justify-center text-rosewood mb-6 group-hover:bg-rosewood group-hover:text-white transition-colors">
                <i data-lucide="sparkles" class="w-6 h-6"></i>
            </div>
            <h3 class="font-serif text-xl font-semibold text-gray-900 mb-2">Esmaltado Permanente</h3>
            <p class="text-warmgray text-sm font-light mb-4">
                Brillo y color de larga duración que conserva su intensidad por semanas sin desgastarse, garantizando la protección de tu uña natural.
            </p>
            <span class="text-xs font-semibold text-rosewood tracking-wider uppercase">Durabilidad & Brillo Impecable</span>
        </div>

        <!-- Servicio 2 -->
        <div class="bg-white p-8 rounded-2xl shadow-sm border border-nude-200 hover:shadow-md transition-all group relative overflow-hidden">
            <div class="absolute top-3 right-3 bg-rosewood/10 text-rosewood text-[10px] font-bold px-2.5 py-1 rounded-full uppercase tracking-wider">Favorito</div>
            <div class="w-12 h-12 rounded-xl bg-nude-100 flex items-center justify-center text-rosewood mb-6 group-hover:bg-rosewood group-hover:text-white transition-colors">
                <i data-lucide="palette" class="w-6 h-6"></i>
            </div>
            <h3 class="font-serif text-xl font-semibold text-gray-900 mb-2">Diseños Personalizados (Nail Art)</h3>
            <p class="text-warmgray text-sm font-light mb-4">
                Realizamos cualquier tipo de diseño a pedido: mano alzada, cristales, efecto baby boomer, estilo francés moderno y creaciones exclusivas.
            </p>
            <span class="text-xs font-semibold text-rosewood tracking-wider uppercase">Creatividad Sin Límites</span>
        </div>

        <!-- Servicio 3 -->
        <div class="bg-white p-8 rounded-2xl shadow-sm border border-nude-200 hover:shadow-md transition-all group">
            <div class="w-12 h-12 rounded-xl bg-nude-100 flex items-center justify-center text-rosewood mb-6 group-hover:bg-rosewood group-hover:text-white transition-colors">
                <i data-lucide="gem" class="w-6 h-6"></i>
            </div>
            <h3 class="font-serif text-xl font-semibold text-gray-900 mb-2">Soft Gel & Uñas Esculpidas</h3>
            <p class="text-warmgray text-sm font-light mb-4">
                Extensiones ligeras y altamente resistentes que te permiten lucir el largo y la forma deseada con una apariencia completamente natural.
            </p>
            <span class="text-xs font-semibold text-rosewood tracking-wider uppercase">Resistencia & Estilo</span>
        </div>
    </div>
</section>

<!-- Sección ¿Cómo Agendar en 3 Pasos? -->
<section id="como-agendar" class="py-16 bg-white border-y border-nude-200">
    <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="text-center max-w-xl mx-auto mb-12">
            <span class="text-rosewood text-xs tracking-widest uppercase font-semibold">Fácil y Rápido</span>
            <h2 class="font-serif text-3xl text-gray-900 font-medium">¿Cómo Agendar tu Cita?</h2>
            <p class="text-warmgray text-sm mt-1">Sigue estos tres sencillos pasos para asegurar tu horario con MaryStudios</p>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-3 gap-8 relative">
            <div class="bg-nude-50 p-6 rounded-2xl border border-nude-200 relative text-center flex flex-col items-center">
                <div class="w-10 h-10 rounded-full bg-rosewood text-white font-bold flex items-center justify-center mb-4 text-sm">1</div>
                <h3 class="font-serif text-lg font-semibold text-gray-900 mb-2">Elige tu Diseño e Idea</h3>
                <p class="text-warmgray text-xs font-light leading-relaxed">
                    Navega por nuestra galería o guarda una foto de la referencia o estilo que te gustaría lucir en tus manos.
                </p>
            </div>

            <div class="bg-nude-50 p-6 rounded-2xl border border-nude-200 relative text-center flex flex-col items-center">
                <div class="w-10 h-10 rounded-full bg-rosewood text-white font-bold flex items-center justify-center mb-4 text-sm">2</div>
                <h3 class="font-serif text-lg font-semibold text-gray-900 mb-2">Escríbenos a WhatsApp</h3>
                <p class="text-warmgray text-xs font-light leading-relaxed">
                    Haz clic en el botón de WhatsApp e indícanos el servicio de tu interés y la fecha u hora que mejor te acomode.
                </p>
            </div>

            <div class="bg-nude-50 p-6 rounded-2xl border border-nude-200 relative text-center flex flex-col items-center">
                <div class="w-10 h-10 rounded-full bg-rosewood text-white font-bold flex items-center justify-center mb-4 text-sm">3</div>
                <h3 class="font-serif text-lg font-semibold text-gray-900 mb-2">¡Confirma y Disfruta!</h3>
                <p class="text-warmgray text-xs font-light leading-relaxed">
                    Coordinamos los detalles finales, reservamos tu cupo y te esperamos en nuestro cómodo estudio de Quilicura.
                </p>
            </div>
        </div>
    </div>
</section>

<!-- Galería de Trabajos -->
<section id="galeria" class="py-20 bg-nude-100/40">
    <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="flex flex-col md:flex-row md:items-end justify-between mb-12">
            <div>
                <span class="text-rosewood text-xs tracking-widest uppercase font-semibold">Portafolio MaryStudios</span>
                <h2 class="font-serif text-3xl sm:text-4xl text-gray-900 font-medium">Galería de Trabajos en Manos</h2>
                <p class="text-warmgray text-sm font-light mt-1">Descubre la diversidad de estilos, acabados y Nail Art creados especialmente en las manos de nuestras clientas.</p>
            </div>
            <a href="https://instagram.com/mary_carmen_garrido" target="_blank" class="mt-4 md:mt-0 text-sm text-rosewood font-medium flex items-center gap-1 hover:underline">
                Ver más publicaciones en @mary_carmen_garrido <i data-lucide="arrow-up-right" class="w-4 h-4"></i>
            </a>
        </div>

        <div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-4">
            <div class="relative group overflow-hidden rounded-2xl shadow-sm aspect-square bg-gray-200">
                <img src="https://images.unsplash.com/photo-1604654894610-df63bc536371?q=80&w=600&auto=format&fit=crop" 
                     alt="Manos con uñas nude minimalistas" 
                     class="w-full h-full object-cover group-hover:scale-110 transition-transform duration-500">
                <div class="absolute inset-0 bg-gradient-to-t from-black/60 via-transparent to-transparent opacity-0 group-hover:opacity-100 transition-opacity flex items-end p-4 text-white">
                    <span class="text-xs font-medium">Nude Elegante & Minimalista</span>
                </div>
            </div>

            <div class="relative group overflow-hidden rounded-2xl shadow-sm aspect-square bg-gray-200">
                <img src="https://images.unsplash.com/photo-1599948128020-9a44505b0d1b?q=80&w=600&auto=format&fit=crop" 
                     alt="Detalle de manos con pedrería y glitter" 
                     class="w-full h-full object-cover group-hover:scale-110 transition-transform duration-500">
                <div class="absolute inset-0 bg-gradient-to-t from-black/60 via-transparent to-transparent opacity-0 group-hover:opacity-100 transition-opacity flex items-end p-4 text-white">
                    <span class="text-xs font-medium">Nail Art con Pedrería</span>
                </div>
            </div>

            <div class="relative group overflow-hidden rounded-2xl shadow-sm aspect-square bg-gray-200">
                <img src="https://images.unsplash.com/photo-1632345031435-8727fec88f2d?q=80&w=600&auto=format&fit=crop" 
                     alt="Manos luciendo esmaltado rosa pastel" 
                     class="w-full h-full object-cover group-hover:scale-110 transition-transform duration-500">
                <div class="absolute inset-0 bg-gradient-to-t from-black/60 via-transparent to-transparent opacity-0 group-hover:opacity-100 transition-opacity flex items-end p-4 text-white">
                    <span class="text-xs font-medium">Soft Gel Tono Pastel</span>
                </div>
            </div>

            <div class="relative group overflow-hidden rounded-2xl shadow-sm aspect-square bg-gray-200">
                <img src="https://images.unsplash.com/photo-1607779097040-26e80aa78e66?q=80&w=600&auto=format&fit=crop" 
                     alt="Mano con uñas francesas modernas" 
                     class="w-full h-full object-cover group-hover:scale-110 transition-transform duration-500">
                <div class="absolute inset-0 bg-gradient-to-t from-black/60 via-transparent to-transparent opacity-0 group-hover:opacity-100 transition-opacity flex items-end p-4 text-white">
                    <span class="text-xs font-medium">Estilo Francés Moderno</span>
                </div>
            </div>

            <div class="relative group overflow-hidden rounded-2xl shadow-sm aspect-square bg-gray-200">
                <img src="https://images.unsplash.com/photo-1519014816548-bf5fe059798b?q=80&w=600&auto=format&fit=crop" 
                     alt="Diseño de uñas a mano alzada en manos" 
                     class="w-full h-full object-cover group-hover:scale-110 transition-transform duration-500">
                <div class="absolute inset-0 bg-gradient-to-t from-black/60 via-transparent to-transparent opacity-0 group-hover:opacity-100 transition-opacity flex items-end p-4 text-white">
                    <span class="text-xs font-medium">Diseño A Mano Alzada</span>
                </div>
            </div>

            <div class="relative group overflow-hidden rounded-2xl shadow-sm aspect-square bg-gray-200">
                <img src="https://images.unsplash.com/photo-1522337360788-8b13dee7a37e?q=80&w=600&auto=format&fit=crop" 
                     alt="Manicura impecable en manos delicadas" 
                     class="w-full h-full object-cover group-hover:scale-110 transition-transform duration-500">
                <div class="absolute inset-0 bg-gradient-to-t from-black/60 via-transparent to-transparent opacity-0 group-hover:opacity-100 transition-opacity flex items-end p-4 text-white">
                    <span class="text-xs font-medium">Uñas Esculpidas Perfeccionadas</span>
                </div>
            </div>

            <div class="relative group overflow-hidden rounded-2xl shadow-sm aspect-square bg-gray-200">
                <img src="https://images.unsplash.com/photo-1604654894610-df63bc536371?q=80&w=600&auto=format&fit=crop" 
                     alt="Detalle de manicura impecable con acabado ultra brillante" 
                     class="w-full h-full object-cover group-hover:scale-110 transition-transform duration-500">
                <div class="absolute inset-0 bg-gradient-to-t from-black/60 via-transparent to-transparent opacity-0 group-hover:opacity-100 transition-opacity flex items-end p-4 text-white">
                    <span class="text-xs font-medium">Acabado Brillante Larga Duración</span>
                </div>
            </div>

            <div class="relative group overflow-hidden rounded-2xl shadow-sm aspect-square bg-gray-200">
                <img src="https://images.unsplash.com/photo-1610992015732-2449b76344bc?q=80&w=600&auto=format&fit=crop" 
                     alt="Manos con combinación de colores de temporada" 
                     class="w-full h-full object-cover group-hover:scale-110 transition-transform duration-500">
                <div class="absolute inset-0 bg-gradient-to-t from-black/60 via-transparent to-transparent opacity-0 group-hover:opacity-100 transition-opacity flex items-end p-4 text-white">
                    <span class="text-xs font-medium">Tendencias de Temporada</span>
                </div>
            </div>
        </div>
    </div>
</section>

<!-- Testimonios de Clientas -->
<section id="testimonios" class="py-20 bg-white border-t border-nude-200">
    <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="text-center max-w-xl mx-auto mb-14">
            <span class="text-rosewood text-xs tracking-widest uppercase font-semibold">Experiencias Reales</span>
            <h2 class="font-serif text-3xl sm:text-4xl text-gray-900 font-medium">Lo que opinan nuestras clientas</h2>
            <p class="text-warmgray text-sm mt-1 font-light">La satisfacción y la durabilidad en tus uñas es nuestra mayor garantía</p>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
            <div class="bg-nude-50 p-6 rounded-2xl border border-nude-200 flex flex-col justify-between">
                <div class="space-y-3">
                    <div class="flex text-amber-400 gap-1 text-sm">★★★★★</div>
                    <p class="text-xs text-gray-700 italic leading-relaxed">
                        "Excelente atención. Mary es muy detallista con las cutículas y los acabados. Mis uñas de Soft Gel me duraron intactas casi un mes sin perder el brillo."
                    </p>
                </div>
                <div class="pt-4 border-t border-nude-200/80 mt-4 flex items-center gap-3">
                    <div class="w-8 h-8 rounded-full bg-nude-300 flex items-center justify-center font-bold text-xs text-rosewood">
                        CP
                    </div>
                    <div>
                        <p class="text-xs font-semibold text-gray-900">Camila P.</p>
                        <p class="text-[10px] text-warmgray">Quilicura · Clienta Frecuente</p>
                    </div>
                </div>
            </div>

            <div class="bg-nude-50 p-6 rounded-2xl border border-nude-200 flex flex-col justify-between">
                <div class="space-y-3">
                    <div class="flex text-amber-400 gap-1 text-sm">★★★★★</div>
                    <p class="text-xs text-gray-700 italic leading-relaxed">
                        "Llevé una foto con un diseño a mano alzada muy complejo de Pinterest y Mary lo recreó idéntico. Es súper amable y los productos que usa no dañan la uña."
                    </p>
                </div>
                <div class="pt-4 border-t border-nude-200/80 mt-4 flex items-center gap-3">
                    <div class="w-8 h-8 rounded-full bg-nude-300 flex items-center justify-center font-bold text-xs text-rosewood">
                        VT
                    </div>
                    <div>
                        <p class="text-xs font-semibold text-gray-900">Valentina T.</p>
                        <p class="text-[10px] text-warmgray">Santiago</p>
                    </div>
                </div>
            </div>

            <div class="bg-nude-50 p-6 rounded-2xl border border-nude-200 flex flex-col justify-between">
                <div class="space-y-3">
                    <div class="flex text-amber-400 gap-1 text-sm">★★★★★</div>
                    <p class="text-xs text-gray-700 italic leading-relaxed">
                        "Los precios son totalmente razonables para la tremenda dedicación que entrega. El ambiente es relajante y muy limpio. 100% recomendada."
                    </p>
                </div>
                <div class="pt-4 border-t border-nude-200/80 mt-4 flex items-center gap-3">
                    <div class="w-8 h-8 rounded-full bg-nude-300 flex items-center justify-center font-bold text-xs text-rosewood">
                        MS
                    </div>
                    <div>
                        <p class="text-xs font-semibold text-gray-900">María S.</p>
                        <p class="text-[10px] text-warmgray">Quilicura</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</section>

<!-- Preguntas Frecuentes (FAQ) -->
<section id="faq" class="py-20 bg-nude-100/50 border-t border-nude-200">
    <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="text-center max-w-xl mx-auto mb-12">
            <span class="text-rosewood text-xs tracking-widest uppercase font-semibold">Resuelve tus Dudas</span>
            <h2 class="font-serif text-3xl text-gray-900 font-medium">Preguntas Frecuentes</h2>
        </div>

        <div class="space-y-4">
            <!-- FAQ 1 -->
            <div class="bg-white rounded-2xl border border-nude-200 overflow-hidden shadow-sm transition-all">
                <button class="w-full p-5 text-left flex justify-between items-center font-medium text-gray-900 text-sm focus:outline-none faq-btn">
                    <span>¿Cuánto tiempo dura una sesión de manicura o Soft Gel?</span>
                    <i data-lucide="chevron-down" class="w-4 h-4 text-rosewood transform transition-transform duration-300"></i>
                </button>
                <div class="px-5 pb-5 text-xs text-warmgray leading-relaxed hidden faq-content">
                    El tiempo estimado varía según la técnica. Un esmaltado permanente suele tomar entre 1h a 1h 15 min, mientras que una postura de Soft Gel o uñas esculpidas con Nail Art complejo puede tomar entre 1h 30 min y 2 horas.
                </div>
            </div>

            <!-- FAQ 2 -->
            <div class="bg-white rounded-2xl border border-nude-200 overflow-hidden shadow-sm transition-all">
                <button class="w-full p-5 text-left flex justify-between items-center font-medium text-gray-900 text-sm focus:outline-none faq-btn">
                    <span>¿Debo llevar mi propia foto o diseño?</span>
                    <i data-lucide="chevron-down" class="w-4 h-4 text-rosewood transform transition-transform duration-300"></i>
                </button>
                <div class="px-5 pb-5 text-xs text-warmgray leading-relaxed hidden faq-content">
                    ¡Como prefieras! Puedes enviarnos tu idea previa o foto de referencia por WhatsApp para coordinar el estilo, o podemos asesorarte personalmente en la cita para elegir el diseño y color perfecto para tus manos.
                </div>
            </div>

            <!-- FAQ 3 -->
            <div class="bg-white rounded-2xl border border-nude-200 overflow-hidden shadow-sm transition-all">
                <button class="w-full p-5 text-left flex justify-between items-center font-medium text-gray-900 text-sm focus:outline-none faq-btn">
                    <span>¿Cuáles son las medidas de higiene y cuidado?</span>
                    <i data-lucide="chevron-down" class="w-4 h-4 text-rosewood transform transition-transform duration-300"></i>
                </button>
                <div class="px-5 pb-5 text-xs text-warmgray leading-relaxed hidden faq-content">
                    En MaryStudios la higiene es fundamental. Todas las herramientas metálicas son rigurosamente sanitizadas y esterilizadas antes de cada atención, y utilizamos limas e insumos desechables por protocolo de salud.
                </div>
            </div>

            <!-- FAQ 4 -->
            <div class="bg-white rounded-2xl border border-nude-200 overflow-hidden shadow-sm transition-all">
                <button class="w-full p-5 text-left flex justify-between items-center font-medium text-gray-900 text-sm focus:outline-none faq-btn">
                    <span>¿Qué medios de pago puedo utilizar?</span>
                    <i data-lucide="chevron-down" class="w-4 h-4 text-rosewood transform transition-transform duration-300"></i>
                </button>
                <div class="px-5 pb-5 text-xs text-warmgray leading-relaxed hidden faq-content">
                    Aceptamos transferencias bancarias electrónicas y pago en efectivo al finalizar la atención.
                </div>
            </div>
        </div>
    </div>
</section>

<!-- Ubicación y Citas -->
<section id="contacto" class="py-20 bg-nude-100/60 border-t border-nude-200">
    <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="grid grid-cols-1 md:grid-cols-12 gap-10 items-stretch">
            <!-- Información de contacto -->
            <div class="md:col-span-5 bg-white p-8 sm:p-10 rounded-3xl border border-nude-200 shadow-sm flex flex-col justify-between">
                <div class="space-y-6">
                    <div>
                        <span class="text-rosewood text-xs tracking-widest uppercase font-semibold">Reserva tu Horario</span>
                        <h2 class="font-serif text-3xl text-gray-900 font-medium mt-1">Ubicación & Citas</h2>
                    </div>

                    <div class="space-y-5">
                        <div class="flex items-start gap-4">
                            <div class="w-10 h-10 rounded-full bg-nude-100 flex items-center justify-center text-rosewood shrink-0 mt-1">
                                <i data-lucide="map-pin" class="w-5 h-5"></i>
                            </div>
                            <div>
                                <h4 class="text-xs uppercase font-semibold tracking-wider text-warmgray">Dirección</h4>
                                <p class="text-sm font-medium text-gray-900">Alcaldesa Elisa Álvarez 626</p>
                                <p class="text-xs text-warmgray">Quilicura, Santiago de Chile</p>
                            </div>
                        </div>

                        <div class="flex items-start gap-4">
                            <div class="w-10 h-10 rounded-full bg-nude-100 flex items-center justify-center text-rosewood shrink-0 mt-1">
                                <i data-lucide="phone" class="w-5 h-5"></i>
                            </div>
                            <div>
                                <h4 class="text-xs uppercase font-semibold tracking-wider text-warmgray">Contacto WhatsApp</h4>
                                <a href="https://wa.me/56975509801?text=Hola%20MaryStudios,%20me%20gustaría%20agendar%20una%20cita" target="_blank" class="text-sm font-medium text-gray-900 hover:text-rosewood transition-colors">
                                    +56 9 7550 9801
                                </a>
                            </div>
                        </div>

                        <div class="flex items-start gap-4">
                            <div class="w-10 h-10 rounded-full bg-nude-100 flex items-center justify-center text-rosewood shrink-0 mt-1">
                                <i data-lucide="instagram" class="w-5 h-5"></i>
                            </div>
                            <div>
                                <h4 class="text-xs uppercase font-semibold tracking-wider text-warmgray">Instagram</h4>
                                <a href="https://instagram.com/mary_carmen_garrido" target="_blank" class="text-sm font-medium text-rosewood hover:underline">
                                    @mary_carmen_garrido
                                </a>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Botones de Redes Directas -->
                <div class="pt-8 mt-8 border-t border-nude-200 flex flex-col gap-3">
                    <a href="https://wa.me/56975509801?text=Hola%20MaryStudios,%20quisiera%20agendar%20una%20cita" 
                       target="_blank" 
                       class="w-full py-3.5 bg-emerald-700 text-white rounded-xl text-xs uppercase tracking-wider font-semibold text-center flex items-center justify-center gap-2 shadow hover:bg-emerald-800 transition-colors">
                        <i data-lucide="message-square" class="w-4 h-4"></i> WhatsApp Directo
                    </a>
                    <a href="https://instagram.com/mary_carmen_garrido" 
                       target="_blank" 
                       class="w-full py-3.5 bg-gradient-to-r from-purple-600 via-pink-600 to-rose-500 text-white rounded-xl text-xs uppercase tracking-wider font-semibold text-center flex items-center justify-center gap-2 shadow hover:opacity-90 transition-opacity">
                        <i data-lucide="instagram" class="w-4 h-4"></i> Ir a Instagram
                    </a>
                </div>
            </div>

            <!-- Mapa interactivo embed -->
            <div class="md:col-span-7 bg-white rounded-3xl border border-nude-200 overflow-hidden shadow-sm min-h-[380px] relative">
                <iframe 
                    title="Ubicación MaryStudios Quilicura"
                    class="w-full h-full min-h-[380px] border-0" 
                    src="https://maps.google.com/maps?q=Alcaldesa+Elisa+Alvarez+626,+Quilicura,+Santiago+Chile&t=&z=15&ie=UTF8&iwloc=&output=embed" 
                    allowfullscreen="" 
                    loading="lazy">
                </iframe>
            </div>
        </div>
    </div>
</section>

<!-- Botón Flotante de WhatsApp para Conversión Rápida -->
<a href="https://wa.me/56975509801?text=Hola%20MaryStudios,%20quiero%20agendar%20una%20cita" 
   target="_blank" 
   aria-label="Contactar por WhatsApp"
   class="fixed bottom-6 right-6 z-50 bg-emerald-500 hover:bg-emerald-600 text-white p-4 rounded-full shadow-2xl pulse-glow flex items-center gap-2 transition-all duration-300 transform hover:scale-110">
    <i data-lucide="message-circle" class="w-6 h-6"></i>
    <span class="hidden sm:inline font-medium text-xs tracking-wider pr-1">Agendar Cita</span>
</a>

<!-- Footer -->
<footer class="bg-nude-50 border-t border-nude-200 py-10">
    <div class="max-w-6xl mx-auto px-4 text-center space-y-4">
        <span class="font-serif text-2xl text-gray-800 font-semibold block">MaryStudios</span>
        <p class="text-xs text-warmgray max-w-md mx-auto">
            Estudio profesional de Manicura & Nail Art en Quilicura, Santiago de Chile. Más de 5 años ofreciendo una atención de excelencia.
        </p>
        <div class="pt-4 text-xs text-warmgray/80">
            &copy; <span id="year"></span> MaryStudios - Todos los derechos reservados.
        </div>
    </div>
</footer>

<script>
    // Inicialización de Lucide Icons
    if (window.lucide) {
        lucide.createIcons();
    }

    // Año actual en el footer
    const yearEl = document.getElementById('year');
    if (yearEl) {
        yearEl.textContent = new Date().getFullYear();
    }

    // Menu Mobile Toggle con validación nula segura
    const menuBtn = document.getElementById('mobile-menu-btn');
    const mobileMenu = document.getElementById('mobile-menu');

    if (menuBtn && mobileMenu) {
        menuBtn.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });
    }

    // FAQ Acordeón Interactivo
    const faqBtns = document.querySelectorAll('.faq-btn');
    faqBtns.forEach(btn => {
        btn.addEventListener('click', () => {
            const content = btn.nextElementSibling;
            const icon = btn.querySelector('i');
            
            if (content) {
                content.classList.toggle('hidden');
            }
            if (icon) {
                icon.classList.toggle('rotate-180');
            }
        });
    });
</script>
