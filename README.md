<!DOCTYPE html>
<html lang="ug" dir="ltr" class="dark">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GitHub Profile Showcase - Freedom</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            darkMode: 'class',
            theme: {
                extend: {
                    colors: {
                        ghBg: '#0d1117',
                        ghCard: '#161b22',
                        ghBorder: '#30363d',
                        flagBlue: '#00a3e0', // Sky/East Turkestan Blue
                        neonCyan: '#00f2fe',
                        neonBlue: '#00d2ff'
                    },
                    boxShadow: {
                        'neon-blue': '0 0 25px rgba(0, 163, 224, 0.6), 0 0 50px rgba(0, 242, 254, 0.3)',
                        'glow-crescent': '0 0 35px rgba(0, 210, 255, 0.9)',
                    }
                }
            }
        }
    </script>
    <!-- FontAwesome for icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800;900&family=JetBrains+Mono:wght@400;600;700&display=swap" rel="stylesheet">
    
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #0d1117;
            color: #c9d1d9;
            overflow-x: hidden;
        }
        .code-font {
            font-family: 'JetBrains Mono', monospace;
        }
        
        /* Neon Glow Text Effects */
        .glow-text-freedom {
            text-shadow: 0 0 15px rgba(0, 163, 224, 0.9), 0 0 30px rgba(0, 242, 254, 0.7), 0 0 50px rgba(0, 163, 224, 0.5);
        }
        
        .hero-card-bg {
            background: linear-gradient(135deg, rgba(9, 21, 37, 0.95) 0%, rgba(4, 15, 28, 0.98) 100%);
            border: 1px solid rgba(0, 163, 224, 0.45);
        }
        
        /* Animated Background Grid */
        .grid-bg {
            background-image: 
                linear-gradient(to right, rgba(0, 163, 224, 0.1) 1px, transparent 1px),
                linear-gradient(to bottom, rgba(0, 163, 224, 0.1) 1px, transparent 1px);
            background-size: 30px 30px;
            animation: gridMove 20s linear infinite;
        }

        @keyframes gridMove {
            0% { background-position: 0 0; }
            100% { background-position: 30px 30px; }
        }

        /* Continuous Animations */
        @keyframes floatSlow {
            0%, 100% { transform: translateY(0px) rotate(0deg); }
            50% { transform: translateY(-14px) rotate(3deg); }
        }

        @keyframes pulseGlow {
            0%, 100% { filter: drop-shadow(0 0 18px rgba(0, 210, 255, 0.85)) drop-shadow(0 0 40px rgba(0, 163, 224, 0.6)); }
            50% { filter: drop-shadow(0 0 30px rgba(0, 242, 254, 1)) drop-shadow(0 0 60px rgba(0, 163, 224, 0.9)); }
        }

        @keyframes starRotate {
            0% { transform: rotate(0deg) scale(1); }
            50% { transform: rotate(180deg) scale(1.08); }
            100% { transform: rotate(360deg) scale(1); }
        }

        @keyframes rayShimmer {
            0%, 100% { opacity: 0.3; transform: scale(0.95); }
            50% { opacity: 0.8; transform: scale(1.08); }
        }

        .animate-float {
            animation: floatSlow 5s ease-in-out infinite;
        }

        .animate-crescent-glow {
            animation: pulseGlow 3s ease-in-out infinite;
        }

        .animate-star-spin {
            transform-origin: center;
            animation: starRotate 25s linear infinite;
        }

        .animate-shimmer {
            animation: rayShimmer 4s ease-in-out infinite;
        }
    </style>
</head>
<body class="min-h-screen bg-ghBg text-slate-200">

    <!-- Top GitHub Navbar Navigation -->
    <header class="border-b border-ghBorder bg-[#161b22]/90 backdrop-blur sticky top-0 z-50 px-4 py-3">
        <div class="max-w-7xl mx-auto flex items-center justify-between">
            <div class="flex items-center gap-4">
                <i class="fa-brands fa-github text-3xl text-white hover:text-cyan-400 transition cursor-pointer"></i>
                <div class="relative hidden sm:block">
                    <input type="text" placeholder="Type / to search" 
                        class="bg-[#0d1117] border border-ghBorder rounded-md px-3 py-1.5 text-sm w-64 focus:outline-none focus:border-cyan-500 text-slate-300">
                    <span class="absolute right-2 top-1.5 text-xs text-slate-500 border border-ghBorder px-1.5 rounded">/</span>
                </div>
            </div>
            <div class="flex items-center gap-3">
                <button class="bg-[#21262d] hover:bg-[#30363d] border border-ghBorder px-3 py-1.5 rounded-md text-xs font-semibold flex items-center gap-1.5">
                    <i class="fa-solid fa-plus"></i> <i class="fa-solid fa-caret-down text-slate-400"></i>
                </button>
                <div class="w-8 h-8 rounded-full border border-cyan-500/50 shadow-neon-blue overflow-hidden cursor-pointer">
                    <img src="https://placehold.co/100x100/0d1117/00a3e0?text=F" alt="User Avatar" class="w-full h-full object-cover">
                </div>
            </div>
        </div>
    </header>

    <!-- Main Container -->
    <main class="max-w-7xl mx-auto px-4 py-6">
        
        <!-- Profile Navigation Tabs -->
        <div class="border-b border-ghBorder mb-6 overflow-x-auto">
            <div class="flex gap-6 min-w-max">
                <a href="#" class="border-b-2 border-flagBlue text-white font-semibold py-2 px-1 flex items-center gap-2 text-sm">
                    <i class="fa-regular fa-bookmark text-slate-400"></i> Overview
                </a>
                <a href="#" class="text-slate-400 hover:text-white py-2 px-1 flex items-center gap-2 text-sm transition">
                    <i class="fa-solid fa-book-bookmark"></i> Repositories <span class="bg-ghBorder text-xs rounded-full px-2 py-0.5">24</span>
                </a>
                <a href="#" class="text-slate-400 hover:text-white py-2 px-1 flex items-center gap-2 text-sm transition">
                    <i class="fa-solid fa-table-cells"></i> Projects
                </a>
                <a href="#" class="text-slate-400 hover:text-white py-2 px-1 flex items-center gap-2 text-sm transition">
                    <i class="fa-solid fa-box"></i> Packages
                </a>
                <a href="#" class="text-slate-400 hover:text-white py-2 px-1 flex items-center gap-2 text-sm transition">
                    <i class="fa-regular fa-star"></i> Stars <span class="bg-ghBorder text-xs rounded-full px-2 py-0.5">142</span>
                </a>
            </div>
        </div>

        <!-- Grid Layout: Left Sidebar + Right Content -->
        <div class="grid grid-cols-1 lg:grid-cols-12 gap-8">
            
            <!-- Left Profile Sidebar -->
            <div class="lg:col-span-3 flex flex-col items-center lg:items-start">
                
                <!-- Profile Avatar with Blue Glow Ring -->
                <div class="relative group mb-4">
                    <div class="absolute -inset-1 bg-gradient-to-r from-flagBlue to-cyan-400 rounded-full blur opacity-75 group-hover:opacity-100 transition duration-500 animate-pulse"></div>
                    <div class="relative w-48 h-48 lg:w-64 lg:h-64 rounded-full overflow-hidden border-2 border-cyan-400 shadow-neon-blue bg-ghBg">
                        <!-- Avatar Content with Crescent Icon -->
                        <div class="w-full h-full bg-gradient-to-b from-[#061826] to-[#020b12] flex flex-col items-center justify-center relative">
                            <!-- SVG Blue Mini Crescent Star Avatar -->
                            <svg class="w-20 h-20 text-flagBlue drop-shadow-[0_0_12px_rgba(0,163,224,0.9)] mb-1" viewBox="0 0 100 100" fill="currentColor">
                                <path d="M50 10 A40 40 0 1 0 90 50 A32 32 0 1 1 50 10 Z"/>
                                <polygon points="68,32 73,44 85,44 76,52 79,64 68,56 57,64 60,52 51,44 63,44"/>
                            </svg>
                            <span class="text-2xl font-black text-white tracking-widest glow-text-freedom code-font">FREEDOM</span>
                            <span class="text-xs text-cyan-400/90 code-font mt-1">// DEVELOPER</span>
                        </div>
                    </div>
                </div>

                <!-- User Profile Info -->
                <h1 class="text-2xl font-bold text-white mb-0.5">Freedom Developer</h1>
                <h2 class="text-slate-400 font-mono text-sm mb-4">freedom-dev</h2>

                <button class="w-full bg-[#21262d] hover:bg-[#30363d] text-white border border-ghBorder font-medium py-1.5 px-4 rounded-md text-sm mb-4 transition shadow-sm hover:border-flagBlue">
                    Follow
                </button>

                <div class="flex items-center gap-4 text-xs text-slate-400 mb-6">
                    <span class="hover:text-cyan-400 cursor-pointer"><strong class="text-white">420</strong> followers</span>
                    <span>•</span>
                    <span class="hover:text-cyan-400 cursor-pointer"><strong class="text-white">95</strong> following</span>
                </div>

                <div class="w-full border-t border-ghBorder pt-4 space-y-2 text-sm text-slate-300">
                    <div class="flex items-center gap-2">
                        <i class="fa-solid fa-location-dot text-slate-500 w-4"></i>
                        <span>East Turkestan / Global</span>
                    </div>
                    <div class="flex items-center gap-2">
                        <i class="fa-regular fa-envelope text-slate-500 w-4"></i>
                        <a href="mailto:freedom@example.com" class="hover:underline hover:text-cyan-400">freedom@dev.org</a>
                    </div>
                    <div class="flex items-center gap-2">
                        <i class="fa-solid fa-link text-slate-500 w-4"></i>
                        <a href="#" class="hover:underline hover:text-cyan-400">freedom-project.dev</a>
                    </div>
                </div>
            </div>

            <!-- Right Main Profile README Showcase -->
            <div class="lg:col-span-9 space-y-6">
                
                <!-- GitHub README Container -->
                <div class="bg-ghCard border border-ghBorder rounded-lg p-4 sm:p-6 shadow-xl relative overflow-hidden">
                    
                    <!-- README Header Indicator -->
                    <div class="flex items-center justify-between border-b border-ghBorder pb-3 mb-6 text-xs text-slate-400 code-font">
                        <div class="flex items-center gap-2">
                            <i class="fa-regular fa-file-lines text-cyan-400"></i>
                            <span>freedom-dev / <strong class="text-slate-200">README.md</strong></span>
                        </div>
                        <i class="fa-solid fa-pencil hover:text-white cursor-pointer"></i>
                    </div>

                    <!-- HERO BANNER CARD (FREEDOM + ANIMATED BLUE CRESCENT STAR) -->
                    <div class="hero-card-bg grid-bg rounded-xl p-6 sm:p-10 relative overflow-hidden shadow-neon-blue border border-flagBlue/50 mb-8">
                        
                        <!-- Background Glow Lights -->
                        <div class="absolute -right-10 -top-10 w-72 h-72 bg-flagBlue/20 rounded-full blur-3xl pointer-events-none animate-shimmer"></div>
                        <div class="absolute left-1/3 bottom-0 w-48 h-48 bg-cyan-500/10 rounded-full blur-2xl pointer-events-none"></div>

                        <div class="grid grid-cols-1 md:grid-cols-12 gap-6 items-center relative z-10">
                            
                            <!-- Left Content -->
                            <div class="md:col-span-7">
                                <!-- Top Status Tag -->
                                <div class="inline-flex items-center gap-2 bg-flagBlue/20 border border-flagBlue/50 rounded-full px-3.5 py-1 text-xs text-cyan-300 mb-6 backdrop-blur">
                                    <span class="w-2.5 h-2.5 rounded-full bg-cyan-400 animate-ping"></span>
                                    <span class="font-semibold tracking-wide">AVAILABLE FOR COLLABORATION</span>
                                </div>

                                <div class="flex items-center gap-2 text-cyan-400 font-semibold text-sm mb-2 code-font">
                                    <i class="fa-solid fa-bolt"></i> HELLO WORLD, IT IS
                                </div>

                                <!-- MAIN FREEDOM TITLE -->
                                <h1 class="text-5xl sm:text-7xl font-black text-white tracking-wider mb-4 leading-none">
                                    <span class="text-transparent bg-clip-text bg-gradient-to-r from-cyan-300 via-flagBlue to-cyan-400 glow-text-freedom">
                                        FREEDOM
                                    </span>
                                </h1>

                                <p class="text-slate-300 text-sm sm:text-base max-w-xl leading-relaxed mb-6">
                                    Building open, decentralized, and elegant software experiences. Empowering innovation through clean code and modern technology.
                                </p>
                                
                                <!-- Badges / Tags -->
                                <div class="flex flex-wrap gap-2 text-xs code-font font-medium">
                                    <span class="bg-[#091b29] text-cyan-400 border border-flagBlue/40 px-3 py-1.5 rounded-md flex items-center gap-1.5 shadow-sm">
                                        &lt;CleanCode /&gt;
                                    </span>
                                    <span class="bg-[#091b29] text-cyan-300 border border-flagBlue/30 px-3 py-1.5 rounded-md">
                                        Modern Web
                                    </span>
                                    <span class="bg-[#091b29] text-blue-300 border border-blue-500/30 px-3 py-1.5 rounded-md">
                                        Open Source
                                    </span>
                                </div>
                            </div>

                            <!-- Right Side: ANIMATED BLUE UYGHUR CRESCENT & STAR (كۆك رەڭلىك ئاي يۇلتۇز) -->
                            <div class="md:col-span-5 flex justify-center md:justify-end items-center mt-6 md:mt-0">
                                <div class="relative w-56 h-56 sm:w-64 sm:h-64 flex items-center justify-center animate-float">
                                    
                                    <!-- Rotating Outer Decorative Radar Ring -->
                                    <svg class="absolute inset-0 w-full h-full text-flagBlue/30 animate-star-spin" viewBox="0 0 200 200">
                                        <circle cx="100" cy="100" r="90" fill="none" stroke="currentColor" stroke-width="1.5" stroke-dasharray="6, 10"/>
                                        <circle cx="100" cy="100" r="75" fill="none" stroke="currentColor" stroke-width="1" stroke-dasharray="2, 6"/>
                                    </svg>

                                    <!-- Glowing Blue Crescent & Star Vector Element -->
                                    <div class="relative z-10 w-44 h-44 sm:w-52 sm:h-52 animate-crescent-glow">
                                        <svg class="w-full h-full text-flagBlue fill-current filter" viewBox="0 0 100 100">
                                            <defs>
                                                <!-- Gradient for Crescent Star -->
                                                <linearGradient id="blueGlowGrad" x1="0%" y1="0%" x2="100%" y2="100%">
                                                    <stop offset="0%" stop-color="#00f2fe" />
                                                    <stop offset="50%" stop-color="#00a3e0" />
                                                    <stop offset="100%" stop-color="#0066ff" />
                                                </linearGradient>
                                            </defs>
                                            
                                            <!-- Crescent Moon (ئاي) -->
                                            <path fill="url(#blueGlowGrad)" d="M 48 10 A 38 38 0 1 0 86 48 A 30 30 0 1 1 48 10 Z" />
                                            
                                            <!-- 5-Pointed Star (يۇلتۇز) -->
                                            <g transform="translate(67, 33) scale(0.38)">
                                                <polygon fill="url(#blueGlowGrad)" points="25,1 32,16 49,18 37,30 40,47 25,39 9,47 13,30 1,18 17,16" />
                                            </g>
                                        </svg>
                                    </div>

                                </div>
                            </div>

                        </div>

                        <!-- Status Bar Footer -->
                        <div class="mt-8 pt-4 border-t border-flagBlue/30 flex items-center justify-between text-xs code-font text-cyan-300">
                            <div class="flex items-center gap-2">
                                <span class="inline-block w-3 h-1 bg-cyan-400 rounded-full animate-pulse"></span>
                                <span>SYS.STATUS // ONLINE & CREATING</span>
                            </div>
                            <span class="text-slate-400">EAST TURKESTAN // 2026</span>
                        </div>
                    </div>

                    <!-- Shields / Live Badges Section -->
                    <div class="flex flex-wrap items-center justify-start gap-3 mb-8 text-xs font-bold code-font">
                        <!-- Profile Views Shield -->
                        <div class="flex rounded-md overflow-hidden border border-ghBorder shadow">
                            <span class="bg-slate-800 text-slate-300 px-3 py-1.5 border-r border-ghBorder">PROFILE VIEWS</span>
                            <span class="bg-flagBlue text-black px-3 py-1.5 font-extrabold">3,890</span>
                        </div>
                        
                        <!-- Followers Shield -->
                        <div class="flex rounded-md overflow-hidden border border-ghBorder shadow">
                            <span class="bg-slate-800 text-slate-300 px-3 py-1.5 border-r border-ghBorder flex items-center gap-1">
                                <i class="fa-brands fa-github"></i> FOLLOWERS
                            </span>
                            <span class="bg-blue-600 text-white px-3 py-1.5">420</span>
                        </div>

                        <!-- Status Shield -->
                        <div class="flex rounded-md overflow-hidden border border-ghBorder shadow">
                            <span class="bg-slate-800 text-slate-300 px-3 py-1.5 border-r border-ghBorder">STATUS</span>
                            <span class="bg-emerald-500 text-black px-3 py-1.5 font-bold">ACTIVELY CODING</span>
                        </div>
                    </div>

                    <!-- About Me Section -->
                    <div class="mb-8">
                        <h3 class="text-xl font-bold text-white mb-4 flex items-center gap-2 border-b border-ghBorder pb-2">
                            <span>👤</span> About Freedom
                        </h3>
                        <ul class="space-y-3 text-slate-300 text-sm leading-relaxed">
                            <li class="flex items-start gap-2">
                                <span class="text-cyan-400 mt-1">🌙</span>
                                <span>Developing modern digital products with a focus on freedom, decentralization, and privacy.</span>
                            </li>
                            <li class="flex items-start gap-2">
                                <span class="text-cyan-400 mt-1">🚀</span>
                                <span>Building scalable web applications, UI/UX designs, and cloud infrastructure.</span>
                            </li>
                            <li class="flex items-start gap-2">
                                <span class="text-cyan-400 mt-1">🌱</span>
                                <span>Continuous learner in AI models, Web3 technologies, and interactive visual designs.</span>
                            </li>
                            <li class="flex items-start gap-2">
                                <span class="text-cyan-400 mt-1">💬</span>
                                <span>Let's collaborate on high-impact open-source projects!</span>
                            </li>
                        </ul>
                    </div>

                    <!-- Tech Stack / Skills Badges -->
                    <div class="mb-8">
                        <h3 class="text-xl font-bold text-white mb-4 flex items-center gap-2 border-b border-ghBorder pb-2">
                            <span>⚡</span> Tech Stack & Tools
                        </h3>
                        <div class="flex flex-wrap gap-2">
                            <span class="bg-[#1c2128] border border-ghBorder hover:border-flagBlue text-cyan-300 px-3 py-1.5 rounded-md text-xs code-font font-medium flex items-center gap-2 transition">
                                <i class="fa-brands fa-react text-cyan-400 text-sm"></i> React.js
                            </span>
                            <span class="bg-[#1c2128] border border-ghBorder hover:border-blue-400 text-blue-300 px-3 py-1.5 rounded-md text-xs code-font font-medium flex items-center gap-2 transition">
                                <i class="fa-brands fa-js text-yellow-400 text-sm"></i> JavaScript / TS
                            </span>
                            <span class="bg-[#1c2128] border border-ghBorder hover:border-teal-400 text-teal-300 px-3 py-1.5 rounded-md text-xs code-font font-medium flex items-center gap-2 transition">
                                <i class="fa-solid fa-wind text-teal-400 text-sm"></i> Tailwind CSS
                            </span>
                            <span class="bg-[#1c2128] border border-ghBorder hover:border-green-400 text-green-300 px-3 py-1.5 rounded-md text-xs code-font font-medium flex items-center gap-2 transition">
                                <i class="fa-brands fa-node-js text-green-400 text-sm"></i> Node.js
                            </span>
                            <span class="bg-[#1c2128] border border-ghBorder hover:border-orange-400 text-orange-300 px-3 py-1.5 rounded-md text-xs code-font font-medium flex items-center gap-2 transition">
                                <i class="fa-brands fa-git-alt text-orange-400 text-sm"></i> Git & GitHub
                            </span>
                        </div>
                    </div>

                    <!-- Activity / Stats Cards Grid -->
                    <div>
                        <h3 class="text-xl font-bold text-white mb-4 flex items-center gap-2 border-b border-ghBorder pb-2">
                            <span>📊</span> GitHub Statistics
                        </h3>
                        <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                            <!-- Stat Card 1 -->
                            <div class="bg-[#161b22] border border-ghBorder hover:border-flagBlue rounded-lg p-4 transition shadow-md">
                                <div class="flex justify-between items-center mb-3">
                                    <span class="text-sm font-semibold text-slate-300">Freedom's Stats</span>
                                    <i class="fa-solid fa-chart-simple text-cyan-400"></i>
                                </div>
                                <div class="space-y-2 text-xs code-font">
                                    <div class="flex justify-between">
                                        <span class="text-slate-400">Total Stars Earned:</span>
                                        <span class="text-cyan-400 font-bold">480</span>
                                    </div>
                                    <div class="flex justify-between">
                                        <span class="text-slate-400">Total Commits (2026):</span>
                                        <span class="text-cyan-400 font-bold">1,850+</span>
                                    </div>
                                    <div class="flex justify-between">
                                        <span class="text-slate-400">Total PRs:</span>
                                        <span class="text-cyan-400 font-bold">142</span>
                                    </div>
                                </div>
                            </div>

                            <!-- Stat Card 2 -->
                            <div class="bg-[#161b22] border border-ghBorder hover:border-flagBlue rounded-lg p-4 transition shadow-md">
                                <div class="flex justify-between items-center mb-3">
                                    <span class="text-sm font-semibold text-slate-300">Top Languages</span>
                                    <i class="fa-solid fa-code text-blue-400"></i>
                                </div>
                                <div class="space-y-2 text-xs code-font">
                                    <div>
                                        <div class="flex justify-between mb-1">
                                            <span class="text-slate-400">TypeScript / JS</span>
                                            <span class="text-slate-300">75%</span>
                                        </div>
                                        <div class="w-full h-1.5 bg-slate-800 rounded-full overflow-hidden">
                                            <div class="w-[75%] h-full bg-cyan-400 shadow-neon-blue"></div>
                                        </div>
                                    </div>
                                    <div>
                                        <div class="flex justify-between mb-1">
                                            <span class="text-slate-400">HTML / CSS</span>
                                            <span class="text-slate-300">20%</span>
                                        </div>
                                        <div class="w-full h-1.5 bg-slate-800 rounded-full overflow-hidden">
                                            <div class="w-[20%] h-full bg-flagBlue"></div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>

                </div>
            </div>

        </div>
    </main>

    <!-- Footer -->
    <footer class="border-t border-ghBorder mt-12 py-6 text-center text-xs text-slate-500">
        <p>© 2026 Freedom GitHub Profile Showcase. Modern Cyan-Blue Glow Aesthetic.</p>
    </footer>

</body>
</html>
