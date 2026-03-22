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
                            50: '#f0f9ff', 100: '#e0f2fe', 200: '#bae6fd', 300: '#7dd3fc',
                            400: '#38bdf8', 500: '#0ea5e9', 600: '#0284c7', 700: '#0369a1',
                            800: '#075985', 900: '#0c4a6e', 950: '#082f49'
                        }
                    },
                    animation: {
                        'float': 'float 6s ease-in-out infinite',
                        'fadeInUp': 'fadeInUp 1s ease-out',
                    }
                }
            }
        }
    </script>
    <style>
        @keyframes float {
            0%, 100% { transform: translate3d(0,0,0); }
            50% { transform: translate3d(0,-10px,0); }
        }
        @keyframes fadeInUp {
            0% { opacity: 0; transform: translateY(30px); }
            100% { opacity: 1; transform: translateY(0); }
        }
        .filter-btn.active { 
            background: linear-gradient(to right, #0ea5e9, #0284c7) !important; 
            color: white !important; 
        }
    </style>
</head>
<body class="bg-gradient-to-br from-skyblue-50 via-white to-skyblue-100 text-slate-900 overflow-x-hidden">

    <!-- Mobile Navigation -->
    <nav class="fixed top-0 w-full z-50 bg-white/95 backdrop-blur-md border-b border-skyblue-200/50 shadow-sm md:relative md:bg-transparent">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-4">
            <div class="flex justify-between items-center">
                <a href="#" class="text-xl sm:text-2xl font-bold bg-gradient-to-r from-skyblue-500 to-skyblue-600 bg-clip-text text-transparent">
                    [Nama Anda]
                </a>
                
                <!-- Desktop Menu -->
                <div class="hidden md:flex space-x-8">
                    <a href="#home" class="hover:text-skyblue-500 font-medium transition-all duration-300 py-2">Home</a>
                    <a href="#about" class="hover:text-skyblue-500 font-medium transition-all duration-300 py-2">About</a>
                    <a href="#works" class="hover:text-skyblue-500 font-medium transition-all duration-300 py-2">Works</a>
                    <a href="#contact" class="hover:text-skyblue-500 font-medium transition-all duration-300 py-2">Contact</a>
                </div>
                
                <!-- Mobile Menu Button -->
                <button id="mobile-menu-btn" class="md:hidden text-skyblue-600 p-2">
                    <i class="fas fa-bars text-xl"></i>
                </button>
            </div>
        </div>
        
        <!-- Mobile Menu -->
        <div id="mobile-menu" class="md:hidden hidden bg-white/95 backdrop-blur-md border-t border-skyblue-200 shadow-lg">
            <div class="px-4 py-6 space-y-4">
                <a href="#home" class="block hover:text-skyblue-500 font-medium transition-all duration-300 py-2">Home</a>
                <a href="#about" class="block hover:text-skyblue-500 font-medium transition-all duration-300 py-2">About</a>
                <a href="#works" class="block hover:text-skyblue-500 font-medium transition-all duration-300 py-2">Works</a>
                <a href="#contact" class="block hover:text-skyblue-500 font-medium transition-all duration-300 py-2">Contact</a>
            </div>
        </div>
    </nav>

    <!-- Hero Section - Fully Responsive -->
    <section id="home" class="min-h-screen flex items-center justify-center pt-20 px-4 sm:px-6 lg:px-8 pb-20 lg:pb-0 overflow-hidden">
        <div class="w-full max-w-4xl mx-auto text-center animate-fadeInUp px-4">
            <div class="inline-block p-3 sm:p-4 bg-gradient-to-r from-skyblue-100 to-skyblue-200 rounded-2xl backdrop-blur-sm border border-skyblue-300/50 mb-6 sm:mb-8 animate-float max-w-max mx-auto">
                <span class="text-xs sm:text-sm bg-gradient-to-r from-skyblue-600 to-skyblue-700 bg-clip-text text-transparent font-semibold px-2">UI/UX Designer</span>
            </div>
            <h1 class="text-4xl sm:text-5xl md:text-6xl lg:text-7xl font-bold bg-gradient-to-r from-slate-900 via-skyblue-600 to-skyblue-700 bg-clip-text text-transparent mb-4 sm:mb-6 leading-tight">
                Membuat <span class="bg-gradient-to-r from-skyblue-500 to-skyblue-600">Pengalaman</span><br class="hidden sm:block">
                Digital yang <span class="bg-gradient-to-r from-skyblue-400 to-skyblue-500">Menyegarkan</span>
            </h1>
            <p class="text-lg sm:text-xl md:text-2xl text-slate-600 mb-8 sm:mb-12 max-w-2xl mx-auto leading-relaxed px-2">
                Saya merancang interface yang clean, modern, dan memberikan pengalaman user yang luar biasa.
            </p>
            <div class="flex flex-col xs:flex-row gap-4 sm:gap-6 justify-center items-center px-2">
                <a href="#works" class="group w-full xs:w-auto bg-gradient-to-r from-skyblue-500 to-skyblue-600 hover:from-skyblue-600 hover:to-skyblue-700 px-8 sm:px-12 py-4 rounded-2xl font-semibold text-lg text-white shadow-2xl hover:shadow-skyblue-500/25 transform hover:-translate-y-1 transition-all duration-500 flex items-center justify-center gap-3 min-h-[56px]">
                    <i class="fas fa-arrow-right text-sm"></i>
                    <span>Lihat Karya</span>
                </a>
                <a href="#contact" class="w-full xs:w-auto px-8 sm:px-12 py-4 border-2 border-skyblue-200 hover:border-skyblue-400 rounded-2xl font-semibold text-lg hover:text-skyblue-600 transition-all duration-300 backdrop-blur-sm bg-white/80 hover:bg-white shadow-lg min-h-[56px] flex items-center justify-center">
                    <i class="fas fa-paper-plane mr-2"></i>Hubungi
                </a>
            </div>
        </div>
        
        <!-- Responsive Floating Elements -->
        <div class="absolute top-1/4 lg:top-1/2 right-4 sm:right-10 w-32 sm:w-48 lg:w-72 h-32 sm:h-48 lg:h-72 bg-gradient-to-r from-skyblue-200/30 to-skyblue-300/30 rounded-full blur-xl sm:blur-2xl lg:blur-3xl animate-pulse hidden lg:block"></div>
        <div class="absolute bottom-10 sm:bottom-20 left-4 sm:left-10 w-40 sm:w-64 lg:w-96 h-40 sm:h-64 lg:h-96 bg-gradient-to-r from-skyblue-300/20 to-skyblue-400/20 rounded-full blur-xl sm:blur-2xl lg:blur-3xl animate-pulse delay-1000 hidden lg:block"></div>
    </section>

    <!-- About Section - Responsive -->
    <section id="about" class="py-20 sm:py-24 lg:py-32 px-4 sm:px-6 lg:px-8 bg-white/50">
        <div class="max-w-6xl mx-auto">
            <div class="text-center mb-16 sm:mb-20 lg:mb-24">
                <h2 class="text-3xl sm:text-4xl md:text-5xl lg:text-6xl font-bold bg-gradient-to-r from-slate-900 to-skyblue-600 bg-clip-text text-transparent mb-4 sm:mb-6 leading-tight">
                    Tentang Saya
                </h2>
                <div class="w-20 sm:w-24 h-1 bg-gradient-to-r from-skyblue-400 to-skyblue-500 mx-auto rounded-full"></div>
            </div>
            
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-12 lg:gap-16 items-center">
                <div class="relative mx-auto w-64 sm:w-80 lg:w-96 h-64 sm:h-80 lg:h-96">
                    <div class="absolute inset-0 w-full h-full bg-gradient-to-br from-skyblue-100 to-skyblue-200 rounded-3xl backdrop-blur-xl border border-skyblue-300/50 p-4 sm:p-6 lg:p-8 animate-float">
                        <div class="w-full h-full bg-white rounded-2xl p-4 sm:p-6 flex items-center justify-center shadow-2xl border border-skyblue-100">
                            <i class="fas fa-user text-4xl sm:text-6xl lg:text-8xl text-skyblue-500"></i>
                        </div>
                    </div>
                </div>
                <div class="space-y-6 lg:space-y-8 text-left lg:text-left">
                    <h3 class="text-2xl sm:text-3xl lg:text-4xl font-bold text-slate-900 mb-4 sm:mb-6">Creative Designer</h3>
                    <p class="text-lg sm:text-xl text-slate-600 leading-relaxed">
                        Dengan pengalaman 5+ tahun di UI/UX Design, saya menciptakan produk digital yang tidak hanya 
                        indah secara visual tapi juga memberikan pengalaman user yang optimal.
                    </p>
                    <div class="grid grid-cols-2 gap-6 pt-6 sm:pt-8 border-t border-skyblue-200">
                        <div>
                            <div class="text-2xl sm:text-3xl lg:text-3xl font-bold text-skyblue-600 mb-1 sm:mb-2">50+</div>
                            <div class="text-slate-600 text-sm sm:text-base">Projects</div>
                        </div>
                        <div>
                            <div class="text-2xl sm:text-3xl lg:text-3xl font-bold text-skyblue-500 mb-1 sm:mb-2">25+</div>
                            <div class="text-slate-600 text-sm sm:text-base">Clients</div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Works Section - Perfect Responsive Grid -->
    <section id="works" class="py-20 sm:py-24 lg:py-32 px-4 sm:px-6 lg:px-8 bg-gradient-to-b from-skyblue-50 to-white">
        <div class="max-w-7xl mx-auto">
            <div class="text-center mb-16 sm:mb-20 lg:mb-24">
                <h2 class="text-3xl sm:text-4xl md:text-5xl lg:text-6xl font-bold bg-gradient-to-r from-slate-900 to-skyblue-600 bg-clip-text text-transparent mb-4 sm:mb-6 leading-tight">
                    Portfolio Terbaik
                </h2>
                <div class="w-20 sm:w-24 h-1 bg-gradient-to-r from-skyblue-400 to-skyblue-500 mx-auto rounded-full"></div>
            </div>
            
            <!-- Responsive Filter Buttons -->
            <div class="flex flex-wrap justify-center gap-2 sm:gap-4 mb-12 sm:mb-16 px-2">
                <button class="filter-btn active px-6 sm:px-8 py-3 bg-gradient-to-r from-skyblue-500 to-skyblue-600 text-white text-sm sm:text-base rounded-xl font-semibold shadow-lg hover:shadow-skyblue-500/25 transition-all duration-300 min-w-[100px]">All</button>
                <button class="filter-btn px-6 sm:px-8 py-3 bg-white hover:bg-skyblue-50 border border-skyblue-200 hover:border-skyblue-400 rounded-xl font-semibold shadow-sm hover:shadow-md transition-all duration-300 text-sm sm:text-base text-slate-700 hover:text-skyblue-600 min-w-[120px]">Web</button>
                <button class="filter-btn px-6 sm:px-8 py-3 bg-white hover:bg-skyblue-50 border border-skyblue-200 hover:border-skyblue-400 rounded-xl font-semibold shadow-sm hover:shadow-md transition-all duration-300 text-sm sm:text-base text-slate-700 hover:text-skyblue-600 min-w-[120px]">Mobile</button>
                <button class="filter-btn px-6 sm:px-8 py-3 bg-white hover:bg-skyblue-50 border border-skyblue-200 hover:border-skyblue-400 rounded-xl font-semibold shadow-sm hover:shadow-md transition-all duration-300 text-sm sm:text-base text-slate-700 hover:text-skyblue-600 min-w-[120px]">Branding</button>
            </div>

            <!-- Responsive Works Grid -->
            <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6 sm:gap-8 px-2">
                <!-- Project Card 1 -->
                <a href="#" class="group relative overflow-hidden rounded-3xl bg-white hover:bg-gradient-to-br hover:from-skyblue-500/5 border border-skyblue-200 hover:border-skyblue-400 shadow-lg hover:shadow-2xl transition-all duration-500 hover:scale-[1.02] sm:hover:scale-105 hover:-translate-y-2 block w-full">
                    <div class="h-48 sm:h-56 lg:h-64 bg-gradient-to-br from-skyblue-200/50 to-skyblue-300/30 group-hover:blur-sm transition-all duration-500"></div>
                    <div class="absolute inset-0 bg-gradient-to-t from-slate-900/20 to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-500 backdrop-blur-sm"></div>
                    <div class="absolute bottom-4 sm:bottom-6 left-4 sm:left-6 right-4 sm:right-6">
                        <h3 class="text-xl sm:text-2xl font-bold text-slate-900 mb-1 sm:mb-2 group-hover:translate-x-2 transition-transform duration-300 leading-tight">E-Commerce App</h3>
                        <p class="text-slate-600 text-sm sm:text-lg mb-3 sm:mb-4 group-hover:translate-x-2 transition-transform duration-300 leading-relaxed">Redesign aplikasi belanja</p>
                        <div class="flex gap-2 opacity-0 group-hover:opacity-100 transition-all duration-500 delay-200">
                            <div class="w-2 h-2 sm:w-3 sm:h-3 bg-skyblue-500 rounded-full animate-pulse"></div>
                            <div class="w-2 h-2 sm:w-3 sm:h-3 bg-skyblue-400 rounded-full animate-pulse" style="animation-delay: 0.2s"></div>
                            <div class="w-2 h-2 sm:w-3 sm:h-3 bg-skyblue-500 rounded-full animate-pulse" style="animation-delay: 0.4s"></div>
                        </div>
                    </div>
                </a>

                <!-- Project Card 2 -->
                <a href="#" class="group relative overflow-hidden rounded-3xl bg-white hover:bg-gradient-to-br hover:from-skyblue-500/5 border border-skyblue-200 hover:border-skyblue-400 shadow-lg hover:shadow-2xl transition-all duration-500 hover:scale-[1.02] sm:hover:scale-105 hover:-translate-y-2 block w-full">
                    <div class="h-48 sm:h-56 lg:h-64 bg-gradient-to-br from-skyblue-300/50 to-skyblue-400/30 group-hover:blur-sm transition-all duration-500"></div>
                    <div class="absolute inset-0 bg-gradient-to-t from-slate-900/20 to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-500 backdrop-blur-sm"></div>
                    <div class="absolute bottom-4 sm:bottom-6 left-4 sm:left-6 right-4 sm:right-6">
                        <h3 class="text-xl sm:text-2xl font-bold text-slate-900 mb-1 sm:mb-2 group-hover:translate-x-2 transition-transform duration-300 leading-tight">Fintech Dashboard</h3>
                        <p class="text-slate-600 text-sm sm:text-lg mb-3 sm:mb-4 group-hover:translate-x-2 transition-transform duration-300 leading-relaxed">Dashboard keuangan modern</p>
                        <div class="flex gap-2 opacity-0 group-hover:opacity-100 transition-all duration-500 delay-200">
                            <div class="w-2 h-2 sm:w-3 sm:h-3 bg-skyblue-500 rounded-full animate-pulse"></div>
                            <div class="w-2 h-2 sm:w-3 sm:h-3 bg-skyblue-400 rounded-full animate-pulse" style="animation-delay: 0.2s"></div>
                            <div class="w-2 h-2 sm:w-3 sm:h-3 bg-skyblue-500 rounded-full animate-pulse" style="animation-delay: 0.4s"></div>
                        </div>
                    </div>
                </a>

                <!-- Project Card 3 -->
                <a href="#" class="group relative overflow-hidden rounded-3xl bg-white hover:bg-gradient-to-br hover:from-skyblue-500/5 border border-skyblue-200 hover:border-skyblue-400 shadow-lg hover:shadow-2xl transition-all duration-500 hover:scale
