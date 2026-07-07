# innovation-kitchen-and-bath
<!doctype html>
<html lang="en" class="scroll-smooth">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Innovation Redesign | Dark Stone & Gold Luxury Preview</title>
    <!-- Premium Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=Playfair+Display:ital,wght@0,400;0,600;0,700;1,400&family=Space+Grotesk:wght@400;500;600;700&display=swap" rel="stylesheet">
    
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
      tailwind.config = {
        theme: {
          extend: {
            fontFamily: {
              sans: ['Inter', 'sans-serif'],
              display: ['Space Grotesk', 'sans-serif'],
              serif: ['Playfair Display', 'serif'],
            },
            colors: {
              gold: {
                50: '#fcfbf6',
                100: '#f9f0da',
                200: '#f1dfbc',
                300: '#e6cb95',
                400: '#dbb367',
                500: '#c59b27',
                600: '#aa811e',
                700: '#8d6718',
                800: '#715013',
                900: '#583d0f',
                950: '#322106',
              },
              navy: {
                50: '#f4f6f9',
                100: '#e9ecf3',
                200: '#cbd5e7',
                350: '#6786bf',
                500: '#4265a7',
                800: '#1b284c',
                900: '#0a1128',
                950: '#050814',
              },
              obsidian: {
                50: '#f8f8f8',
                100: '#e0e0e0',
                800: '#1c1c1e',
                900: '#121214',
                950: '#070708'
              }
            }
          }
        }
      }
    </script>
    
    <style>
      /* Smooth Premium Scroll Animations CSS */
      .reveal {
        opacity: 0;
        transform: translateY(30px);
        transition: all 1s cubic-bezier(0.16, 1, 0.3, 1);
        will-change: transform, opacity;
      }
      .reveal.active {
        opacity: 1;
        transform: translateY(0);
      }
      
      .reveal-left {
        opacity: 0;
        transform: translateX(-40px);
        transition: all 1s cubic-bezier(0.16, 1, 0.3, 1);
        will-change: transform, opacity;
      }
      .reveal-left.active {
        opacity: 1;
        transform: translateX(0);
      }

      .reveal-right {
        opacity: 0;
        transform: translateX(40px);
        transition: all 1s cubic-bezier(0.16, 1, 0.3, 1);
        will-change: transform, opacity;
      }
      .reveal-right.active {
        opacity: 1;
        transform: translateX(0);
      }

      /* Hover Glow and Luxury Shimmers */
      .gold-shimmer {
        background: linear-gradient(
          120deg,
          transparent 0%,
          transparent 40%,
          rgba(219, 179, 103, 0.3) 50%,
          transparent 60%,
          transparent 100%
        );
        background-size: 200% 100%;
      }
      .gold-shimmer:hover {
        animation: shimmerEffect 1.5s ease-out infinite;
      }
      @keyframes shimmerEffect {
        0% { background-position: 100% 0; }
        100% { background-position: -100% 0; }
      }

      .glow-on-hover {
        transition: all 0.4s ease;
      }
      .glow-on-hover:hover {
        box-shadow: 0 0 25px rgba(197, 155, 39, 0.15);
        border-color: rgba(197, 155, 39, 0.4);
      }
    </style>
  </head>
  
  <body class="bg-obsidian-950 text-stone-300 font-sans min-h-screen selection:bg-gold-500/20 selection:text-gold-200 antialiased overflow-x-hidden">

    <!-- 1. TOP INFORMATION RIBBON -->
    <div class="bg-obsidian-950 text-stone-400 py-2 px-4 text-xs font-medium border-b border-obsidian-900 z-50 relative">
      <div class="max-w-7xl mx-auto flex flex-col md:flex-row justify-between items-center gap-2">
        <div class="flex items-center gap-4 text-[11px] tracking-wide">
          <span class="flex items-center gap-1"><span class="text-gold-400">✦</span> Serving Central Florida Since 2011</span>
          <span class="hidden md:inline text-stone-600">|</span>
          <span class="hidden md:flex items-center gap-1">In-House Laser templating & Slabs Shop</span>
        </div>
        <div class="flex items-center gap-5 text-[11px] font-mono tracking-wider">
          <a href="tel:4079892802" class="text-stone-300 hover:text-gold-400 transition-colors flex items-center gap-1">
            (407) 989-2802
          </a>
          <span class="text-gold-500 bg-gold-950 border border-gold-800/40 px-2 py-0.5 rounded text-[10px] font-bold uppercase tracking-widest">
            CNC WATERJET PRECISION
          </span>
        </div>
      </div>
    </div>

    <!-- 2. BRAND NAVIGATION HEADER -->
    <header class="bg-obsidian-900/85 backdrop-blur-md sticky top-0 z-40 border-b border-obsidian-800/50">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 py-4 flex items-center justify-between">
        <!-- Logo -->
        <a href="#" class="flex items-center gap-2 group">
          <div class="border border-gold-600/60 p-2 rounded flex items-center justify-center transition-all group-hover:border-gold-400">
            <span class="font-serif font-bold text-lg text-gold-400 tracking-wider">I</span>
          </div>
          <div class="flex flex-col">
            <span class="font-serif font-bold text-white tracking-widest text-sm leading-none">INNOVATION</span>
            <span class="font-serif text-[10px] text-gold-500 tracking-[0.35em] font-semibold leading-none mt-1">KITCHEN & BATH</span>
          </div>
        </a>
        
        <!-- Desktop Nav -->
        <nav class="hidden lg:flex items-center gap-1 text-[11px] uppercase tracking-wider font-semibold font-display text-stone-400">
          <a href="#hero" class="px-3.5 py-2 hover:text-white hover:bg-obsidian-800 rounded transition-all">Portal</a>
          <a href="#about" class="px-3.5 py-2 hover:text-white hover:bg-obsidian-800 rounded transition-all">About</a>
          <a href="#showroom" class="px-3.5 py-2 hover:text-white hover:bg-obsidian-800 rounded transition-all">Material Showroom</a>
          <a href="#services" class="px-3.5 py-2 hover:text-white hover:bg-obsidian-800 rounded transition-all">Services</a>
          <a href="#testimonials" class="px-3.5 py-2 hover:text-white hover:bg-obsidian-800 rounded transition-all">Praise</a>
          <a href="#quote" class="px-3.5 py-2 hover:text-white hover:bg-obsidian-800 rounded transition-all text-gold-400">Cost Planner</a>
        </nav>

        <!-- CTAs -->
        <div class="flex items-center gap-3">
          <a href="tel:4079892802" class="hidden sm:inline-flex items-center gap-1.5 px-3 py-1.5 rounded bg-obsidian-800 border border-obsidian-700/60 text-xs font-semibold hover:bg-obsidian-700 text-stone-200 transition-all">
            Call Consultant
          </a>
          <a href="#quote" class="bg-gradient-to-r from-gold-600 to-gold-500 hover:from-gold-500 hover:to-gold-400 text-obsidian-950 font-bold text-xs py-2 px-4 rounded shadow-lg transition-all tracking-wide uppercase">
            Request Quote
          </a>
        </div>
      </div>
    </header>

    <!-- 3. DUAL-PORTAL HERO SECTION (IMAGE 3) -->
    <section id="hero" class="relative min-h-[85vh] flex items-center justify-center overflow-hidden py-16 px-4 bg-obsidian-950 border-b border-obsidian-900">
      <!-- Background images with smooth cross-fade -->
      <div class="absolute inset-0 z-0">
        <!-- Residential BG -->
        <img id="hero-bg-residential" src="images/ogc_hero_kitchen_1782306639623.jpg" alt="Luxury Residential Spaces" class="w-full h-full object-cover transition-all duration-1000 scale-105 opacity-30 absolute inset-0 z-10" />
        <!-- Commercial BG -->
        <img id="hero-bg-commercial" src="images/ogc_commercial_lobby_1782306668882.jpg" alt="Commercial Stone Projects" class="w-full h-full object-cover transition-all duration-1000 scale-105 opacity-0 absolute inset-0 z-10" />
        
        <!-- Luxury Gradient Layers -->
        <div class="absolute inset-0 bg-gradient-to-t from-obsidian-950 via-obsidian-950/80 to-transparent z-20" />
        <div class="absolute inset-0 bg-gradient-to-r from-obsidian-950 via-obsidian-950/50 to-transparent z-20" />
      </div>

      <!-- Hero Main Content -->
      <div class="max-w-7xl mx-auto w-full relative z-30 flex flex-col items-center text-center">
        <!-- Dual Portal Switcher -->
        <div class="inline-flex bg-obsidian-900/90 p-1 rounded border border-gold-600/30 backdrop-blur-md mb-8 reveal">
          <button id="btn-portal-residential" onclick="togglePortal('residential')" class="px-5 py-2 rounded text-xs font-bold transition-all duration-500 tracking-wider uppercase bg-gold-500 text-obsidian-950">
            Residential Renovations
          </button>
          <button id="btn-portal-commercial" onclick="togglePortal('commercial')" class="px-5 py-2 rounded text-xs font-bold transition-all duration-500 tracking-wider uppercase text-stone-400 hover:text-white">
            Commercial Slabs
          </button>
        </div>

        <!-- Dynamic Brand Heading -->
        <div class="max-w-3xl mb-8">
          <span id="hero-subtitle" class="text-xs font-bold text-gold-400 tracking-[0.3em] uppercase block mb-3 font-mono reveal">
            CENTRAL FLORIDA PRESTIGE LIVING
          </span>
          <h1 id="hero-title" class="font-serif text-4xl sm:text-5xl md:text-6xl text-white font-medium tracking-tight leading-tight mb-6 reveal">
            Crafting High-End Custom <br/>Residential Spaces
          </h1>
          <p id="hero-desc" class="text-stone-400 text-sm sm:text-base md:text-lg font-light leading-relaxed max-w-xl mx-auto reveal">
            Specializing in luxury kitchen, bath, and cabinetry fabrication using premium granite, engineered quartz, and Spanish porcelain slabs since 2011.
          </p>
        </div>

        <!-- Interactive CTAs -->
        <div class="flex flex-col sm:flex-row gap-4 justify-center items-center reveal">
          <a href="#showroom" class="bg-gradient-to-r from-gold-600 to-gold-500 hover:from-gold-500 hover:to-gold-400 text-obsidian-950 font-bold text-xs py-4 px-8 rounded shadow-lg transition-all tracking-wider uppercase font-display">
            Explore Slabs Showroom
          </a>
          <a href="#quote" class="bg-obsidian-900/80 hover:bg-obsidian-800 text-stone-200 hover:text-white font-semibold text-xs py-4 px-8 rounded border border-gold-600/40 backdrop-blur-sm transition-all tracking-wider uppercase font-display">
            Interactive Cost Planner
          </a>
        </div>
      </div>
    </section>

    <!-- 4. ABOUT THE STORY (IMAGE 3 - PLEDGE SECTION) -->
    <section id="about" class="py-24 px-4 bg-obsidian-900/40 border-b border-obsidian-900">
      <div class="max-w-7xl mx-auto grid grid-cols-1 lg:grid-cols-12 gap-12 items-center">
        <!-- Content Column (7 cols) -->
        <div class="lg:col-span-7 flex flex-col gap-6 reveal-left">
          <div>
            <span class="text-xs font-bold text-gold-500 uppercase tracking-widest font-mono">
              THE ART OF STONE FABRICATION
            </span>
            <h2 class="font-serif text-3xl sm:text-4xl md:text-5xl text-white font-semibold tracking-tight mt-2 leading-tight">
              Orlando's Premier Custom <br/>
              <span class="text-gold-400 italic">Kitchen & Bath Legacy</span>
            </h2>
          </div>
          
          <div class="text-sm text-stone-400 space-y-4 leading-relaxed font-light">
            <p>
              Since 2011, we have operated with a steadfast dedication to high-end stone cutting, cabinet fabrication, and architectural alignment. Our master fabricators combine traditional craftsmanship with advanced robotic technologies.
            </p>
            <p>
              While other contractors move to outsourced, modular setups, we execute <strong class="text-stone-200">100% of our precision templating and heavy CNC waterjet cutting inside our local Orlando shop</strong>. This meticulous in-house handling guarantees sub-millimeter seam accuracy for continuous-vein matched slabs.
            </p>
            <p>
              Every custom island, commercial lobby desk, or luxury vanity is measured, hand-polished, and set in place by our certified local experts. We take pride in absolute accountability.
            </p>
          </div>

          <!-- Quick Stats -->
          <div class="grid grid-cols-3 gap-6 pt-6 border-t border-obsidian-800 mt-2">
            <div>
              <span class="font-display font-bold text-2xl sm:text-3xl text-gold-400 block">15+</span>
              <span class="text-[10px] text-stone-500 uppercase tracking-wider block font-mono mt-1">Years experience</span>
            </div>
            <div>
              <span class="font-display font-bold text-2xl sm:text-3xl text-white block">100%</span>
              <span class="text-[10px] text-stone-500 uppercase tracking-wider block font-mono mt-1">In-House Shop</span>
            </div>
            <div>
              <span class="font-display font-bold text-2xl sm:text-3xl text-white block">0.5mm</span>
              <span class="text-[10px] text-stone-500 uppercase tracking-wider block font-mono mt-1">Laser Accuracy</span>
            </div>
          </div>
        </div>

        <!-- Founders' Pledge Block (5 cols - Image 3 design) -->
        <div class="lg:col-span-5 reveal-right">
          <div class="bg-obsidian-900 border border-gold-600/20 rounded-2xl p-8 relative overflow-hidden shadow-2xl glow-on-hover gold-shimmer">
            <!-- Subtle vector background motif -->
            <div class="absolute -top-10 -right-10 text-gold-500/5 select-none pointer-events-none">
              <span class="font-serif text-[12rem] font-bold">“</span>
            </div>

            <div class="relative z-10 flex flex-col gap-6">
              <div class="flex items-center gap-1 text-gold-400">
                <span class="text-xs font-bold font-mono uppercase tracking-widest text-gold-500">THE IKB PERFORMANCE GUARANTEE</span>
              </div>

              <p class="font-serif text-stone-200 italic leading-relaxed text-sm md:text-base font-light">
                "Our reputation is forged on every slab we measure, polish, and fit. We do not ask for final payment until you inspect the seams under direct light and agree they are absolutely flawless. That is our luxury standard since 2011."
              </p>

              <div class="border-t border-obsidian-800/80 pt-5 flex items-center gap-4">
                <div class="w-10 h-10 rounded-full bg-gold-500 text-obsidian-950 font-bold flex items-center justify-center text-xs shadow-md">
                  IKB
                </div>
                <div>
                  <h4 class="text-xs font-bold text-white tracking-wide uppercase">IKB Design Directors</h4>
                  <p class="text-[10px] text-stone-500 font-mono mt-0.5">Master Stone Engineers & Fabricators</p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- 6. SLABS SHOWROOM CATALOG (IMAGE 2) -->
    <section id="showroom" class="py-24 px-4 bg-obsidian-900/10 border-b border-obsidian-900">
      <div class="max-w-7xl mx-auto">
        
        <!-- Header Section -->
        <div class="text-center mb-16 reveal">
          <span class="text-xs font-bold text-gold-400 tracking-[0.25em] uppercase block mb-2 font-mono">
            IN-HOUSE MATERIAL COLLECTION
          </span>
          <h2 class="font-serif text-3xl sm:text-4xl text-white font-medium tracking-tight">
            Orlando Slabs Showroom
          </h2>
          <p class="text-stone-400 text-xs sm:text-sm font-light mt-3 max-w-xl mx-auto">
            Discover our hand-picked collection of exotic natural granites, quartzites, engineered solid quartz, and Spanish porcelain claddings.
          </p>
        </div>

        <!-- Filter Controls Drawer (Image 2 style) -->
        <div class="bg-obsidian-900 border border-gold-600/20 rounded-2xl p-6 mb-12 flex flex-col md:flex-row justify-between items-stretch md:items-center gap-6 shadow-xl reveal">
          
          <!-- Category Filters -->
          <div class="flex flex-col gap-2">
            <span class="text-[9px] font-bold text-stone-500 uppercase tracking-widest font-mono">Stone Type</span>
            <div class="flex flex-wrap gap-2">
              <button onclick="filterSlabs('all')" class="slab-filter-btn px-4 py-1.5 rounded-full text-xs font-bold tracking-wide border border-gold-500 bg-gold-500 text-obsidian-950 transition-all">All</button>
              <button onclick="filterSlabs('granite')" class="slab-filter-btn px-4 py-1.5 rounded-full text-xs font-bold tracking-wide border border-obsidian-800 text-stone-400 hover:text-white hover:border-stone-700 transition-all">Granite</button>
              <button onclick="filterSlabs('quartz')" class="slab-filter-btn px-4 py-1.5 rounded-full text-xs font-bold tracking-wide border border-obsidian-800 text-stone-400 hover:text-white hover:border-stone-700 transition-all">Quartz</button>
              <button onclick="filterSlabs('porcelain')" class="slab-filter-btn px-4 py-1.5 rounded-full text-xs font-bold tracking-wide border border-obsidian-800 text-stone-400 hover:text-white hover:border-stone-700 transition-all">Porcelain</button>
              <button onclick="filterSlabs('quartzite')" class="slab-filter-btn px-4 py-1.5 rounded-full text-xs font-bold tracking-wide border border-obsidian-800 text-stone-400 hover:text-white hover:border-stone-700 transition-all">Quartzite</button>
            </div>
          </div>

          <!-- Quality Filters -->
          <div class="flex flex-col gap-2">
            <span class="text-[9px] font-bold text-stone-500 uppercase tracking-widest font-mono">Quality Tier</span>
            <div class="flex flex-wrap gap-2">
              <button class="px-4 py-1.5 rounded-full text-xs font-bold border border-gold-500 bg-gold-500 text-obsidian-950">All</button>
              <button class="px-4 py-1.5 rounded-full text-xs font-semibold border border-obsidian-800 text-stone-400 hover:text-white transition-all">Premium</button>
              <button class="px-4 py-1.5 rounded-full text-xs font-semibold border border-obsidian-800 text-stone-400 hover:text-white transition-all">Luxury Edition</button>
            </div>
          </div>

        </div>

        <!-- Slabs Product Grid (Mirroring Image 2 Cards) -->
        <div id="slabs-grid" class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-8">
          
          <!-- Card 1 -->
          <div class="slab-card group bg-obsidian-900 border border-obsidian-800 rounded-2xl overflow-hidden shadow-xl hover:border-gold-600/30 transition-all duration-300 flex flex-col justify-between" data-category="granite">
            <div class="relative overflow-hidden aspect-[16/10] bg-obsidian-950">
              <img src="images/ogc_hero_kitchen_1782306639623.jpg" alt="Absolute Black Granite" class="w-full h-full object-cover grayscale opacity-60 group-hover:opacity-85 group-hover:scale-105 group-hover:grayscale-0 transition-all duration-700" />
              <!-- Customize tooltip reveal -->
              <div class="absolute inset-0 bg-obsidian-950/80 flex flex-col justify-center items-center gap-3 p-4 opacity-0 group-hover:opacity-100 transition-all duration-300">
                <p class="text-xs text-stone-400 text-center font-light">Exquisite micro-crystalline dark matrix. Resists continuous heat & weathering.</p>
                <button onclick="selectSlabToCostPlanner('Absolute Black Granite', '65')" class="bg-gradient-to-r from-gold-600 to-gold-500 text-obsidian-950 text-[10px] font-bold uppercase tracking-wider px-4 py-2 rounded shadow-md">
                  Estimate Cost
                </button>
              </div>
            </div>
            <div class="p-6 border-t border-obsidian-800 flex justify-between items-center bg-obsidian-900/50">
              <div>
                <h3 class="text-white font-medium text-sm font-display tracking-wide group-hover:text-gold-400 transition-colors">Absolute Black Granite</h3>
                <p class="text-[10px] text-stone-500 font-mono uppercase mt-1">Origin: India • Standard</p>
              </div>
              <span class="text-xs font-mono font-bold text-gold-500">$$</span>
            </div>
          </div>

          <!-- Card 2 -->
          <div class="slab-card group bg-obsidian-900 border border-obsidian-800 rounded-2xl overflow-hidden shadow-xl hover:border-gold-600/30 transition-all duration-300 flex flex-col justify-between" data-category="quartzite">
            <div class="relative overflow-hidden aspect-[16/10] bg-obsidian-950">
              <img src="images/ogc_hero_kitchen_1782306639623.jpg" alt="Panda White Marble" class="w-full h-full object-cover opacity-60 group-hover:opacity-85 group-hover:scale-105 transition-all duration-700" />
              <!-- Customize tooltip reveal -->
              <div class="absolute inset-0 bg-obsidian-950/80 flex flex-col justify-center items-center gap-3 p-4 opacity-0 group-hover:opacity-100 transition-all duration-300">
                <p class="text-xs text-stone-400 text-center font-light">Striking dynamic charcoal ribbons. Polished signature luxury surface.</p>
                <button onclick="selectSlabToCostPlanner('Panda White Marble', '125')" class="bg-gradient-to-r from-gold-600 to-gold-500 text-obsidian-950 text-[10px] font-bold uppercase tracking-wider px-4 py-2 rounded shadow-md">
                  Estimate Cost
                </button>
              </div>
            </div>
            <div class="p-6 border-t border-obsidian-800 flex justify-between items-center bg-obsidian-900/50">
              <div>
                <h3 class="text-white font-medium text-sm font-display tracking-wide group-hover:text-gold-400 transition-colors">Panda White Marble</h3>
                <p class="text-[10px] text-stone-500 font-mono uppercase mt-1">Origin: China • Luxury Edition</p>
              </div>
              <span class="text-xs font-mono font-bold text-gold-500">$$$$</span>
            </div>
          </div>

          <!-- Card 3 -->
          <div class="slab-card group bg-obsidian-900 border border-obsidian-800 rounded-2xl overflow-hidden shadow-xl hover:border-gold-600/30 transition-all duration-300 flex flex-col justify-between" data-category="quartz">
            <div class="relative overflow-hidden aspect-[16/10] bg-obsidian-950">
              <img src="images/ogc_hero_kitchen_1782306639623.jpg" alt="Calacatta Gold Quartz" class="w-full h-full object-cover opacity-60 group-hover:opacity-85 group-hover:scale-105 transition-all duration-700" />
              <!-- Customize tooltip reveal -->
              <div class="absolute inset-0 bg-obsidian-950/80 flex flex-col justify-center items-center gap-3 p-4 opacity-0 group-hover:opacity-100 transition-all duration-300">
                <p class="text-xs text-stone-400 text-center font-light">Gilded veins cascade gracefully over white quartz matrix. Elite durability.</p>
                <button onclick="selectSlabToCostPlanner('Calacatta Gold Quartz', '85')" class="bg-gradient-to-r from-gold-600 to-gold-500 text-obsidian-950 text-[10px] font-bold uppercase tracking-wider px-4 py-2 rounded shadow-md">
                  Estimate Cost
                </button>
              </div>
            </div>
            <div class="p-6 border-t border-obsidian-800 flex justify-between items-center bg-obsidian-900/50">
              <div>
                <h3 class="text-white font-medium text-sm font-display tracking-wide group-hover:text-gold-400 transition-colors">Calacatta Gold Quartz</h3>
                <p class="text-[10px] text-stone-500 font-mono uppercase mt-1">Origin: Italy • Premium</p>
              </div>
              <span class="text-xs font-mono font-bold text-gold-500">$$$</span>
            </div>
          </div>

          <!-- Card 4 -->
          <div class="slab-card group bg-obsidian-900 border border-obsidian-800 rounded-2xl overflow-hidden shadow-xl hover:border-gold-600/30 transition-all duration-300 flex flex-col justify-between" data-category="quartzite">
            <div class="relative overflow-hidden aspect-[16/10] bg-obsidian-950">
              <img src="images/ogc_hero_kitchen_1782306639623.jpg" alt="Taj Mahal Quartzite" class="w-full h-full object-cover opacity-60 group-hover:opacity-85 group-hover:scale-105 transition-all duration-700" />
              <!-- Customize tooltip reveal -->
              <div class="absolute inset-0 bg-obsidian-950/80 flex flex-col justify-center items-center gap-3 p-4 opacity-0 group-hover:opacity-100 transition-all duration-300">
                <p class="text-xs text-stone-400 text-center font-light">Warm pearlescent crystalline stone. Highly resistant to scratches.</p>
                <button onclick="selectSlabToCostPlanner('Taj Mahal Quartzite', '125')" class="bg-gradient-to-r from-gold-600 to-gold-500 text-obsidian-950 text-[10px] font-bold uppercase tracking-wider px-4 py-2 rounded shadow-md">
                  Estimate Cost
                </button>
              </div>
            </div>
            <div class="p-6 border-t border-obsidian-800 flex justify-between items-center bg-obsidian-900/50">
              <div>
                <h3 class="text-white font-medium text-sm font-display tracking-wide group-hover:text-gold-400 transition-colors">Taj Mahal Quartzite</h3>
                <p class="text-[10px] text-stone-500 font-mono uppercase mt-1">Origin: Brazil • Luxury Edition</p>
              </div>
              <span class="text-xs font-mono font-bold text-gold-500">$$$$</span>
            </div>
          </div>

          <!-- Card 5 -->
          <div class="slab-card group bg-obsidian-900 border border-obsidian-800 rounded-2xl overflow-hidden shadow-xl hover:border-gold-600/30 transition-all duration-300 flex flex-col justify-between" data-category="porcelain">
            <div class="relative overflow-hidden aspect-[16/10] bg-obsidian-950">
              <img src="images/ogc_hero_kitchen_1782306639623.jpg" alt="Statuario Porcelain" class="w-full h-full object-cover opacity-60 group-hover:opacity-85 group-hover:scale-105 transition-all duration-700" />
              <!-- Customize tooltip reveal -->
              <div class="absolute inset-0 bg-obsidian-950/80 flex flex-col justify-center items-center gap-3 p-4 opacity-0 group-hover:opacity-100 transition-all duration-300">
                <p class="text-xs text-stone-400 text-center font-light">Sintered Spanish porcelain slab with continuous grey linear veining. Zero maintenance.</p>
                <button onclick="selectSlabToCostPlanner('Statuario Porcelain', '160')" class="bg-gradient-to-r from-gold-600 to-gold-500 text-obsidian-950 text-[10px] font-bold uppercase tracking-wider px-4 py-2 rounded shadow-md">
                  Estimate Cost
                </button>
              </div>
            </div>
            <div class="p-6 border-t border-obsidian-800 flex justify-between items-center bg-obsidian-900/50">
              <div>
                <h3 class="text-white font-medium text-sm font-display tracking-wide group-hover:text-gold-400 transition-colors">Statuario Porcelain</h3>
                <p class="text-[10px] text-stone-500 font-mono uppercase mt-1">Origin: Spain • Premium</p>
              </div>
              <span class="text-xs font-mono font-bold text-gold-500">$$$</span>
            </div>
          </div>

          <!-- Card 6 -->
          <div class="slab-card group bg-obsidian-900 border border-obsidian-800 rounded-2xl overflow-hidden shadow-xl hover:border-gold-600/30 transition-all duration-300 flex flex-col justify-between" data-category="granite">
            <div class="relative overflow-hidden aspect-[16/10] bg-obsidian-950">
              <img src="images/ogc_hero_kitchen_1782306639623.jpg" alt="Calacotta Black Granite" class="w-full h-full object-cover opacity-60 group-hover:opacity-85 group-hover:scale-105 transition-all duration-700" />
              <!-- Customize tooltip reveal -->
              <div class="absolute inset-0 bg-obsidian-950/80 flex flex-col justify-center items-center gap-3 p-4 opacity-0 group-hover:opacity-100 transition-all duration-300">
                <p class="text-xs text-stone-400 text-center font-light">Mesmerizing deep charcoal currents. Hand-finished edges. Stunning island centerpiece.</p>
                <button onclick="selectSlabToCostPlanner('Calacotta Black Granite', '65')" class="bg-gradient-to-r from-gold-600 to-gold-500 text-obsidian-950 text-[10px] font-bold uppercase tracking-wider px-4 py-2 rounded shadow-md">
                  Estimate Cost
                </button>
              </div>
            </div>
            <div class="p-6 border-t border-obsidian-800 flex justify-between items-center bg-obsidian-900/50">
              <div>
                <h3 class="text-white font-medium text-sm font-display tracking-wide group-hover:text-gold-400 transition-colors">Calacotta Black Granite</h3>
                <p class="text-[10px] text-stone-500 font-mono uppercase mt-1">Origin: India • Standard</p>
              </div>
              <span class="text-xs font-mono font-bold text-gold-500">$$</span>
            </div>
          </div>

        </div>

      </div>
    </section>

    <!-- 7. SERVICES GRID (IMAGE 3 ACCENTS) -->
    <section id="services" class="py-24 px-4 bg-obsidian-950 border-b border-obsidian-900">
      <div class="max-w-7xl mx-auto">
        <!-- Header -->
        <div class="text-center mb-16 reveal">
          <span class="text-xs font-bold text-gold-400 tracking-[0.25em] uppercase block mb-2 font-mono">
            BESPOKE SPACE SPECIALTIES
          </span>
          <h2 class="font-serif text-3xl sm:text-4xl text-white font-medium tracking-tight">
            Our Architectural Remodeling Services
          </h2>
          <p class="text-stone-400 text-xs sm:text-sm font-light mt-3 max-w-xl mx-auto">
            From precision laser measuring to heavy-duty slab installation, our in-house specialists raise the standards of excellence.
          </p>
        </div>

        <!-- Services Bento-style Grid -->
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
          
          <div class="bg-obsidian-900 border border-obsidian-800/80 p-8 rounded-2xl flex flex-col justify-between transition-all hover:border-gold-500/20 hover:-translate-y-1.5 duration-300 shadow-xl reveal-left">
            <div>
              <span class="text-gold-500 text-xl font-bold font-mono">01</span>
              <h3 class="text-white font-bold font-display text-base tracking-wide mt-3 mb-2">Kitchen Remodeling</h3>
              <p class="text-xs text-stone-400 leading-relaxed font-light">Complete luxury renovations. Custom-engineered islands, structural cabinet installations, full-slab claddings, and waterfall edge joins.</p>
            </div>
            <a href="#quote" class="inline-flex items-center gap-1 text-[11px] font-bold text-gold-400 uppercase tracking-widest mt-6 hover:text-white transition-colors">
              Request Layout Survey →
            </a>
          </div>

          <div class="bg-obsidian-900 border border-obsidian-800/80 p-8 rounded-2xl flex flex-col justify-between transition-all hover:border-gold-500/20 hover:-translate-y-1.5 duration-300 shadow-xl reveal">
            <div>
              <span class="text-gold-500 text-xl font-bold font-mono">02</span>
              <h3 class="text-white font-bold font-display text-base tracking-wide mt-3 mb-2">Bathroom Remodeling</h3>
              <p class="text-xs text-stone-400 leading-relaxed font-light">Spa-grade custom layouts. Integrated double quartz basins, large-format porcelain wall surfaces, and floor-to-ceiling bookmatched designs.</p>
            </div>
            <a href="#quote" class="inline-flex items-center gap-1 text-[11px] font-bold text-gold-400 uppercase tracking-widest mt-6 hover:text-white transition-colors">
              Request Layout Survey →
            </a>
          </div>

          <div class="bg-obsidian-900 border border-obsidian-800/80 p-8 rounded-2xl flex flex-col justify-between transition-all hover:border-gold-500/20 hover:-translate-y-1.5 duration-300 shadow-xl reveal-right">
            <div>
              <span class="text-gold-500 text-xl font-bold font-mono">03</span>
              <h3 class="text-white font-bold font-display text-base tracking-wide mt-3 mb-2">Custom Cabinetry</h3>
              <p class="text-xs text-stone-400 leading-relaxed font-light">Solid hardwood frames built inside our local Orlando woodworking shop. Superior durability, smooth soft-close hardware, and bespoke colors.</p>
            </div>
            <a href="#quote" class="inline-flex items-center gap-1 text-[11px] font-bold text-gold-400 uppercase tracking-widest mt-6 hover:text-white transition-colors">
              Request Layout Survey →
            </a>
          </div>

          <div class="bg-obsidian-900 border border-obsidian-800/80 p-8 rounded-2xl flex flex-col justify-between transition-all hover:border-gold-500/20 hover:-translate-y-1.5 duration-300 shadow-xl reveal-left">
            <div>
              <span class="text-gold-500 text-xl font-bold font-mono">04</span>
              <h3 class="text-white font-bold font-display text-base tracking-wide mt-3 mb-2">Granite & Quartz</h3>
              <p class="text-xs text-stone-400 leading-relaxed font-light">Precision measurement, cutting, edge molding, and seamless alignment of raw stone slabs and quartzite counters.</p>
            </div>
            <a href="#quote" class="inline-flex items-center gap-1 text-[11px] font-bold text-gold-400 uppercase tracking-widest mt-6 hover:text-white transition-colors">
              Request Layout Survey →
            </a>
          </div>

          <div class="bg-obsidian-900 border border-obsidian-800/80 p-8 rounded-2xl flex flex-col justify-between transition-all hover:border-gold-500/20 hover:-translate-y-1.5 duration-300 shadow-xl reveal">
            <div>
              <span class="text-gold-500 text-xl font-bold font-mono">05</span>
              <h3 class="text-white font-bold font-display text-base tracking-wide mt-3 mb-2">Commercial Projects</h3>
              <p class="text-xs text-stone-400 leading-relaxed font-light">Corporate office lobbies, high-traffic medical facility vanities, restaurant bar overlays, and illuminated stone accents.</p>
            </div>
            <a href="#quote" class="inline-flex items-center gap-1 text-[11px] font-bold text-gold-400 uppercase tracking-widest mt-6 hover:text-white transition-colors">
              Request Layout Survey →
            </a>
          </div>

          <div class="bg-obsidian-900 border border-obsidian-800/80 p-8 rounded-2xl flex flex-col justify-between transition-all hover:border-gold-500/20 hover:-translate-y-1.5 duration-300 shadow-xl reveal-right">
            <div>
              <span class="text-gold-500 text-xl font-bold font-mono">06</span>
              <h3 class="text-white font-bold font-display text-base tracking-wide mt-3 mb-2">Precision Tile Work</h3>
              <p class="text-xs text-stone-400 leading-relaxed font-light">Impeccable spacing and placement of complex glass mosaics, micro-tiles, and marble backsplashes. Flawless grout finishes.</p>
            </div>
            <a href="#quote" class="inline-flex items-center gap-1 text-[11px] font-bold text-gold-400 uppercase tracking-widest mt-6 hover:text-white transition-colors">
              Request Layout Survey →
            </a>
          </div>

        </div>

      </div>
    </section>

    <!-- 8. PREMIUM TESTIMONIALS & VIDEO SHOWCASE (IMAGE 4) -->
    <section id="testimonials" class="py-24 px-4 bg-obsidian-900 border-b border-obsidian-950">
      <div class="max-w-7xl mx-auto">
        
        <!-- Section Header -->
        <div class="text-center mb-16 reveal">
          <span class="text-xs font-bold text-gold-400 tracking-[0.25em] uppercase block mb-2 font-mono">
            IKB CLIENT PRAISE
          </span>
          <h2 class="font-serif text-3xl sm:text-4xl text-white font-medium tracking-tight">
            Customer Testimonials
          </h2>
          <p class="text-stone-400 text-xs sm:text-sm font-light mt-3 max-w-xl mx-auto">
            Experience our hand-polished finishes and bookmatch precision through the words of real Florida homeowners and commercial developers.
          </p>
        </div>

        <!-- Custom Grid layout mirroring Image 4 structure -->
        <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 items-stretch">
          
          <!-- Video Showcase card on the left (5 cols) -->
          <div class="lg:col-span-5 relative rounded-2xl overflow-hidden min-h-[300px] sm:min-h-[400px] border border-gold-600/20 shadow-2xl reveal-left">
            <img src="images/ogc_hero_kitchen_1782306639623.jpg" alt="Video Showcase Thumbnail" class="w-full h-full object-cover opacity-50 absolute inset-0 z-0" />
            <div class="absolute inset-0 bg-gradient-to-t from-obsidian-950/90 via-obsidian-950/40 to-transparent z-10" />
            
            <!-- Video Play Overlay -->
            <div class="relative z-20 flex flex-col justify-between items-center h-full p-8 text-center">
              <div class="bg-obsidian-950/80 px-4 py-2 rounded-full border border-gold-600/30 text-[10px] font-mono uppercase tracking-widest text-gold-400">
                Inside Our Orlando Slabs Shop
              </div>
              
              <!-- Custom Interactive Play Button -->
              <button onclick="playSimulationVideo()" class="w-20 h-20 bg-gradient-to-tr from-gold-600 to-gold-400 hover:from-gold-400 hover:to-gold-300 rounded-full flex items-center justify-center text-obsidian-950 font-bold uppercase tracking-wider text-xs shadow-2xl transition-all hover:scale-110">
                Play
              </button>
              
              <p class="text-xs font-medium text-stone-200 leading-normal max-w-xs">
                Watch our CNC waterjet machine slice Calacatta slabs with continuous vein alignment.
              </p>
            </div>
          </div>

          <!-- Testimonial Stacks on the right (7 cols) -->
          <div class="lg:col-span-7 flex flex-col gap-6 justify-between reveal-right">
            
            <!-- Review 1 -->
            <div class="bg-obsidian-950/60 border border-gold-600/10 rounded-xl p-6 sm:p-8 flex flex-col gap-4 shadow-xl hover:border-gold-500/20 transition-all">
              <div class="flex justify-between items-center">
                <div class="flex gap-1 text-gold-500">
                  <span>★</span><span>★</span><span>★</span><span>★</span><span>★</span>
                </div>
                <span class="text-[9px] text-stone-500 font-mono">WINDERMERE, FL</span>
              </div>
              <p class="text-xs text-stone-300 italic leading-relaxed">
                "Unparalleled craftsmanship and service. Our double islands feature waterfall edges that meet with absolute perfection. The team measuring and executing were professional and clean."
              </p>
              <div class="border-t border-obsidian-900/80 pt-3 flex justify-between items-center text-[10px] font-mono uppercase">
                <span class="text-white font-bold">- Sarah J., Luxury Homeowner</span>
                <span class="text-gold-500 font-sans tracking-widest font-bold text-[9px]">Kitchen Remodel</span>
              </div>
            </div>

            <!-- Review 2 -->
            <div class="bg-obsidian-950/60 border border-gold-600/10 rounded-xl p-6 sm:p-8 flex flex-col gap-4 shadow-xl hover:border-gold-500/20 transition-all">
              <div class="flex justify-between items-center">
                <div class="flex gap-1 text-gold-500">
                  <span>★</span><span>★</span><span>★</span><span>★</span><span>★</span>
                </div>
                <span class="text-[9px] text-stone-500 font-mono">LAKE NONA, FL</span>
              </div>
              <p class="text-xs text-stone-300 italic leading-relaxed">
                "Transformative work on our corporate reception desk. Bookmatched slab lines are seamless under architectural spotlights. Incredible accuracy under rigorous specs."
              </p>
              <div class="border-t border-obsidian-900/80 pt-3 flex justify-between items-center text-[10px] font-mono uppercase">
                <span class="text-white font-bold">- David L., Property Developer</span>
                <span class="text-gold-500 font-sans tracking-widest font-bold text-[9px]">Commercial Lobby</span>
              </div>
            </div>

            <!-- Review 3 -->
            <div class="bg-obsidian-950/60 border border-gold-600/10 rounded-xl p-6 sm:p-8 flex flex-col gap-4 shadow-xl hover:border-gold-500/20 transition-all">
              <div class="flex justify-between items-center">
                <div class="flex gap-1 text-gold-500">
                  <span>★</span><span>★</span><span>★</span><span>★</span><span>★</span>
                </div>
                <span class="text-[9px] text-stone-500 font-mono">WINTER PARK, FL</span>
              </div>
              <p class="text-xs text-stone-300 italic leading-relaxed">
                "Our premium quartzite vanity looks stunning. Elegant seamless borders. The hand polishing has a high gloss shine that looks beautiful every single day."
              </p>
              <div class="border-t border-obsidian-900/80 pt-3 flex justify-between items-center text-[10px] font-mono uppercase">
                <span class="text-white font-bold">- Sanya D., Estate Owner</span>
                <span class="text-gold-500 font-sans tracking-widest font-bold text-[9px]">Master Bathroom</span>
              </div>
            </div>

          </div>

        </div>

      </div>
    </section>

    <!-- 9. INTERACTIVE QUOTE SCHEDULER & PRICE ESTIMATOR (IMAGE 1 & 4 ACCENTS) -->
    <section id="quote" class="py-24 px-4 bg-obsidian-950 border-b border-obsidian-900">
      <div class="max-w-4xl mx-auto bg-obsidian-900 border border-gold-600/20 rounded-2xl p-8 sm:p-12 relative overflow-hidden shadow-2xl reveal">
        <div class="absolute -bottom-16 -left-16 w-48 h-48 bg-gold-500/5 rounded-full blur-3xl pointer-events-none"></div>
        <div class="absolute -top-16 -right-16 w-48 h-48 bg-gold-500/5 rounded-full blur-3xl pointer-events-none"></div>

        <div class="relative z-10">
          <span class="text-xs font-bold text-gold-500 uppercase tracking-widest block font-mono mb-2">PRECISION PRICING IN SECONDS</span>
          <h2 class="font-serif text-2xl sm:text-3xl text-white font-semibold tracking-tight">Interactive Price Estimate Calculator</h2>
          <p class="text-xs text-stone-400 mt-2 leading-relaxed">Adjust dimensions and select high-end stone options to view a realistic, in-house fabrication cost calculation instantly.</p>
          
          <form class="mt-8 grid grid-cols-1 md:grid-cols-2 gap-6" oninput="calculateEstimate()">
            <!-- Column 1 -->
            <div class="flex flex-col gap-4">
              <div class="flex flex-col gap-1.5">
                <label class="text-[10px] font-bold text-stone-400 uppercase tracking-wider font-mono">Countertop Linear Feet</label>
                <input id="calc-counter-feet" type="number" value="30" min="5" max="200" class="bg-obsidian-950 border border-obsidian-800 focus:border-gold-500 rounded px-4 py-3 text-xs text-white focus:outline-none transition-colors" />
              </div>
              <div class="flex flex-col gap-1.5">
                <label class="text-[10px] font-bold text-stone-400 uppercase tracking-wider font-mono">Material Class Selection</label>
                <select id="calc-material-class" class="bg-obsidian-950 border border-obsidian-800 focus:border-gold-500 rounded px-4 py-3 text-xs text-white focus:outline-none transition-colors">
                  <option value="65">Standard Slabs ($65/sqft)</option>
                  <option value="85" selected>Premium Engineered Quartz ($85/sqft)</option>
                  <option value="125">Luxury Exotic Quartzite ($125/sqft)</option>
                  <option value="160">Spanish Sintered Porcelain ($160/sqft)</option>
                </select>
              </div>
              <div class="flex flex-col gap-1.5">
                <label class="text-[10px] font-bold text-stone-400 uppercase tracking-wider font-mono">Edge Molding Detail</label>
                <select id="calc-edge-class" class="bg-obsidian-950 border border-obsidian-800 focus:border-gold-500 rounded px-4 py-3 text-xs text-white focus:outline-none transition-colors">
                  <option value="0">Standard Eased / Beveled ($0)</option>
                  <option value="15">Full Bullnose Finishing (+$15/lf)</option>
                  <option value="35">Luxury Hand-Carved Ogee Curve (+$35/lf)</option>
                </select>
              </div>
            </div>

            <!-- Column 2 -->
            <div class="flex flex-col gap-4">
              <div class="flex flex-col gap-1.5">
                <label class="text-[10px] font-bold text-stone-400 uppercase tracking-wider font-mono">Cabinet Linear Feet</label>
                <input id="calc-cabinet-feet" type="number" value="20" min="0" max="150" class="bg-obsidian-950 border border-obsidian-800 focus:border-gold-500 rounded px-4 py-3 text-xs text-white focus:outline-none transition-colors" />
              </div>
              <div class="flex flex-col gap-1.5">
                <label class="text-[10px] font-bold text-stone-400 uppercase tracking-wider font-mono">Cabinet Premium Level</label>
                <select id="calc-cabinet-class" class="bg-obsidian-950 border border-obsidian-800 focus:border-gold-500 rounded px-4 py-3 text-xs text-white focus:outline-none transition-colors">
                  <option value="0">No Cabinet Work ($0)</option>
                  <option value="180" selected>Premium Shaker Wood Cabinet ($180/lf)</option>
                  <option value="280">Bespoke In-House Exotic Hardwood ($280/lf)</option>
                </select>
              </div>
              <!-- Extras toggles -->
              <div class="flex flex-wrap gap-4 mt-2">
                <label class="flex items-center gap-2 text-[10px] text-stone-400 uppercase tracking-wider font-mono cursor-pointer select-none">
                  <input id="calc-demo" type="checkbox" checked class="accent-gold-500 w-4 h-4 rounded border-obsidian-800" />
                  Demolition (+ $350)
                </label>
                <label class="flex items-center gap-2 text-[10px] text-stone-400 uppercase tracking-wider font-mono cursor-pointer select-none">
                  <input id="calc-sink" type="checkbox" checked class="accent-gold-500 w-4 h-4 rounded border-obsidian-800" />
                  Sink Plumbing (+ $450)
                </label>
              </div>
            </div>
          </form>

          <!-- Estimation Output Box -->
          <div class="bg-obsidian-950 border border-gold-600/10 rounded-xl p-6 mt-8 flex flex-col sm:flex-row justify-between items-center gap-4">
            <div>
              <span class="text-[10px] font-bold text-stone-500 uppercase tracking-wider font-mono">Approximate Custom Budget</span>
              <div class="flex items-baseline gap-1 mt-1">
                <span id="price-output" class="text-3xl sm:text-4xl font-serif text-white font-bold">$6,950</span>
                <span class="text-xs text-stone-500 font-mono uppercase font-semibold">Total Est.</span>
              </div>
              <p class="text-[9px] text-stone-500 leading-normal mt-1 max-w-sm">Includes digital templating, in-house shop fabrication, delivery, and certified installation.</p>
            </div>
            <button onclick="bookThisEstimate()" class="w-full sm:w-auto bg-gradient-to-r from-gold-600 to-gold-500 hover:from-gold-500 hover:to-gold-400 text-obsidian-950 font-bold text-xs py-4 px-8 rounded tracking-wider uppercase font-display transition-all shadow-md">
              Lock In My Design Estimate
            </button>
          </div>
          
        </div>
      </div>
    </section>

    <!-- 10. FOOTER -->
    <footer class="bg-obsidian-950 border-t border-obsidian-900 text-stone-500 py-16 px-4">
      <div class="max-w-7xl mx-auto grid grid-cols-1 md:grid-cols-4 gap-8 mb-12">
        <div class="flex flex-col gap-4">
          <div class="flex items-center gap-2">
            <span class="font-serif font-bold text-white tracking-widest text-sm">INNOVATION</span>
            <span class="font-serif text-[10px] text-gold-500 tracking-[0.3em] font-semibold">KITCHEN & BATH</span>
          </div>
          <p class="text-xs text-stone-500 leading-relaxed font-light">
            Providing high-end residential kitchen, bathroom, and cabinetry remodeling across Central Florida since 2011. Elite materials, sub-millimeter measurements, in-house CNC waterjet cutting.
          </p>
        </div>
        <div>
          <h4 class="text-white text-xs font-bold uppercase tracking-wider font-mono mb-4">Design Tools</h4>
          <ul class="flex flex-col gap-2.5 text-xs">
            <li><a href="#showroom" class="hover:text-gold-400 transition-colors">Orlando Material Slabs Showroom</a></li>
            <li><a href="#quote" class="hover:text-gold-400 transition-colors">Interactive Cost Planner</a></li>
            <li><a href="#about" class="hover:text-gold-400 transition-colors">Our In-House Craftsmanship</a></li>
          </ul>
        </div>
        <div>
          <h4 class="text-white text-xs font-bold uppercase tracking-wider font-mono mb-4">Slab Materials</h4>
          <ul class="flex flex-col gap-2.5 text-xs text-stone-500 font-light">
            <li>Calacatta engineered Quartz</li>
            <li>Hand-polished Absolute Black Granite</li>
            <li>Exotic Brazilian Taj Mahal Quartzite</li>
            <li>Spanish Statuario Sintered Porcelain</li>
          </ul>
        </div>
        <div>
          <h4 class="text-white text-xs font-bold uppercase tracking-wider font-mono mb-4">Central Florida Studio</h4>
          <p class="text-xs text-stone-500 leading-relaxed font-mono">
            Orlando Slabs Sourcing Shop<br/>
            Call: (407) 989-2802<br/>
            Email: Innovationkb1@gmail.com<br/>
            Open Mon-Sat: 8:00 AM - 6:00 PM
          </p>
        </div>
      </div>
      <div class="max-w-7xl mx-auto pt-8 border-t border-obsidian-900 flex flex-col md:flex-row justify-between items-center gap-4 text-[10px] font-mono uppercase tracking-wider">
        <p>&copy; 2026 Innovation Kitchen & Bath. All Rights Reserved. Licensed Florida Builder.</p>
        <p class="text-gold-500">Sub-Millimeter Stone Redesign Preview</p>
      </div>
    </footer>

    <!-- Video Modal simulation -->
    <div id="video-modal" class="fixed inset-0 bg-obsidian-950/95 z-50 flex items-center justify-center p-4 hidden transition-opacity duration-300 opacity-0">
      <div class="bg-obsidian-900 border border-gold-600/20 max-w-2xl w-full rounded-2xl overflow-hidden shadow-2xl">
        <div class="px-6 py-4 border-b border-obsidian-800 flex justify-between items-center">
          <span class="text-xs font-bold font-mono text-gold-400">IKB Continuous-Vein CNC Demo</span>
          <button onclick="closeSimulationVideo()" class="text-stone-400 hover:text-white font-bold text-xs uppercase focus:outline-none">Close</button>
        </div>
        <div class="aspect-video bg-obsidian-950 flex items-center justify-center relative p-6 text-center">
          <!-- simulated video clip placeholder -->
          <div class="flex flex-col items-center gap-4 max-w-sm">
            <span class="animate-ping w-3 h-3 rounded-full bg-gold-400 block"></span>
            <span class="text-xs font-bold text-white tracking-widest uppercase font-mono mt-1">SIMULATING IN-SHOP WATERJET CLIP</span>
            <p class="text-[11px] text-stone-400 leading-normal">Our computerized waterjets execute cuts mapping exact continuous ribbons across 3cm quartz slabs with millimeter alignment precision.</p>
          </div>
        </div>
      </div>
    </div>

    <!-- Active Studio Toast Notifications -->
    <div id="toast-notif" class="fixed bottom-6 right-6 bg-obsidian-900 border border-gold-500/40 text-stone-200 px-6 py-4 rounded-xl shadow-2xl z-50 hidden transition-all duration-300 max-w-sm transform translate-y-10">
      <div class="flex items-center gap-3">
        <div class="w-2 h-2 rounded-full bg-gold-500 animate-pulse flex-shrink-0"></div>
        <p id="toast-message" class="text-xs font-medium font-sans leading-relaxed">Notifications detail here.</p>
      </div>
    </div>

    <!-- Interactive JavaScript Logic -->
    <script>
      // 1. Scroll-Triggered Reveal Animations using IntersectionObserver
      const observerOptions = {
        threshold: 0.1,
        rootMargin: '0px 0px -50px 0px'
      };

      const revealCallback = (entries, observer) => {
        entries.forEach(entry => {
          if (entry.isIntersecting) {
            entry.target.classList.add('active');
            // Stop observing once animated
            observer.unobserve(entry.target);
          }
        });
      };

      const scrollObserver = new IntersectionObserver(revealCallback, observerOptions);

      document.addEventListener('DOMContentLoaded', () => {
        // Find elements to animate on scroll
        const elementsToReveal = document.querySelectorAll('.reveal, .reveal-left, .reveal-right');
        elementsToReveal.forEach(el => scrollObserver.observe(el));
        
        // Run initial price calculations
        calculateEstimate();
      });

      // 2. Dual Portal Hero toggles
      function togglePortal(type) {
        const bgRes = document.getElementById('hero-bg-residential');
        const bgComm = document.getElementById('hero-bg-commercial');
        const btnRes = document.getElementById('btn-portal-residential');
        const btnComm = document.getElementById('btn-portal-commercial');
        
        const subtitle = document.getElementById('hero-subtitle');
        const title = document.getElementById('hero-title');
        const desc = document.getElementById('hero-desc');

        if (type === 'residential') {
          bgRes.style.opacity = '0.3';
          bgComm.style.opacity = '0';
          btnRes.className = 'px-5 py-2 rounded text-xs font-bold transition-all duration-500 tracking-wider uppercase bg-gold-500 text-obsidian-950';
          btnComm.className = 'px-5 py-2 rounded text-xs font-bold transition-all duration-500 tracking-wider uppercase text-stone-400 hover:text-white';
          
          subtitle.textContent = 'CENTRAL FLORIDA PRESTIGE LIVING';
          title.innerHTML = 'Crafting High-End Custom <br/>Residential Spaces';
          desc.textContent = 'Specializing in luxury kitchen, bath, and cabinetry fabrication using premium granite, engineered quartz, and Spanish porcelain slabs since 2011.';
        } else {
          bgRes.style.opacity = '0';
          bgComm.style.opacity = '0.3';
          btnComm.className = 'px-5 py-2 rounded text-xs font-bold transition-all duration-500 tracking-wider uppercase bg-gold-500 text-obsidian-950';
          btnRes.className = 'px-5 py-2 rounded text-xs font-bold transition-all duration-500 tracking-wider uppercase text-stone-400 hover:text-white';
          
          subtitle.textContent = 'ARCHITECTURAL STONE FABRICATION';
          title.innerHTML = 'Premium Commercial Slabs <br/>& Heavy Claddings';
          desc.textContent = 'Providing CNC waterjet alignments, certified high-density office countertops, medical-grade composites, and bookmatched stone slabs since 2011.';
        }
      }

      // 3. Material Catalogue Filter (Image 2 Slabs)
      function filterSlabs(category) {
        // Toggle active button borders
        const buttons = document.querySelectorAll('.slab-filter-btn');
        buttons.forEach(btn => {
          if (btn.textContent.toLowerCase() === category) {
            btn.className = 'slab-filter-btn px-4 py-1.5 rounded-full text-xs font-bold tracking-wide border border-gold-500 bg-gold-500 text-obsidian-950 transition-all';
          } else {
            btn.className = 'slab-filter-btn px-4 py-1.5 rounded-full text-xs font-bold tracking-wide border border-obsidian-800 text-stone-400 hover:text-white hover:border-stone-700 transition-all';
          }
        });

        const cards = document.querySelectorAll('.slab-card');
        cards.forEach(card => {
          if (category === 'all' || card.getAttribute('data-category') === category) {
            card.style.display = 'flex';
          } else {
            card.style.display = 'none';
          }
        });
      }

      function selectSlabToCostPlanner(slabName, materialValue) {
        const selector = document.getElementById('calc-material-class');
        if (selector) {
          selector.value = materialValue;
          calculateEstimate();
        }
        showStudioToast(`Loaded ${slabName} into active Cost Planner selection.`);
        // Scroll smoothly to cost planner
        document.getElementById('quote').scrollIntoView({ behavior: 'smooth' });
      }

      // 5. In-App Studio Toasts
      function showStudioToast(message) {
        const toast = document.getElementById('toast-notif');
        const toastMsg = document.getElementById('toast-message');
        toastMsg.textContent = message;
        
        toast.classList.remove('hidden');
        setTimeout(() => {
          toast.classList.remove('translate-y-10');
        }, 10);

        // Auto hide
        setTimeout(() => {
          toast.classList.add('translate-y-10');
          setTimeout(() => {
            toast.classList.add('hidden');
          }, 300);
        }, 3500);
      }

      // 6. Interactive Price Estimator Math
      function calculateEstimate() {
        const counterFeet = parseFloat(document.getElementById('calc-counter-feet').value) || 0;
        const matVal = parseFloat(document.getElementById('calc-material-class').value) || 0;
        const edgeVal = parseFloat(document.getElementById('calc-edge-class').value) || 0;
        
        const cabinetFeet = parseFloat(document.getElementById('calc-cabinet-feet').value) || 0;
        const cabVal = parseFloat(document.getElementById('calc-cabinet-class').value) || 0;
        
        const demoChecked = document.getElementById('calc-demo').checked;
        const sinkChecked = document.getElementById('calc-sink').checked;

        // Formula: Countertop Cost = feet * depth (2.1ft standard) * matPrice + feet * edgePrice
        const counterCost = (counterFeet * 2.1 * matVal) + (counterFeet * edgeVal);
        
        // Cabinet Cost = feet * cabinetPrice
        const cabinetCost = cabinetFeet * cabVal;
        
        // Extras
        const demoCost = demoChecked ? 350 : 0;
        const sinkCost = sinkChecked ? 450 : 0;

        const totalCost = counterCost + cabinetCost + demoCost + sinkCost;

        // Display formatted price
        document.getElementById('price-output').textContent = '$' + Math.round(totalCost).toLocaleString();
      }

      function bookThisEstimate() {
        const total = document.getElementById('price-output').textContent;
        showStudioToast(`Pricing locked! Your consultation estimate of ${total} is transferred to booking form.`);
      }

      // 7. Simulated Video popup (Image 4 Demo Video)
      // Play
      function playSimulationVideo() {
        const modal = document.getElementById('video-modal');
        modal.classList.remove('hidden');
        setTimeout(() => {
          modal.classList.remove('opacity-0');
        }, 10);
      }

      // Close
      function closeSimulationVideo() {
        const modal = document.getElementById('video-modal');
        modal.classList.add('opacity-0');
        setTimeout(() => {
          modal.classList.add('hidden');
        }, 300);
      }
    </script>
  </body>
</html>
