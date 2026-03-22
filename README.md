<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>[Nama Anda] - UI/UX Designer</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: { 'sans': ['Inter', 'sans-serif'] },
                    colors: {
                        skyblue: {
                            50: '#f0f9ff',
                            100: '#e0f2fe',
                            200: '#bae6fd',
                            300: '#7dd3fc',
                            400: '#38bdf8',
                            500: '#0ea5e9', // Biru langit utama
                            600: '#0284c7',
                            700: '#0369a1',
                            800: '#075985',
                            900: '#0c4a6e',
                            950: '#082f49'
                        }
                    },
                    animation: {
                        'float': 'float 6s ease-in-out infinite',
                        'fadeInUp': 'fadeInUp 1s ease-out',
                    },
                    keyframes: {
                        float: {
                            '0%, 100%': { transform: 'translate3d(0,0,0)' },
                            '50%': { transform: 'translate3d(0,-10px,0)' },
                        },
                        fadeInUp: {
                            '0%': { opacity: 0, transform: 'translateY(30px)' },
                            '100%': { opacity: 1, transform: 'translateY(0)' },
                        }
                    }
                }
            }
        }
    </script>
</head>
<body class="bg-gradient-to-br from-skyblue-50 via-white to-skyblue-100 text-slate-900 overflow-x-hidden">

    <!-- Navigation -->
    <nav class="fixed top-0 w-full z-50 bg-white/95 backdrop-blur-md border-b border-skyblue-200/50 shadow-sm">
        <div class="max-w-7xl mx-auto px-6 py-4">
            <div class="flex justify-between items-center">
                <a href="#" class="text-2xl font-bold bg-gradient-to-r from-skyblue-500 to-skyblue-600 bg-clip-text text-transparent">
                    [Nama Anda]
                </a>
                <div class="hidden md:flex space-x-8">
                    <a href="#home" class="hover:text-skyblue-500 font-medium transition-all duration-300">Home</a>
                    <a href="#about" class="hover:text-skyblue-500 font-medium transition-all duration-300">About</a>
                    <a href="#works" class="hover:text-skyblue-500 font-medium transition-all duration-300">Works</a>
                    <a href="#contact" class="hover:text-skyblue-500 font-medium transition-all duration-300">Contact</a>
                </div>
                <button class="md:hidden text-skyblue-600">
                    <i class="fas fa-bars text-2xl"></i>
                </button>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="min-h-screen flex items-center justify-center pt-20 px-6 overflow-hidden">
        <div class="text-center max-w-4xl mx-auto animate-fadeInUp">
            <div class="inline-block p-4 bg-gradient-to-r from-skyblue-100 to-skyblue-200 rounded-2xl backdrop-blur-sm border border-skyblue-300/50 mb-8 animate-float">
                <span class="text-sm bg-gradient-to-r from-skyblue-600 to-skyblue-700 bg-clip-text text-transparent font-semibold">UI/UX Designer</span>
            </div>
            <h1 class="text-6xl md:text-7xl font-bold bg-gradient-to-r from-slate-900 via-skyblue-600 to-skyblue-700 bg-clip-text text-transparent mb-6 leading-tight">
                Membuat <span class="bg-gradient-to-r from-skyblue-500 to-skyblue-600">Pengalaman</span><br>
                Digital yang <span class="bg-gradient-to-r from-skyblue-400 to-skyblue-500">Menyegarkan</span>
            </h1>
            <p class="text-xl md:text-2xl text-slate-600 mb-12 max-w-2xl mx-auto leading-relaxed">
                Saya merancang interface yang clean, modern, dan memberikan pengalaman user yang luar biasa.
            </p>
            <div class="flex flex-col sm:flex-row gap-6 justify-center items-center">
                <a href="#works" class="group bg-gradient-to-r from-skyblue-500 to-skyblue-600 hover:from-skyblue-600 hover:to-skyblue-700 px-12 py-4 rounded-2xl font-semibold text-lg text-white shadow-2xl hover:shadow-skyblue-500/25 transform hover:-translate-y-1 transition-all duration-500 flex items-center gap-3">
                    <i class="fas fa-arrow-right"></i>
                    <span>Lihat Karya Saya</span>
                </a>
                <a href="#contact" class="px-12 py-4 border-2 border-skyblue-200 hover:border-skyblue-400 rounded-2xl font-semibold text-lg hover:text-skyblue-600 transition-all duration-300 backdrop-blur-sm bg-white/80 hover:bg-white">
                    <i class="fas fa-paper-plane mr-2"></i>Hubungi Saya
                </a>
            </div>
        </div>
        <!-- Floating Elements -->
        <div class="absolute top-1/2 right-10 w-72 h-72 bg-gradient-to-r from-skyblue-200/30 to-skyblue-300/30 rounded-full blur-3xl animate-pulse"></div>
        <div class="absolute bottom-20 left-10 w-96 h-96 bg-gradient-to-r from-skyblue-300/20 to-skyblue-400/20 rounded-full blur-3xl animate-pulse delay-1000"></div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-32 px-6 bg-white/50">
        <div class="max-w-7xl mx-auto">
            <div class="text-center mb-24">
                <h2 class="text-5xl md:text-6xl font-bold bg-gradient-to-r from-slate-900 to-skyblue-600 bg-clip-text text-transparent mb-6">
                    Tentang Saya
                </h2>
                <div class="w-24 h-1 bg-gradient-to-r from-skyblue-400 to-skyblue-500 mx-auto rounded-full"></div>
            </div>
            
            <div class="grid md:grid-cols-2 gap-16 items-center">
                <div class="relative">
                    <div class="w-96 h-96 bg-gradient-to-br from-skyblue-100 to-skyblue-200 rounded-3xl backdrop-blur-xl border border-skyblue-300/50 p-8 animate-float">
                        <div class="w-full h-full bg-white rounded-2xl p-6 flex items-center justify-center shadow-2xl">
                            <i class="fas fa-user text-8xl text-skyblue-500"></i>
                        </div>
                    </div>
                </div>
                <div class="space-y-8">
                    <h3 class="text-4xl font-bold text-slate-900 mb-6">Creative Designer</h3>
                    <p class="text-xl text-slate-600 leading-relaxed">
                        Dengan pengalaman 5+ tahun di UI/UX Design, saya menciptakan produk digital yang tidak hanya 
                        indah secara visual tapi juga memberikan pengalaman user yang optimal.
                    </p>
                    <div class="grid md:grid-cols-2 gap-6 pt-8 border-t border-skyblue-200">
                        <div>
                            <div class="text-3xl font-bold text-skyblue-600 mb-2">50+</div>
                            <div class="text-slate-600">Projects Completed</div>
                        </div>
                        <div>
                            <div class="text-3xl font-bold text-skyblue-500 mb-2">25+</div>
                            <div class="text-slate-600">Happy Clients</div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Works Section -->
    <section id="works" class="py-32 px-6 bg-gradient-to-b from-skyblue-50 to-white">
        <div class="max-w-7xl mx-auto">
            <div class="text-center mb-24">
                <h2 class="text-5xl md:text-6xl font-bold bg-gradient-to-r from-slate-900 to-skyblue-600 bg-clip-text text-transparent mb-6">
                    Portfolio Terbaik
                </h2>
                <div class="w-24 h-1 bg-gradient-to-r from-skyblue-400 to-skyblue-500 mx-auto rounded-full"></div>
            </div>
            
            <!-- Filter Buttons -->
            <div class="flex flex-wrap justify-center gap-4 mb-16">
                <button class="filter-btn active px-8 py-3 bg-gradient-to-r from-skyblue-500 to-skyblue-600 text-white rounded-xl font-semibold shadow-lg hover:shadow-skyblue-500/25 transition-all duration-300">All</button>
                <button class="filter-btn px-8 py-3 bg-white hover:bg-skyblue-50 border border-skyblue-200 hover:border-skyblue-400 rounded-xl font-semibold shadow-sm hover:shadow-md transition-all duration-300 text-slate-700 hover:text-skyblue-600">Web Design</button>
                <button class="filter-btn px-8 py-3 bg-white hover:bg-skyblue-50 border border-skyblue-200 hover:border-skyblue-400 rounded-xl font-semibold shadow-sm hover:shadow-md transition-all duration-300 text-slate-700 hover:text-skyblue-600">Mobile App</button>
                <button class="filter-btn px-8 py-3 bg-white hover:bg-skyblue-50 border border-skyblue-200 hover:border-skyblue-400 rounded-xl font-semibold shadow-sm hover:shadow-md transition-all duration-300 text-slate-700 hover:text-skyblue-600">Branding</button>
            </div>

            <!-- Works Grid -->
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Project Card 1 -->
                <a href="#" class="group relative overflow-hidden rounded-3xl bg-white hover:bg-gradient-to-br hover:from-skyblue-500/5 border border-skyblue-200 hover:border-skyblue-400 shadow-lg hover:shadow-2xl transition-all duration-500 hover:scale-105 hover:-translate-y-2">
                    <div class="h-64 bg-gradient-to-br from-skyblue-200/50 to-skyblue-300/30 group-hover:blur-sm transition-all duration-500"></div>
                    <div class="absolute inset-0 bg-gradient-to-t from-slate-900/20 to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-500 backdrop-blur-sm"></div>
                    <div class="absolute bottom-6 left-6 right-6">
                        <h3 class="text-2xl font-bold text-slate-900 mb-2 group-hover:translate-x-2 transition-transform duration-300">E-Commerce App</h3>
                        <p class="text-slate-600 text-lg mb-4 group-hover:translate-x-2 transition-transform duration-300">Redesign aplikasi belanja modern</p>
                        <div class="flex gap-4 opacity-0 group-hover:opacity-100 transition-all duration-500 delay-200">
                            <div class="w-3 h-3 bg-skyblue-500 rounded-full animate-pulse"></div>
                            <div class="w-3 h-3 bg-skyblue-400 rounded-full animate-pulse" style="animation-delay: 0.2s"></div>
                            <div class="w-3 h-3 bg-skyblue-500 rounded-full animate-pulse" style="animation-delay: 0.4s"></div>
                        </div>
                    </div>
                </a>

                <!-- Project Card 2 -->
                <a href="#" class="group relative overflow-hidden rounded-3xl bg-white hover:bg-gradient-to-br hover:from-skyblue-500/5 border border-skyblue-200 hover:border-skyblue-400 shadow-lg hover:shadow-2xl transition-all duration-500 hover:scale-105 hover:-translate-y-2">
                    <div class="h-64 bg-gradient-to-br from-skyblue-300/50 to-skyblue-400/30 group-hover:blur-sm transition-all duration-500"></div>
                    <div class="absolute inset-0 bg-gradient-to-t from-slate-900/20 to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-500 backdrop-blur-sm"></div>
                    <div class="absolute bottom-6 left-6 right-6">
                        <h3 class="text-2xl font-bold text-slate-900 mb-2 group-hover:translate-x-2 transition-transform duration-300">Fintech Dashboard</h3>
                        <p class="text-slate-600 text-lg mb-4 group-hover:translate-x-2 transition-transform duration-300">Dashboard keuangan yang clean & modern</p>
                        <div class="flex gap-4 opacity-0 group-hover:opacity-100 transition-all duration-500 delay-200">
                            <div class="w-3 h-3 bg-skyblue-500 rounded-full animate-pulse"></div>
                            <div class="w-3 h-3 bg-skyblue-400 rounded-full animate-pulse" style="animation-delay: 0.2s"></div>
                            <div class="w-3 h-3 bg-skyblue-500 rounded-full animate-pulse" style="animation-delay: 0.4s"></div>
                        </div>
                    </div>
                </a>

                <!-- Project Card 3 -->
                <a href="#" class="group relative overflow-hidden rounded-3xl bg-white hover:bg-gradient-to-br hover:from-skyblue-500/5 border border-skyblue-200 hover:border-skyblue-400 shadow-lg hover:shadow-2xl transition-all duration-500 hover:scale-105 hover:-translate-y-2">
                    <div class="h-64 bg-gradient-to-br from-skyblue-200/50 to-skyblue-100/50 group-hover:blur-sm transition-all duration-500"></div>
                    <div class="absolute inset-0 bg-gradient-to-t from-slate-900/20 to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-500 backdrop-blur-sm"></div>
                    <div class="absolute bottom-6 left-6 right-6">
                        <h3 class="text-2xl font-bold text-slate-900 mb-2 group-hover:translate-x-2 transition-transform duration-300">Social Media App</h3>
                        <p class="text-slate-600 text-lg mb-4 group-hover:translate-x-2 transition-transform duration-300">Aplikasi sosial media generasi baru</p>
                        <div class="flex gap-4 opacity-0 group-hover:opacity-100 transition-all duration-500 delay-200">
                            <div class="w-3 h-3 bg-skyblue-500 rounded-full animate-pulse"></div>
                            <div class="w-3 h-3 bg-skyblue-400 rounded-full animate-pulse" style="animation-delay: 0.2s"></div>
                            <div class="w-3 h-3 bg-skyblue-500 rounded-full animate-pulse" style="animation-delay: 0.4s"></div>
                        </div>
                    </div>
                </a>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-32 px-6 bg-gradient-to-b from-white to-skyblue-50">
        <div class="max-w-4xl mx-auto text-center">
            <h2 class="text-5xl md:text-6xl font-bold bg-gradient-to-r from-slate-900 to-skyblue-600 bg-clip-text text-transparent mb-6">
                Mari Berkolaborasi
            </h2>
            <p class="text-xl text-slate-600 mb-16 max-w-2xl mx-auto">
                Punya project menarik? Saya siap membantu mewujudkannya menjadi digital product yang luar biasa.
            </p>
            
            <div class="grid md:grid-cols-2 gap-12">
                <div class="space-y-6">
                    <div class="text-4xl font-bold text-skyblue-600 mb-4">📧 Kontak</div>
                    <div class="space-y-4">
                        <div class="flex items-center gap-4 p-6 bg-white/70 backdrop-blur-sm rounded-2xl hover:bg-white shadow-lg hover:shadow-xl border border-skyblue-200 hover:border-skyblue-300 transition-all duration-300">
                            <i class="fas fa-envelope text-2xl text-skyblue-500"></i>
                            <div>
                                <div class="font-semibold text-slate-900">Email</div>
                                <a href="mailto:hello@yourname.com" class="text-skyblue-600 hover:text-skyblue-700 font-semibold transition-colors">hello@yourname.com</a>
                            </div>
                        </div>
                        <div class="flex items-center gap-4 p-6 bg-white/70 backdrop-blur-sm rounded-2xl hover:bg-white shadow-lg hover:shadow-xl border border-skyblue-200 hover:border-skyblue-300 transition-all duration-300">
                            <i class="fas fa-phone text-2xl text-skyblue-500"></i>
                            <div>
                                <div class="font-semibold text-slate-900">Phone</div>
                                <a href="tel:+628123456789" class="text-skyblue-600 hover:text-skyblue-700 font-semibold transition-colors">+62 812 3456 7890</a>
                            </div>
                        </div>
                    </div>
                </div>
                
                <form class="space-y-6 max-w-lg mx-auto">
                    <input type="text" placeholder="Nama Lengkap" class="w-full p-5 bg-white/70 backdrop-blur-sm border border-skyblue-200 hover:border-skyblue-400 rounded-2xl text-slate-900 placeholder-slate-500 shadow-lg focus:outline-none focus:border-skyblue-500 focus:shadow-skyblue-200 focus:shadow-xl transition-all duration-
