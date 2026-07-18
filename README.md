<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>The Conscious Compass Travel Co.</title>
    <!-- Tailwind CSS for modern, responsive layout styling -->
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400..900;1,400..900&family=Plus+Jakarta+Sans:ital,wght@0,200..800;1,200..800&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Plus Jakarta Sans', sans-serif;
            background-color: #FAF6F0; /* Warm linen background */
            color: #2C302E; /* Deep charcoal */
            scroll-behavior: smooth;
        }
        h1, h2, h3, h4, .serif {
            font-family: 'Playfair Display', serif;
        }
    </style>
</head>
<body class="min-h-screen flex flex-col justify-between selection:bg-stone-200 relative overflow-x-hidden">

    <!-- Layered Watercolor Displacement Filter for Hand-Painted Hummingbird Aesthetics -->
    <svg class="hidden">
        <defs>
            <filter id="watercolor-displacement">
                <feTurbulence type="fractalNoise" baseFrequency="0.04" numOctaves="3" result="noise" />
                <feDisplacementMap in="SourceGraphic" in2="noise" scale="7" xChannelSelector="R" yChannelSelector="G" />
            </filter>
        </defs>
    </svg>

    <!-- Interactive Custom Watercolor Violet-Eared Hummingbird Asset -->
    <div id="hummingbird-container" class="fixed right-6 top-32 z-50 w-24 h-24 pointer-events-none md:pointer-events-auto transition-transform duration-300 ease-out select-none">
        <svg id="hummingbird-svg" viewBox="0 0 160 120" class="w-full h-full drop-shadow-sm filter" style="filter: url(#watercolor-displacement); transform-origin: 88px 50px;">
            <!-- Soft Watercolor Translucent Gradients -->
            <defs>
                <linearGradient id="body-grad" x1="0%" y1="0%" x2="100%" y2="100%">
                    <stop offset="0%" stop-color="#4E5142" stop-opacity="0.85" />
                    <stop offset="40%" stop-color="#8C7A6B" stop-opacity="0.9" />
                    <stop offset="80%" stop-color="#3D4035" stop-opacity="0.8" />
                </linearGradient>
                <linearGradient id="wing-grad" x1="0%" y1="0%" x2="100%" y2="100%">
                    <stop offset="0%" stop-color="#3D4035" stop-opacity="0.65" />
                    <stop offset="60%" stop-color="#4E5142" stop-opacity="0.75" />
                    <stop offset="100%" stop-color="#8C7A6B" stop-opacity="0.55" />
                </linearGradient>
            </defs>
            
            <!-- Long Slender Hummingbird Beak -->
            <path d="M 10 38 Q 45 42 75 42" stroke="#2C302E" stroke-width="1.5" stroke-linecap="round" fill="none" />
            
            <!-- Swept-back Layered Tail Feathers -->
            <path d="M 65 82 C 50 95 30 105 15 110 C 35 98 50 88 58 80 Z" fill="url(#body-grad)" />
            <path d="M 62 82 C 45 100 25 112 8 116 C 28 102 45 92 54 81 Z" fill="url(#body-grad)" class="opacity-80" />

            <!-- Underwing (Anatomical Flutter Action Layer) -->
            <g id="underwing" style="transform-origin: 88px 50px;">
                <path d="M 88 50 C 100 20 115 -10 130 -15 C 120 10 105 30 88 50 Z" fill="url(--wing-grad)" />
            </g>

            <!-- Anatomical Body Contour (Sleek throat, swelling chest & slender belly) -->
            <path d="M 75 42 Q 85 35 92 40 C 105 48 108 65 98 75 C 88 85 75 88 65 82 C 55 76 50 62 58 52 C 64 44 80 40 92 40 Z" fill="url(#body-grad)" />
            
            <!-- Tiny Delicate Eye -->
            <circle cx="82" cy="38" r="1.5" fill="#2C302E" />

            <!-- Overwing (Anatomical Flutter Action Layer) -->
            <g id="overwing" style="transform-origin: 88px 50px;">
                <path d="M 88 50 C 110 15 135 -15 155 -25 C 135 15 110 40 88 50 Z" fill="url(#wing-grad)" />
            </g>
        </svg>
    </div>

    <!-- Elegant Text Branding -->
    <header class="py-10 px-4 text-center max-w-4xl mx-auto">
        <h1 class="text-3xl md:text-5xl font-semibold tracking-widest text-[#3D4035] uppercase">
            The Conscious Compass
        </h1>
        <!-- High Impact Placement: Core Sub-Headline Positioning Statement -->
        <p class="text-xs md:text-sm tracking-[0.35em] font-medium text-[#4E5142] uppercase mt-3 italic">
            For the conscious traveler.
        </p>
        <p class="text-[10px] md:text-xs tracking-[0.25em] text-[#8C7A6B] uppercase mt-4 font-semibold border-t border-stone-200/60 pt-4 inline-block px-6">
            Travel Co. • Intentionally Curated Journeys
        </p>
    </header>

    <main class="w-full max-w-4xl mx-auto px-4 pb-20 flex-grow">
        
        <!-- Landscape Watercolor Banner Block -->
        <div class="relative w-full aspect-[21/9] rounded-2xl overflow-hidden shadow-sm bg-stone-100 border border-stone-200/40 mb-12">
            <img id="banner" src="landscape.jpg" alt="Rainforest Artistry Canvas" class="w-full h-full object-cover object-[50%_50%] transition-opacity duration-500 opacity-0" onload="this.classList.remove('opacity-0')">
            
            <!-- Safe Fallback: If landscape.jpg is missing, load a moody rainforest canopy -->
            <script>
                document.getElementById('banner').onerror = function() {
                    this.src = "https://images.unsplash.com/photo-1516026672322-bc52d61a55d5?auto=format&fit=crop&w=1200&q=80";
                };
            </script>
        </div>

        <!-- Section 1: Expandable "Meet Your Travel Architect" Intro -->
        <section class="max-w-4xl mx-auto mb-16 bg-white/40 border border-stone-200/40 rounded-3xl p-6 md:p-10 shadow-sm">
            <div class="text-center max-w-2xl mx-auto">
                <span class="text-xs tracking-[0.2em] text-[#8C7A6B] uppercase font-bold">The Curator</span>
                <h2 class="text-3xl font-medium text-[#3D4035] mt-2 mb-6">Meet Your Travel Architect</h2>
            </div>
            
            <div class="text-stone-600 leading-relaxed text-sm md:text-base max-w-3xl mx-auto">
                <!-- Hook Paragraph: Always Visible -->
                <p class="font-medium text-[#4E5142] italic text-center text-base md:text-lg mb-6 leading-relaxed max-w-2xl mx-auto">
                    An exceptional travel experience is born from the tension between raw adventure and meticulous design. It requires a planner who looks past generic, glossy brochures and instead understands how to read a landscape, decode unpredictable infrastructure, and engage intentionally with local community networks.
                </p>
                
                <!-- Expandable Deep-Dive Split Grid Panel -->
                <div id="about-extended" class="hidden border-t border-stone-200/60 pt-8 mt-6">
                    <div class="flex flex-col md:flex-row gap-8 items-start">
                        <!-- Left Column: Biography Narrative -->
                        <div class="md:w-3/5 space-y-5 text-left text-xs md:text-sm leading-relaxed">
                            <p>
                                My career has been defined by the art of <strong class="text-[#3D4035] font-semibold">curation</strong>. As a multidisciplinary artist and educator, I have spent years exploring the intersection of visual storytelling, global connectivity, and geographic navigation. In the art world, curation is about selecting, organizing, and presenting elements to tell a profound, cohesive story. In high-end travel design, I apply that exact same artistic lens. I do not just book trips; I curate immersive, sensory, and highly intentional environments for you to experience.
                            </p>
                            <p>
                                My design philosophy is built from firsthand, real-world experience navigating diverse international terrains—from the dense canopy systems of Central America to complex, transit-heavy urban landscapes. Having mapped out and executed deep-dive family travels and eco-conscious expeditions across the globe, I launched <strong class="text-[#3D4035] font-semibold">The Conscious Compass Travel Co.</strong> to provide travelers with an entirely new standard of travel intelligence.
                            </p>
                            <p>
                                I specialize in translating complex international logistics, regional transit systems, and intricate cultural topographies into a singular, beautifully curated blueprint. My focus is entirely on slow, sustainable, and eco-conscious travel—crafting journeys that honor the ecosystems we visit while protecting the absolute safety, structural comfort, and culinary needs of your travel party. I don't just tell you where to go; I give you the complete spatial awareness, transit protocols, and expertly curated neighborhood insights you need to experience a destination with complete, unwavering confidence.
                            </p>
                            <p class="font-medium text-[#4E5142] italic pt-3 text-sm">
                                Let’s step away from the endless planning loops and curate your next masterpiece.
                            </p>
                        </div>
                        
                        <!-- Right Column: Portrait and Stationery Logo Stacking Grid -->
                        <div class="md:w-2/5 w-full flex flex-col gap-5 shrink-0">
                            <!-- Portrait Frame -->
                            <div class="rounded-2xl overflow-hidden border border-stone-200/60 shadow-sm aspect-square bg-stone-100">
                                <img id="about-portrait" src="Portrait.jpg" alt="Travel Architect Portrait" class="w-full h-full object-cover transition-opacity duration-500 opacity-0" onload="this.classList.remove('opacity-0')">
                            </div>
                            <!-- Logo Frame (Clean and direct reference to Logo.jpg) -->
                            <div class="rounded-2xl overflow-hidden border border-stone-200/60 shadow-sm bg-white p-2">
                                <img id="about-logo" src="Logo.jpg" alt="The Conscious Compass Logo" class="w-full h-auto rounded-xl transition-opacity duration-500 opacity-0" onload="this.classList.remove('opacity-0')">
                            </div>

                            <script>
                                // Fallback scripts to keep the preview beautiful before you upload your local assets
                                document.getElementById('about-portrait').onerror = function() {
                                    this.src = "https://images.unsplash.com/photo-1534528741775-53994a69daeb?auto=format&fit=crop&w=600&q=80";
                                    this.classList.remove('opacity-0');
                                };
                                document.getElementById('about-logo').onerror = function() {
                                    this.src = "https://images.unsplash.com/photo-1513542789411-b6a5d4f31634?auto=format&fit=crop&w=600&q=80";
                                    this.classList.remove('opacity-0');
                                };
                            </script>
                        </div>
                    </div>
                </div>
                
                <!-- Interactive Toggle Button -->
                <div class="text-center pt-4">
                    <button id="about-toggle-btn" onclick="toggleAbout()" class="inline-flex items-center gap-2 text-xs font-semibold tracking-wider uppercase text-[#8C7A6B] hover:text-[#3D4035] border-b border-[#8C7A6B] pb-1 transition-colors focus:outline-none">
                        <span id="about-toggle-text">Read My Full Story</span>
                        <svg id="about-toggle-icon" class="w-3 h-3 transform transition-transform duration-200 text-[#8C7A6B]" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" d="M19 9l-7 7-7-7"></path>
                        </svg>
                    </button>
                </div>
            </div>
        </section>

        <hr class="border-stone-200/60 my-16">

        <!-- Section 2: Restructured Horizontal Service Tiers -->
        <section class="mb-20 max-w-4xl mx-auto">
            <div class="text-center mb-12">
                <span class="text-xs tracking-[0.2em] text-[#8C7A6B] uppercase font-bold">Services & Blueprints</span>
                <h2 class="text-3xl md:text-4xl font-medium text-[#3D4035] mt-2">The Three Curated Tiers</h2>
                <p class="text-stone-500 text-sm mt-3">Choose the level of design, scaffolding, and support your journey requires.</p>
            </div>

            <div class="space-y-6">
                <!-- Tier 1: Horizontal Framework Layout -->
                <div class="bg-white p-6 md:p-8 border border-stone-200/60 rounded-3xl flex flex-col md:flex-row gap-6 md:gap-8 shadow-sm hover:shadow-md transition items-stretch">
                    <!-- Left Column Anchor -->
                    <div class="md:w-1/4 flex flex-col justify-between border-b md:border-b-0 md:border-r border-stone-200/40 pb-5 md:pb-0 md:pr-6 min-w-[200px]">
                        <div>
                            <span class="text-xs font-bold tracking-wider text-[#8C7A6B] uppercase">Tier 1</span>
                            <h3 class="text-lg font-bold text-[#3D4035] mt-1 leading-snug">The Deep-Dive Research Blueprint</h3>
                            <p class="text-2xl font-semibold text-[#4E5142] mt-3">$175 <span class="text-xs text-stone-500 font-normal block md:inline">/ focus topic</span></p>
                        </div>
                        <a href="#discover" class="block text-center mt-6 bg-stone-100 hover:bg-stone-200 text-[#3D4035] font-semibold text-xs py-3 rounded-xl transition">
                            Select Blueprint ➔
                        </a>
                    </div>
                    <!-- Right Column Spaced Content -->
                    <div class="md:w-3/4 flex flex-col justify-center space-y-4 text-xs md:text-sm text-stone-600">
                        <p class="italic text-stone-700"><strong class="text-stone-800 font-semibold">Perfect For:</strong> The confident DIY traveler or anxious planner who loves booking their own trips but wants an expert to eliminate the stress of logistics, safety, or complex international entry requirements.</p>
                        <p><strong class="text-stone-800 font-semibold">What You Receive:</strong> A highly organized, comprehensive custom PDF document focusing entirely on what is keeping you up at night.</p>
                        
                        <div class="pt-2 space-y-2.5">
                            <span class="block font-bold tracking-wider text-[10px] uppercase text-stone-400">Included Deliverables:</span>
                            <div class="grid grid-cols-1 sm:grid-cols-2 gap-x-6 gap-y-3 text-xs">
                                <div class="flex gap-2"><span class="text-stone-400">🗺️</span> <span><strong class="text-stone-800">Custom Logistics Map:</strong> Step-by-step public transit breakdowns, train routing, or private transit options.</span></div>
                                <div class="flex gap-2"><span class="text-stone-400">🛂</span> <span><strong class="text-stone-800">Bureaucracy Guide:</strong> Up-to-date visa checkpoints, digital landing forms, and entry immunization protocols.</span></div>
                                <div class="flex gap-2"><span class="text-stone-400">🛡️</span> <span><strong class="text-stone-800">Safety Briefing:</strong> Neighborhood security maps, active regional scams to avoid, and emergency contact points.</span></div>
                                <div class="flex gap-2"><span class="text-stone-400">📋</span> <span><strong class="text-stone-800">Packing Checklists:</strong> Tailored gear profiles for your destination's explicit topography or micro-climate.</span></div>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Tier 2: Horizontal Framework Layout -->
                <div class="bg-white p-6 md:p-8 border border-stone-200/60 rounded-3xl flex flex-col md:flex-row gap-6 md:gap-8 shadow-sm hover:shadow-md transition items-stretch">
                    <!-- Left Column Anchor -->
                    <div class="md:w-1/4 flex flex-col justify-between border-b md:border-b-0 md:border-r border-stone-200/40 pb-5 md:pb-0 md:pr-6 min-w-[200px]">
                        <div>
                            <span class="text-xs font-bold tracking-wider text-[#8C7A6B] uppercase">Tier 2</span>
                            <h3 class="text-lg font-bold text-[#3D4035] mt-1 leading-snug">The "Day-Hacker" Partial Itinerary</h3>
                            <p class="text-2xl font-semibold text-[#4E5142] mt-3">$75 <span class="text-xs text-stone-500 font-normal block md:inline">/ planned day</span></p>
                            <p class="text-[10px] text-stone-400 italic mt-1">*Minimum of 2 days required</p>
                        </div>
                        <a href="#discover" class="block text-center mt-6 bg-stone-100 hover:bg-stone-200 text-[#3D4035] font-semibold text-xs py-3 rounded-xl transition">
                            Select Day-Hacker ➔
                        </a>
                    </div>
                    <!-- Right Column Spaced Content -->
                    <div class="md:w-3/4 flex flex-col justify-center space-y-4 text-xs md:text-sm text-stone-600">
                        <p class="italic text-stone-700"><strong class="text-stone-800 font-semibold">Perfect For:</strong> Travelers who have 70% of their trip figured out but are completely stuck on how to maximize a specific multi-day stretch, handle a complex transit day, or curate a flawless hidden-gem experience.</p>
                        <p><strong class="text-stone-800 font-semibold">What You Receive:</strong> Seamless, hourly time-blocked execution blueprints for the specific dates requested, designed to plug directly into your existing calendar.</p>
                        
                        <div class="pt-2 space-y-2.5">
                            <span class="block font-bold tracking-wider text-[10px] uppercase text-stone-400">Included Deliverables:</span>
                            <div class="grid grid-cols-1 sm:grid-cols-2 gap-x-6 gap-y-3 text-xs">
                                <div class="flex gap-2"><span class="text-stone-400">⏱️</span> <span><strong class="text-stone-800">Optimized Flow:</strong> Minute-by-minute or block pacing to eliminate city crisscrossing bottlenecks.</span></div>
                                <div class="flex gap-2"><span class="text-stone-400">🍽️</span> <span><strong class="text-stone-800">Curated Culinary Matches:</strong> Hidden local dining markers and market walking loops mapped for those specific dates.</span></div>
                                <div class="flex gap-2"><span class="text-stone-400">📍</span> <span><strong class="text-stone-800">"Getting There" Blueprint:</strong> Explicit transfer directives, platform codes, and link connections.</span></div>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Tier 3: Horizontal Framework Layout (Flagship Row Highlight) -->
                <div class="bg-[#FAF6F0] p-6 md:p-8 border-2 border-[#8C7A6B]/50 rounded-3xl flex flex-col md:flex-row gap-6 md:gap-8 shadow-sm relative overflow-hidden items-stretch">
                    <div class="absolute top-0 right-0 bg-[#8C7A6B] text-white text-[9px] tracking-wider uppercase py-1 px-4 rounded-bl-xl font-bold shadow-xs">
                        Flagship Service
                    </div>
                    <!-- Left Column Anchor -->
                    <div class="md:w-1/4 flex flex-col justify-between border-b md:border-b-0 md:border-r border-stone-300 pb-5 md:pb-0 md:pr-6 min-w-[200px]">
                        <div>
                            <span class="text-xs font-bold tracking-wider text-[#8C7A6B] uppercase block mt-2">Tier 3</span>
                            <h3 class="text-lg font-bold text-[#3D4035] mt-1 leading-snug">The All-Inclusive Custom Retainer</h3>
                            
                            <div class="space-y-0.5 mt-3">
                                <p class="text-base font-semibold text-[#4E5142]">$450 <span class="text-[10px] text-stone-500 font-normal">/ 1–7 Day Trip</span></p>
                                <p class="text-base font-semibold text-[#4E5142]">$750 <span class="text-[10px] text-stone-500 font-normal">/ 8–14 Day Journey</span></p>
                                <p class="text-[9px] text-stone-400 italic">Trips 15+ days customized on request</p>
                            </div>
                        </div>
                        <a href="#discover" class="block text-center mt-6 bg-[#4E5142] hover:bg-[#3D4035] text-white font-semibold text-xs py-3 rounded-xl transition shadow-xs">
                            Retain Travel Architect ➔
                        </a>
                    </div>
                    <!-- Right Column Spaced Content -->
                    <div class="md:w-3/4 flex flex-col justify-center space-y-4 text-xs md:text-sm text-stone-600">
                        <p class="italic text-stone-700"><strong class="text-stone-800 font-semibold">Perfect For:</strong> The busy traveler who wants a flawless, deeply intentional international vacation from start to finish without spending 40 hours staring at travel forums and cross-referencing maps.</p>
                        <p><strong class="text-stone-800 font-semibold">What You Receive:</strong> A complete, beautifully mapped, comprehensive end-to-end travel blueprint.</p>
                        
                        <div class="pt-2 space-y-2.5">
                            <span class="block font-bold tracking-wider text-[10px] uppercase text-stone-400">Included Deliverables:</span>
                            <div class="grid grid-cols-1 sm:grid-cols-2 gap-x-6 gap-y-3 text-xs">
                                <div class="flex gap-2"><span class="text-stone-400">✨</span> <span><strong class="text-stone-800">The Signature Blueprint:</strong> Comprehensive multi-page master document matching Tiers 1 and 2 for the entire duration.</span></div>
                                <div class="flex gap-2"><span class="text-stone-400">🏨</span> <span><strong class="text-stone-800">Accommodation Shortlists:</strong> 2–3 hand-selected, verified independent boutique lodging matches with link anchors.</span></div>
                                <div class="flex gap-2"><span class="text-stone-400">🔄</span> <span><strong class="text-stone-800">Two Revision Rounds:</strong> Collaborative aesthetic adjustments to tweak pace and environmental balance.</span></div>
                                <div class="flex gap-2"><span class="text-[#8C7A6B]">🎁</span> <span><strong class="text-stone-800">Complimentary Travel Print:</strong> Choose any signature 8x10 watercolor landscape print — shipped straight to your wall.</span></div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <hr class="border-stone-200/60 my-16">

        <!-- Section 3: Fine Art Travel Prints & Commissions -->
        <section class="mb-20">
            <div class="text-center mb-12">
                <span class="text-xs tracking-[0.2em] text-[#8C7A6B] uppercase font-bold">The Artist's Gallery</span>
                <h2 class="text-3xl md:text-4xl font-medium text-[#3D4035] mt-2">Travel Prints & Commissions</h2>
                <p class="text-stone-500 text-sm mt-3 max-w-lg mx-auto">
                    Bring the vibrant atmosphere of your journey home through physical, hand-rendered artwork.
                </p>
            </div>

            <div class="grid grid-cols-1 sm:grid-cols-2 gap-8 max-w-2xl mx-auto items-stretch">
                <!-- Standalone Prints -->
                <div class="bg-white p-3 rounded-2xl shadow-sm border border-stone-200/40 flex flex-col justify-between">
                    <div>
                        <div class="aspect-[4/3] rounded-xl overflow-hidden bg-stone-100">
                            <img src="landscape.jpg" alt="Misty Canoe Watercolor Print" class="w-full h-full object-cover">
                        </div>
                        <div class="mt-4 px-2">
                            <span class="text-[10px] font-bold tracking-wider text-[#8C7A6B] uppercase">Fine Art Editions</span>
                            <div class="flex justify-between items-baseline mt-0.5">
                                <h4 class="font-bold text-[#3D4035] text-sm">Watercolor Travel Prints</h4>
                                <span class="text-sm font-semibold text-[#4E5142]">$35.00</span>
                            </div>
                            <p class="text-xs text-stone-500 mt-2 leading-relaxed">
                                Fine art reproductions of on-location landscape sketches, cloudy forest channels, mountain passes, or historic streets. Every standard print featured across our portfolio is available in a classic <strong class="text-stone-800">8x10 size</strong>, perfectly structured for standard framing.
                            </p>
                            <div class="mt-4 pt-3 border-t border-stone-100 space-y-2">
                                <p class="text-xs text-[#8C7A6B] font-medium italic">
                                    🎁 Complimentary for Tier 3 clients. Select your print of choice in the form below for free home shipping.
                                </p>
                                <p class="text-[11px] text-stone-400 font-medium">
                                    🗓️ Coming Soon: Custom curated greeting card sets, debuting this holiday season.
                                </p>
                            </div>
                        </div>
                    </div>
                    <div class="p-2 pt-4">
                        <a href="#discover" class="block text-center bg-stone-100 hover:bg-stone-200 text-[#3D4035] text-xs font-semibold py-2.5 rounded-lg transition">
                            Order Standard Print ➔
                        </a>
                    </div>
                </div>

                <!-- Custom Commissions Block -->
                <div class="bg-white p-6 rounded-2xl shadow-sm border border-stone-200/40 flex flex-col justify-between text-center">
                    <div class="my-auto py-2">
                        <span class="text-xs tracking-wider uppercase text-[#8C7A6B] font-bold">Bespoke Artifacts</span>
                        <h4 class="text-xl font-semibold text-[#3D4035] mt-1 mb-2">Custom Travel Art Commissions</h4>
                        
                        <div class="space-y-0.5 mb-4">
                            <p class="text-base font-semibold text-[#4E5142]">Original Watercolor (Size A4): $65.00</p>
                            <p class="text-base font-semibold text-[#4E5142]">Original Acrylic (Size A4): $90.00</p>
                        </div>
                        
                        <p class="text-xs text-stone-500 leading-relaxed max-w-xs mx-auto mb-5 text-left">
                            Transform a cherished travel moment into a custom, hand-painted original illustration. Whether capturing the misty canopy of a rainforest, an open savannah, or an ancient alleyway, I specialize in atmospheric, environment-first scenes. Figures can be gently woven in to capture scale and presence, but please note I focus strictly on the spirit of the landscape rather than detailed facial portraiture or portraits.
                        </p>
                        
                        <div class="bg-stone-50/80 border border-stone-200/30 rounded-xl p-3 max-w-xs mx-auto">
                            <p class="text-[10px] text-stone-500">
                                Available as a custom original keepsake across <strong class="text-stone-700">any travel service tier</strong>, or commissioned on its own.
                            </p>
                        </div>
                    </div>
                    <a href="#discover" class="block text-center bg-[#4E5142] hover:bg-[#3D4035] text-white font-semibold text-xs py-3 rounded-lg transition shadow-xs">
                        Request a Commission ➔
                    </a>
                </div>
            </div>
        </section>

        <hr class="border-stone-200/60 my-16">

        <!-- Section 4: Interactive Strategic FAQs (Including the newly integrated "How it Works" question) -->
        <section class="mb-20 max-w-2xl mx-auto">
            <div class="text-center mb-12">
                <span class="text-xs tracking-[0.2em] text-[#8C7A6B] uppercase font-bold">Clarifying the Path</span>
                <h2 class="text-3xl md:text-4xl font-medium text-[#3D4035] mt-2">Frequently Asked Questions</h2>
            </div>

            <div class="divide-y divide-stone-200/60 border-t border-b border-stone-200/60">
                <!-- FAQ Item 1: REIMAGINED "HOW IT WORKS" TIMELINE -->
                <div class="group py-4">
                    <button class="w-full text-left py-4 font-semibold text-sm md:text-base text-[#3D4035] flex justify-between items-center focus:outline-none select-none transition-colors" onclick="toggleFAQ(1)">
                        <span class="flex items-center gap-4">
                            <span class="text-xs font-serif italic text-[#8C7A6B]/50 font-normal tracking-wide">01</span>
                            <span>How does this process work from start to finish?</span>
                        </span>
                        <svg id="icon-1" class="w-4 h-4 text-[#8C7A6B] transform transition-transform duration-300" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" d="M19 9l-7 7-7-7"></path>
                        </svg>
                    </button>
                    <!-- Silk-smooth CSS Sliding Drawer Container -->
                    <div id="faq-1" class="max-h-0 overflow-hidden opacity-0 transition-all duration-500 ease-in-out">
                        <div class="pb-6 pl-8 text-xs md:text-sm text-stone-600 space-y-6 pt-2 border-l-2 border-[#8C7A6B]/20 ml-2.5">
                            <!-- Step 1 -->
                            <div class="relative pl-6">
                                <div class="absolute -left-[31px] top-1 bg-[#8C7A6B] w-2.5 h-2.5 rounded-full border-2 border-white ring-4 ring-[#FAF6F0]"></div>
                                <h4 class="font-bold text-[#3D4035] mb-1">1. Submit Your Parameters</h4>
                                <p class="leading-relaxed">Fill out our comprehensive digital Discovery Questionnaire below. Tell us where you are heading, your culinary adventurousness, or fine art details, and the specific variables that are keeping you up at night.</p>
                            </div>
                            <!-- Step 2 -->
                            <div class="relative pl-6">
                                <div class="absolute -left-[31px] top-1 bg-[#8C7A6B] w-2.5 h-2.5 rounded-full border-2 border-white ring-4 ring-[#FAF6F0]"></div>
                                <h4 class="font-bold text-[#3D4035] mb-1">2. Secure Your Retainer</h4>
                                <p class="leading-relaxed">Next, you will receive a digital invoice corresponding to your selected tier. Once processing settles, we immediately deploy our firsthand international research network to engineer your blueprint layout asset.</p>
                            </div>
                            <!-- Step 3 -->
                            <div class="relative pl-6">
                                <div class="absolute -left-[31px] top-1 bg-[#8C7A6B] w-2.5 h-2.5 rounded-full border-2 border-white ring-4 ring-[#FAF6F0]"></div>
                                <h4 class="font-bold text-[#3D4035] mb-1">3. Receive Your Masterpiece</h4>
                                <p class="leading-relaxed">Within 7 to 10 business days, a beautifully formatted, highly scannable, custom digital document lands securely in your inbox, engineered to shift complex planning friction into unwavering global confidence.</p>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- FAQ Item 2 -->
                <div class="group py-4">
                    <button class="w-full text-left py-4 font-semibold text-sm md:text-base text-[#3D4035] flex justify-between items-center focus:outline-none select-none transition-colors" onclick="toggleFAQ(2)">
                        <span class="flex items-center gap-4">
                            <span class="text-xs font-serif italic text-[#8C7A6B]/50 font-normal tracking-wide">02</span>
                            <span>Why should I pay a planning retainer when I can book travel myself or use a traditional agent for free?</span>
                        </span>
                        <svg id="icon-2" class="w-4 h-4 text-[#8C7A6B] transform transition-transform duration-300" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" d="M19 9l-7 7-7-7"></path>
                        </svg>
                    </button>
                    <div id="faq-2" class="max-h-0 overflow-hidden opacity-0 transition-all duration-500 ease-in-out">
                        <div class="pb-6 pl-8 text-xs md:text-sm text-stone-600 leading-relaxed pt-2">
                            Traditional travel agents are primarily compensated through backend commissions from major suppliers, meaning their recommendations can sometimes lean toward large resort chains or bulk cruises that offer standard payouts. At The Conscious Compass, we operate entirely on an independent, fee-for-service model. You are paying for an elite level of custom curation, deep international landscape research, and surgical logistics management. Because we are not beholden to commission structures, our loyalty belongs 100% to you. We filter out the noise to hand-select independent boutique stays, hyper-local eco-lodges, and off-the-beaten-path experiences that match your exact comfort level, physical agility, and dietary needs. We save you dozens of hours of frustrating guesswork, giving you complete spatial confidence before you fly.
                        </div>
                    </div>
                </div>

                <!-- FAQ Item 3 -->
                <div class="group py-4">
                    <button class="w-full text-left py-4 font-semibold text-sm md:text-base text-[#3D4035] flex justify-between items-center focus:outline-none select-none transition-colors" onclick="toggleFAQ(3)">
                        <span class="flex items-center gap-4">
                            <span class="text-xs font-serif italic text-[#8C7A6B]/50 font-normal tracking-wide">03</span>
                            <span>Since you are a design-only planner, how do my hotels and excursions actually get booked?</span>
                        </span>
                        <svg id="icon-3" class="w-4 h-4 text-[#8C7A6B] transform transition-transform duration-300" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" d="M19 9l-7 7-7-7"></path>
                        </svg>
                    </button>
                    <div id="faq-3" class="max-h-0 overflow-hidden opacity-0 transition-all duration-500 ease-in-out">
                        <div class="pb-6 pl-8 text-xs md:text-sm text-stone-600 leading-relaxed pt-2">
                            We design the blueprint; you lock in the reservations. Once your final custom itinerary or research dossier is completed, you will receive a beautifully formatted, comprehensive digital document. For all recommended accommodations, trains, private transfers, and curated excursions, we provide direct, vetted reservation links. All you have to do is click and input your payment details. This transparent method ensures that you maintain absolute control over your loyalty points, personal credit card data, and cancellation policies, with zero hidden markups or third-party booking fees.
                        </div>
                    </div>
                </div>

                <!-- FAQ Item 4 -->
                <div class="group py-4">
                    <button class="w-full text-left py-4 font-semibold text-sm md:text-base text-[#3D4035] flex justify-between items-center focus:outline-none select-none transition-colors" onclick="toggleFAQ(4)">
                        <span class="flex items-center gap-4">
                            <span class="text-xs font-serif italic text-[#8C7A6B]/50 font-normal tracking-wide">04</span>
                            <span>What happens if my flight gets delayed or a hotel cancellation happens while I am on my trip?</span>
                        </span>
                        <svg id="icon-4" class="w-4 h-4 text-[#8C7A6B] transform transition-transform duration-300" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" d="M19 9l-7 7-7-7"></path>
                        </svg>
                    </button>
                    <div id="faq-4" class="max-h-0 overflow-hidden opacity-0 transition-all duration-500 ease-in-out">
                        <div class="pb-6 pl-8 text-xs md:text-sm text-stone-600 leading-relaxed pt-2">
                            Because we are a design, curation, and intelligence service rather than a transactional booking agency, the legal contracts for your reservations exist directly between you and the vendors you choose to book (the airlines, boutique hotels, or local tour operators). While we do not provide 24/7 on-trip crisis management or re-booking services, your custom blueprint is intentionally designed to mitigate these risks. We build robust time tolerances into your transit networks, provide clear alternative routes, and supply emergency local contact protocols right inside your dossier so you can smoothly navigate unexpected travel anomalies with complete independence. We highly recommend securing comprehensive travel insurance for every international journey.
                        </div>
                    </div>
                </div>

                <!-- FAQ Item 5 -->
                <div class="group py-4">
                    <button class="w-full text-left py-4 font-semibold text-sm md:text-base text-[#3D4035] flex justify-between items-center focus:outline-none select-none transition-colors" onclick="toggleFAQ(5)">
                        <span class="flex items-center gap-4">
                            <span class="text-xs font-serif italic text-[#8C7A6B]/50 font-normal tracking-wide">05</span>
                            <span>I have severe food allergies / strict dietary boundaries. Can your curated recommendations accommodate me safely?</span>
                        </span>
                        <svg id="icon-5" class="w-4 h-4 text-[#8C7A6B] transform transition-transform duration-300" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" d="M19 9l-7 7-7-7"></path>
                        </svg>
                    </button>
                    <div id="faq-5" class="max-h-0 overflow-hidden opacity-0 transition-all duration-500 ease-in-out">
                        <div class="pb-6 pl-8 text-xs md:text-sm text-stone-600 leading-relaxed pt-2">
                            Absolutely. In fact, this is one of our primary specialties. Cross-referencing safe dining in unfamiliar countries can be incredibly stressful. When building your custom itinerary or research dossier, we don't just pull arbitrary restaurant reviews. We deeply analyze your dietary profile—whether you are strictly vegan, managing celiac disease, or navigating severe food allergies. We curate dedicated dining blueprints and, for our Tier 3 flagship clients, we explicitly verify the physical kitchen frameworks and kitchenette capabilities of our recommended lodging to ensure your safety and comfort are fully integrated into the architecture of your trip.
                        </div>
                    </div>
                </div>

                <!-- FAQ Item 6 -->
                <div class="group py-4">
                    <button class="w-full text-left py-4 font-semibold text-sm md:text-base text-[#3D4035] flex justify-between items-center focus:outline-none select-none transition-colors" onclick="toggleFAQ(6)">
                        <span class="flex items-center gap-4">
                            <span class="text-xs font-serif italic text-[#8C7A6B]/50 font-normal tracking-wide">06</span>
                            <span>Can I request revisions if the initial blueprint pace doesn't feel quite right?</span>
                        </span>
                        <svg id="icon-6" class="w-4 h-4 text-[#8C7A6B] transform transition-transform duration-300" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" d="M19 9l-7 7-7-7"></path>
                        </svg>
                    </button>
                    <div id="faq-6" class="max-h-0 overflow-hidden opacity-0 transition-all duration-500 ease-in-out">
                        <div class="pb-6 pl-8 text-xs md:text-sm text-stone-600 leading-relaxed pt-2">
                            Yes, collaboration is a vital part of the artistic design process. For our Tier 3 Custom Trip Retainer, your investment includes up to two complete rounds of revisions. After receiving your initial draft blueprint, we will review the pacing, accommodation styles, and daily flow together, fine-tuning the elements until it perfectly mirrors your ideal travel energy. For our Tier 1 and Tier 2 services, our comprehensive intake form is designed to capture your exact parameters upfront so your finalized dossier hits the mark right out of the gate.
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <hr class="border-stone-200/60 my-16">

        <!-- Section 5: The Full Master Discovery Questionnaire Form -->
        <section id="discover" class="bg-white/75 backdrop-blur-md border border-stone-200/60 rounded-3xl p-6 md:p-10 shadow-sm max-w-2xl mx-auto mb-16">
            <div class="text-center mb-8">
                <span class="text-xs tracking-[0.2em] text-[#8C7A6B] uppercase font-bold">Client Intake Matrix</span>
                <h3 class="text-2xl md:text-3xl font-medium text-[#3D4035] mt-1">Master Discovery Questionnaire</h3>
                <p class="text-xs text-stone-500 mt-2">Please outline your operational parameters below to anchor your curated asset architecture.</p>
            </div>

            <form action="https://api.web3forms.com/submit" method="POST" id="discover-form" class="space-y-8 text-sm text-stone-700">
                <!-- Web3Forms Security Tokens -->
                <input type="hidden" name="access_key" value="YOUR_ACCESS_KEY_HERE">
                <input type="hidden" name="subject" value="Master Intake Profile - The Conscious Compass">
                <input type="hidden" name="from_name" value="The Conscious Compass Portal">
                <input type="hidden" name="redirect" value="">

                <!-- SECTION 1: THE FOUNDATION -->
                <div class="space-y-5 border-b border-stone-200/50 pb-8">
                    <h4 class="font-serif font-semibold text-lg text-[#3D4035] flex items-center gap-2">
                        <span class="text-xs font-sans font-bold bg-[#8C7A6B]/15 text-[#8C7A6B] w-5 h-5 rounded-full inline-flex items-center justify-center">1</span> 
                        The Foundation
                    </h4>
                    
                    <!-- Q1: Contact Details -->
                    <div class="grid grid-cols-1 md:grid-cols-3 gap-4">
                        <div>
                            <label class="block text-[11px] font-semibold tracking-wider text-stone-500 uppercase mb-1">Full Name</label>
                            <input type="text" name="client_name" required class="w-full px-4 py-2.5 rounded-xl border border-stone-200 focus:border-[#8C7A6B] focus:ring-1 focus:ring-[#8C7A6B] outline-none bg-stone-50/40 transition">
                        </div>
                        <div>
                            <label class="block text-[11px] font-semibold tracking-wider text-stone-500 uppercase mb-1">Email Address</label>
                            <input type="email" name="email" required class="w-full px-4 py-2.5 rounded-xl border border-stone-200 focus:border-[#8C7A6B] focus:ring-1 focus:ring-[#8C7A6B] outline-none bg-stone-50/40 transition">
                        </div>
                        <div>
                            <label class="block text-[11px] font-semibold tracking-wider text-stone-500 uppercase mb-1">Phone Number</label>
                            <input type="tel" name="client_phone" required class="w-full px-4 py-2.5 rounded-xl border border-stone-200 focus:border-[#8C7A6B] focus:ring-1 focus:ring-[#8C7A6B] outline-none bg-stone-50/40 transition">
                        </div>
                    </div>

                    <!-- Q2: Party Dynamics -->
                    <div class="space-y-2">
                        <label class="block text-[11px] font-semibold tracking-wider text-stone-500 uppercase">Who will be embarking on this journey?</label>
                        <div class="grid grid-cols-1 md:grid-cols-2 gap-2.5 pt-1">
                            <label class="flex items-center gap-3 p-3 bg-stone-50/40 border border-stone-200/60 rounded-xl cursor-pointer hover:bg-stone-50/80 transition select-none">
                                <input type="radio" name="party_dynamics" value="solo" checked class="accent-[#8C7A6B]">
                                <span>Just me (Solo traveler)</span>
                            </label>
                            <label class="flex items-center gap-3 p-3 bg-stone-50/40 border border-stone-200/60 rounded-xl cursor-pointer hover:bg-stone-50/80 transition select-none">
                                <input type="radio" name="party_dynamics" value="partner" class="accent-[#8C7A6B]">
                                <span>Me and a partner/spouse</span>
                            </label>
                            <label class="flex items-center gap-3 p-3 bg-stone-50/40 border border-stone-200/60 rounded-xl cursor-pointer hover:bg-stone-50/80 transition select-none">
                                <input type="radio" name="party_dynamics" value="family" id="party-family-trigger" class="accent-[#8C7A6B]">
                                <span>A family trip</span>
                            </label>
                            <label class="flex items-center gap-3 p-3 bg-stone-50/40 border border-stone-200/60 rounded-xl cursor-pointer hover:bg-stone-50/80 transition select-none">
                                <input type="radio" name="party_dynamics" value="group" class="accent-[#8C7A6B]">
                                <span>A group of friends or extended family</span>
                            </label>
                        </div>
                    </div>

                    <!-- Conditional Dynamic Field: Family Child Ages -->
                    <div id="family-ages-wrapper" class="hidden bg-stone-50/80 border border-stone-200/60 rounded-xl p-4 transition-all duration-300 transform">
                        <label class="block text-[11px] font-semibold tracking-wider text-[#8C7A6B] uppercase mb-1">Please list the ages of any children traveling:</label>
                        <input type="text" name="family_child_ages" placeholder="e.g., 4, 8" class="w-full px-4 py-2.5 rounded-xl border border-stone-200 focus:border-[#8C7A6B] focus:ring-1 focus:ring-[#8C7A6B] outline-none bg-white transition">
                    </div>

                    <!-- Q3: Service Selection Framework -->
                    <div class="space-y-2 pt-2">
                        <label class="block text-[11px] font-semibold tracking-wider text-stone-500 uppercase">Which portfolio segment are we securing?</label>
                        <div class="space-y-2.5 pt-1">
                            <span class="block text-[10px] font-bold tracking-widest uppercase text-stone-400 mt-2">— Travel Architecture Frameworks</span>
                            <label class="flex items-start gap-3 p-3 bg-white border border-stone-200 rounded-xl cursor-pointer hover:border-stone-300 transition select-none">
                                <input type="radio" name="service_framework" value="tier_1" checked class="accent-[#8C7A6B] mt-1 framework-type-trigger">
                                <div class="text-xs"><strong class="text-stone-800 font-semibold block text-sm">Tier 1: The Deep-Dive Research Blueprint ($175)</strong> For independent travelers who handle bookings but want expert analysis on logistics, safety, and entry constraints.</div>
                            </label>
                            <label class="flex items-start gap-3 p-3 bg-white border border-stone-200 rounded-xl cursor-pointer hover:border-stone-300 transition select-none">
                                <input type="radio" name="service_framework" value="tier_2" class="accent-[#8C7A6B] mt-1 framework-type-trigger">
                                <div class="text-xs"><strong class="text-stone-800 font-semibold block text-sm">Tier 2: The "Day-Hacker" Partial Itinerary ($75/day)</strong> For those who have the framework set but require hourly custom curation for specific multi-day stretches.</div>
                            </label>
                            <label class="flex items-start gap-3 p-3 bg-white border border-stone-200 rounded-xl cursor-pointer hover:border-stone-300 transition select-none">
                                <input type="radio" name="service_framework" value="tier_3" class="accent-[#8C7A6B] mt-1 framework-type-trigger">
                                <div class="text-xs"><strong class="text-stone-800 font-semibold block text-sm">Tier 3: The All-Inclusive Custom Trip Retainer ($450+)</strong> Our flagship end-to-end design covering lodging shortlists, pacing, maps, and absolute workflow coordination.</div>
                            </label>
                            
                            <span class="block text-[10px] font-bold tracking-widest uppercase text-stone-400 mt-4 block">— Fine Art Portfolio Add-Ons Only</span>
                            <label class="flex items-start gap-3 p-3 bg-white border-2 border-[#8C7A6B]/30 rounded-xl cursor-pointer bg-stone-50/10 transition select-none">
                                <input type="radio" name="service_framework" value="art_commission" class="accent-[#8C7A6B] mt-1 framework-type-trigger">
                                <div class="text-xs"><strong class="text-stone-800 font-semibold block text-sm text-[#8C7A6B]">Bespoke Fine Art Travel Commission (A4 - $65+)</strong> Request an original watercolor or acrylic landscape piece capturing a dedicated travel memory space (completely bypasses travel planning forms).</div>
                            </label>
                            <label class="flex items-start gap-3 p-3 bg-white border border-stone-200 rounded-xl cursor-pointer hover:border-stone-300 transition select-none">
                                <input type="radio" name="service_framework" value="art_print" class="accent-[#8C7A6B] mt-1 framework-type-trigger">
                                <div class="text-xs"><strong class="text-stone-800 font-semibold block text-sm text-stone-700">Standalone Portfolio Watercolor Travel Print (8x10 - $35.00)</strong> Order a standard 8x10 fine art print production of a landscape featured in our gallery tracks.</div>
                            </label>
                        </div>
                    </div>
                </div>

                <!-- TRAVEL INTERFACE SECTION: DESTINATION, ENERGY, & CULINARY STYLE -->
                <div id="travel-core-fields" class="space-y-5 border-b border-stone-200/50 pb-8">
                    <h4 class="font-serif font-semibold text-lg text-[#3D4035] flex items-center gap-2">
                        <span class="text-xs font-sans font-bold bg-[#8C7A6B]/15 text-[#8C7A6B] w-5 h-5 rounded-full inline-flex items-center justify-center">2</span> 
                        Destination, Energy, & Sensory Profile
                    </h4>

                    <!-- Q4: Core Parameters -->
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                        <div>
                            <label class="block text-[11px] font-semibold tracking-wider text-stone-500 uppercase mb-1">Where are you exploring? (Destinations / Ideas)</label>
                            <input type="text" name="target_destination" placeholder="e.g., Costa Rica Rainforest, Colombia Highland Canopy" class="w-full px-4 py-2.5 rounded-xl border border-stone-200 focus:border-[#8C7A6B] focus:ring-1 focus:ring-[#8C7A6B] outline-none bg-stone-50/40 transition">
                        </div>
                        <div>
                            <label class="block text-[11px] font-semibold tracking-wider text-stone-500 uppercase mb-1">Estimated Travel Dates / Window</label>
                            <input type="text" name="travel_dates_window" placeholder="e.g., Mid-October, Late August" class="w-full px-4 py-2.5 rounded-xl border border-stone-200 focus:border-[#8C7A6B] focus:ring-1 focus:ring-[#8C7A6B] outline-none bg-stone-50/40 transition">
                        </div>
                    </div>

                    <!-- Q5: Trip Energy -->
                    <div class="space-y-2">
                        <label class="block text-[11px] font-semibold tracking-wider text-stone-500 uppercase">Primary Trip Energy Focus (Select up to 2)</label>
                        <div class="grid grid-cols-1 md:grid-cols-2 gap-2.5 pt-1">
                            <label class="flex items-center gap-3 p-3 bg-white border border-stone-200 rounded-xl cursor-pointer hover:bg-stone-50/30 transition select-none">
                                <input type="checkbox" name="trip_energy[]" value="culture" class="rounded accent-[#8C7A6B]">
                                <span>Deep immersion into local culture, arts, & history</span>
                            </label>
                            <label class="flex items-center gap-3 p-3 bg-white border border-stone-200 rounded-xl cursor-pointer hover:bg-stone-50/30 transition select-none">
                                <input type="checkbox" name="trip_energy[]" value="active" id="energy-active-trigger" class="rounded accent-[#8C7A6B]">
                                <span class="font-medium text-stone-800">Active exploration, hiking, & variable terrains</span>
                            </label>
                            <label class="flex items-center gap-3 p-3 bg-white border border-stone-200 rounded-xl cursor-pointer hover:bg-stone-50/30 transition select-none">
                                <input type="checkbox" name="trip_energy[]" value="relaxation" class="rounded accent-[#8C7A6B]">
                                <span>Unplugged relaxation, nature, & slow wandering</span>
                            </label>
                            <label class="flex items-center gap-3 p-3 bg-white border border-stone-200 rounded-xl cursor-pointer hover:bg-stone-50/30 transition select-none">
                                <input type="checkbox" name="trip_energy[]" value="culinary" class="rounded accent-[#8C7A6B]">
                                <span>Culinary journeys, local markets, & food scenes</span>
                            </label>
                            <label class="flex items-center gap-3 p-3 bg-white border border-stone-200 rounded-xl cursor-pointer hover:bg-stone-50/30 transition select-none">
                                <input type="checkbox" name="trip_energy[]" value="sustainable" class="rounded accent-[#8C7A6B]">
                                <span>Eco-conscious, sustainable, & wildlife travel</span>
                            </label>
                        </div>
                    </div>

                    <!-- Conditional Dynamic Field: Q6 Agility (Triggered by 'Active Exploration') -->
                    <div id="agility-fields-wrapper" class="hidden bg-stone-50/80 border border-stone-200/60 rounded-2xl p-4 md:p-5 transition-all duration-300 transform">
                        <label class="block text-[11px] font-semibold tracking-wider text-[#8C7A6B] uppercase mb-2">Q6: Physical Agility & Terrain Comfort</label>
                        <div class="space-y-2 text-xs">
                            <label class="flex items-start gap-3 p-2.5 bg-white border border-stone-100 rounded-xl cursor-pointer">
                                <input type="radio" name="physical_agility" value="scenic" checked class="accent-[#8C7A6B] mt-0.5">
                                <span><strong class="text-stone-800 block">The Scenic Soles (Leisurely):</strong> We love nature but require flat, well-maintained paths, boardwalks, and brief trail lengths (under 2 miles) with marginal inclines.</span>
                            </label>
                            <label class="flex items-start gap-3 p-2.5 bg-white border border-stone-100 rounded-xl cursor-pointer">
                                <input type="radio" name="physical_agility" value="steady" class="accent-[#8C7A6B] mt-0.5">
                                <span><strong class="text-stone-800 block">The Steady Trekkers (Moderate):</strong> We handle unpaved paths, uneven footings, and moderate vertical shifts. Routinely enjoy 3–5 mile day journeys.</span>
                            </label>
                            <label class="flex items-start gap-3 p-2.5 bg-white border border-stone-100 rounded-xl cursor-pointer">
                                <input type="radio" name="physical_agility" value="summit" class="accent-[#8C7A6B] mt-0.5">
                                <span><strong class="text-stone-800 block">The Summit Seekers (Advanced):</strong> Bring on steep vertical profiles, scrambles, higher altitudes, or technical water crossings (6+ miles).</span>
                            </label>
                            <label class="flex items-start gap-3 p-2.5 bg-white border border-stone-100 rounded-xl cursor-pointer">
                                <input type="radio" name="physical_agility" value="accessible" class="accent-[#8C7A6B] mt-0.5">
                                <span><strong class="text-stone-800 block">Mobility-Conscious / Accessible Needs:</strong> We strictly require terrain that is paved, flat, or fully optimized for strollers, wheels, or specific physical accommodations.</span>
                            </label>
                        </div>
                    </div>

                    <!-- Q7: Culinary Style -->
                    <div class="space-y-2">
                        <label class="block text-[11px] font-semibold tracking-wider text-stone-500 uppercase">Q7: Culinary Adventurousness & Profile</label>
                        <div class="grid grid-cols-1 md:grid-cols-2 gap-2.5 text-xs">
                            <label class="flex items-start gap-3 p-3 bg-white border border-stone-200 rounded-xl cursor-pointer">
                                <input type="radio" name="culinary_profile" value="safe" checked class="accent-[#8C7A6B] mt-0.5">
                                <span><strong class="text-stone-800 block">The Play-It-Safe Diner:</strong> Familiar profiles, highly rated standard venues, and predictable dining blocks.</span>
                            </label>
                            <label class="flex items-start gap-3 p-3 bg-white border border-stone-200 rounded-xl cursor-pointer">
                                <input type="radio" name="culinary_profile" value="curious" class="accent-[#8C7A6B] mt-0.5">
                                <span><strong class="text-stone-800 block">The Curious Casual:</strong> Open to signature regional dishes inside comfortable, accessible sit-down environments.</span>
                            </label>
                            <label class="flex items-start gap-3 p-3 bg-white border border-stone-200 rounded-xl cursor-pointer">
                                <input type="radio" name="culinary_profile" value="explorer" class="accent-[#8C7A6B] mt-0.5">
                                <span><strong class="text-stone-800 block">The Culinary Explorer:</strong> Lead me to street stalls, night networks, and hidden alleys. I thrive on regional ingredients.</span>
                            </label>
                            <label class="flex items-start gap-3 p-3 bg-white border border-stone-200 rounded-xl cursor-pointer">
                                <input type="radio" name="culinary_profile" value="fine_diner" class="accent-[#8C7A6B] mt-0.5">
                                <span><strong class="text-stone-800 block">The Fine Diner:</strong> Tasting menus, Michelin citations, and structured high-end gastronomic environments.</span>
                            </label>
                        </div>
                    </div>

                    <!-- Q8: Structural Comfort Zone -->
                    <div class="space-y-2">
                        <label class="block text-[11px] font-semibold tracking-wider text-stone-500 uppercase">Q8: Environmental & Structural Comfort Zone</label>
                        <div class="space-y-2 text-xs">
                            <label class="flex items-center gap-3 p-3 bg-white border border-stone-200 rounded-xl cursor-pointer">
                                <input type="radio" name="structural_comfort" value="seamless" checked class="accent-[#8C7A6B]">
                                <span>Seamless & Comfortable — Pre-arranged private transfers, boutique lodging, and verified infrastructure.</span>
                            </label>
                            <label class="flex items-center gap-3 p-3 bg-white border border-stone-200 rounded-xl cursor-pointer">
                                <input type="radio" name="structural_comfort" value="adventure" class="accent-[#8C7A6B]">
                                <span>I love an adventure — Fully comfortable navigating regional trains, public networks, and organic topographies.</span>
                            </label>
                            <label class="flex items-center gap-3 p-3 bg-white border border-stone-200 rounded-xl cursor-pointer">
                                <input type="radio" name="structural_comfort" value="mixed" class="accent-[#8C7A6B]">
                                <span>A beautiful mix — Secure boutique base camps for rest, but entirely exploratory and raw during day intervals.</span>
                            </label>
                        </div>
                    </div>
                </div>

                <!-- SECTION 3: TARGETED DEEP-DIVES (BRANCHING CONTAINER) -->
                <div class="pb-2">
                    
                    <!-- TIER 1 DYNAMIC FIELDS -->
                    <div id="tier-1-fields" class="space-y-5 border-b border-stone-200/50 pb-8 dynamic-tier-section">
                        <h4 class="font-serif font-semibold text-lg text-[#4E5142] flex items-center gap-2">
                            <span class="text-xs font-sans font-bold bg-[#4E5142]/15 text-[#4E5142] w-5 h-5 rounded-full inline-flex items-center justify-center">3</span> 
                            Tier 1: Deep-Dive Research Scope
                        </h4>
                        <div class="space-y-2">
                            <label class="block text-[11px] font-semibold tracking-wider text-stone-500 uppercase">Q9: What are the top 3 friction points keeping you up at night?</label>
                            <div class="space-y-2 text-xs pt-1">
                                <label class="flex items-center gap-3 p-2.5 bg-white border border-stone-200 rounded-xl cursor-pointer">
                                    <input type="checkbox" name="t1_friction[]" value="transit" class="rounded accent-[#4E5142]">
                                    <span>Navigating the local public transit, train networks, or regional ferries</span>
                                </label>
                                <label class="flex items-center gap-3 p-2.5 bg-white border border-stone-200 rounded-xl cursor-pointer">
                                    <input type="checkbox" name="t1_friction[]" value="bureaucracy" class="rounded accent-[#4E5142]">
                                    <span>Visas, passport validity, complex entry requirements, or health protocols</span>
                                </label>
                                <label class="flex items-center gap-3 p-2.5 bg-white border border-stone-200 rounded-xl cursor-pointer">
                                    <input type="checkbox" name="t1_friction[]" value="safety" class="rounded accent-[#4E5142]">
                                    <span>Neighborhood safety, local scams, and solo travel security</span>
                                </label>
                                <label class="flex items-center gap-3 p-2.5 bg-white border border-stone-200 rounded-xl cursor-pointer">
                                    <input type="checkbox" name="t1_friction[]" value="packing" class="rounded accent-[#4E5142]">
                                    <span>Packing correctly for complex climates, varying topographies, or cultural dress codes</span>
                                </label>
                                <label class="flex items-center gap-3 p-2.5 bg-white border border-stone-200 rounded-xl cursor-pointer">
                                    <input type="checkbox" name="t1_friction[]" value="eco_operators" class="rounded accent-[#4E5142]">
                                    <span>Identifying verified sustainable, eco-conscious tour operators or local guides</span>
                                </label>
                            </div>
                        </div>
                        <div>
                            <label class="block text-[11px] font-semibold tracking-wider text-stone-500 uppercase mb-1">Q10: Tell us more about the specific anxieties or unique excitements you have for this location.</label>
                            <textarea name="t1_anxieties_narrative" rows="4" placeholder="e.g., 'I want a clear breakdown of how to purchase train segments online vs locally,'..." class="w-full px-4 py-3 rounded-xl border border-stone-200 focus:border-[#4E5142] focus:ring-1 focus:ring-[#4E5142] outline-none bg-stone-50/40 transition"></textarea>
                        </div>
                    </div>

                    <!-- TIER 2 DYNAMIC FIELDS -->
                    <div id="tier-2-fields" class="hidden space-y-5 border-b border-stone-200/50 pb-8 dynamic-tier-section">
                        <h4 class="font-serif font-semibold text-lg text-[#4E5142] flex items-center gap-2">
                            <span class="text-xs font-sans font-bold bg-[#4E5142]/15 text-[#4E5142] w-5 h-5 rounded-full inline-flex items-center justify-center">3</span> 
                            Tier 2: The "Day-Hacker" Details
                        </h4>
                        <div class="grid grid-cols-1 md:grid-cols-3 gap-4">
                            <div class="md:col-span-1">
                                <label class="block text-[11px] font-semibold tracking-wider text-stone-500 uppercase mb-1">Q11: Active Days Required (Min. 2)</label>
                                <input type="number" name="t2_planned_days" min="2" placeholder="3" class="w-full px-4 py-2.5 rounded-xl border border-stone-200 focus:border-[#4E5142] focus:ring-1 focus:ring-[#4E5142] outline-none bg-stone-50/40 transition">
                            </div>
                            <div class="md:col-span-2">
                                <label class="block text-[11px] font-semibold tracking-wider text-stone-500 uppercase mb-1">Q12: Specific Dates / Segments for Us to Design</label>
                                <input type="text" name="t2_segments_description" placeholder="e.g., Days 3, 4, & 5 while in the cloud forest province" class="w-full px-4 py-2.5 rounded-xl border border-stone-200 focus:border-[#4E5142] focus:ring-1 focus:ring-[#4E5142] outline-none bg-stone-50/40 transition">
                            </div>
                        </div>
                        <div>
                            <label class="block text-[11px] font-semibold tracking-wider text-stone-500 uppercase mb-1">Q13: Fixed Bookings Already Secured for These Days</label>
                            <textarea name="t2_fixed_assets" rows="3" placeholder="List existing lodging names, transit assets..." class="w-full px-4 py-3 rounded-xl border border-stone-200 focus:border-[#4E5142] focus:ring-1 focus:ring-[#4E5142] outline-none bg-stone-50/40 transition"></textarea>
                        </div>
                        <div>
                            <label class="block text-[11px] font-semibold tracking-wider text-stone-500 uppercase mb-1">Q14: Specific Dietary Boundaries or Severe Allergies for Dining Links</label>
                            <textarea name="t2_dietary_needs" rows="3" placeholder="State explicit constraints, cross-contamination concerns, or type 'None'..." class="w-full px-4 py-3 rounded-xl border border-stone-200 focus:border-[#4E5142] focus:ring-1 focus:ring-[#4E5142] outline-none bg-stone-50/40 transition"></textarea>
                        </div>
                    </div>

                    <!-- TIER 3 DYNAMIC FIELDS -->
                    <div id="tier-3-fields" class="hidden space-y-5 border-b border-stone-200/50 pb-8 dynamic-tier-section">
                        <h4 class="font-serif font-semibold text-lg text-[#4E5142] flex items-center gap-2">
                            <span class="text-xs font-sans font-bold bg-[#4E5142]/15 text-[#4E5142] w-5 h-5 rounded-full inline-flex items-center justify-center">3</span> 
                            Tier 3: Flagship Custom Retainer Masterclass
                        </h4>
                        <div class="space-y-2">
                            <label class="block text-[11px] font-semibold tracking-wider text-stone-500 uppercase">Q15: Expected Travel Investment (Excluding Design Retainer)</label>
                            <div class="grid grid-cols-2 md:grid-cols-4 gap-2 text-xs">
                                <label class="flex items-center gap-2 p-2.5 bg-white border border-stone-200 rounded-xl cursor-pointer"><input type="radio" name="t3_budget" value="3k-5k" checked class="accent-[#4E5142]"> <span>$3,000–$5,000</span></label>
                                <label class="flex items-center gap-2 p-2.5 bg-white border border-stone-200 rounded-xl cursor-pointer"><input type="radio" name="t3_budget" value="5k-10k" class="accent-[#4E5142]"> <span>$5,000–$10,000</span></label>
                                <label class="flex items-center gap-2 p-2.5 bg-white border border-stone-200 rounded-xl cursor-pointer"><input type="radio" name="t3_budget" value="10k-15k" class="accent-[#4E5142]"> <span>$10,000–$15,000</span></label>
                                <label class="flex items-center gap-2 p-2.5 bg-white border border-stone-200 rounded-xl cursor-pointer"><input type="radio" name="t3_budget" value="15k+" class="accent-[#4E5142]"> <span>$15,000+</span></label>
                            </div>
                        </div>
                        <div class="space-y-2">
                            <label class="block text-[11px] font-semibold tracking-wider text-stone-500 uppercase">Q16: Travel Pacing Preference</label>
                            <div class="space-y-2 text-xs">
                                <label class="flex items-center gap-3 p-2.5 bg-white border border-stone-200 rounded-xl cursor-pointer"><input type="radio" name="t3_pacing" value="slow" checked class="accent-[#4E5142]"> <span><strong class="text-stone-800 font-semibold">Slow & Immersive:</strong> Unpack once, anchor in fewer locations.</span></label>
                                <label class="flex items-center gap-3 p-2.5 bg-white border border-stone-200 rounded-xl cursor-pointer"><input type="radio" name="t3_pacing" value="balanced" class="accent-[#4E5142]"> <span><strong class="text-stone-800 font-semibold">Balanced:</strong> Organic morning activities matched with unprogrammed afternoons.</span></label>
                                <label class="flex items-center gap-3 p-2.5 bg-white border border-stone-200 rounded-xl cursor-pointer"><input type="radio" name="t3_pacing" value="dynamic" class="accent-[#4E5142]"> <span><strong class="text-stone-800 font-semibold">Dynamic Explorer:</strong> Shifting bases every 2–3 days to explore maximum ground.</span></label>
                            </div>
                        </div>
                        <div class="space-y-2">
                            <label class="block text-[11px] font-semibold tracking-wider text-stone-500 uppercase">Q17: Dietary Accommodations & Restrictions (Select all that apply)</label>
                            <div class="grid grid-cols-2 md:grid-cols-3 gap-2.5 text-xs">
                                <label class="flex items-center gap-2 p-2 bg-white border border-stone-100 rounded-lg"><input type="checkbox" name="t3_diet[]" value="none" class="rounded accent-[#4E5142]"> <span>None / Unrestricted</span></label>
                                <label class="flex items-center gap-2 p-2 bg-white border border-stone-100 rounded-lg"><input type="checkbox" name="t3_diet[]" value="vegetarian" class="rounded accent-[#4E5142]"> <span>Vegetarian</span></label>
                                <label class="flex items-center gap-2 p-2 bg-white border border-stone-100 rounded-lg"><input type="checkbox" name="t3_diet[]" value="vegan" class="rounded accent-[#4E5142]"> <span class="font-semibold text-emerald-700">Vegan</span></label>
                                <label class="flex items-center gap-2 p-2 bg-white border border-stone-100 rounded-lg"><input type="checkbox" name="t3_diet[]" value="gluten_free" class="rounded accent-[#4E5142]"> <span class="font-semibold text-amber-700">Gluten-Free / Celiac</span></label>
                                <label class="flex items-center gap-2 p-2 bg-white border border-stone-100 rounded-lg"><input type="checkbox" name="t3_diet[]" value="dairy_free" class="rounded accent-[#4E5142]"> <span>Dairy-Free</span></label>
                            </div>
                            <div class="grid grid-cols-1 md:grid-cols-2 gap-3 pt-1 text-xs">
                                <input type="text" name="t3_allergies_spec" placeholder="Specify severe food allergies here..." class="px-3 py-2 border border-stone-200 rounded-xl bg-white outline-none focus:border-[#4E5142]">
                                <input type="text" name="t3_religious_spec" placeholder="Specify religious constraints (Halal, Kosher)..." class="px-3 py-2 border border-stone-200 rounded-xl bg-white outline-none focus:border-[#4E5142]">
                            </div>
                        </div>
                        <div class="space-y-2">
                            <label class="block text-[11px] font-semibold tracking-wider text-stone-500 uppercase">Q18: Critical Accommodation Infrastructure</label>
                            <div class="space-y-2 text-xs">
                                <label class="flex items-center gap-3 p-2.5 bg-white border border-stone-200 rounded-xl cursor-pointer"><input type="radio" name="t3_infrastructure" value="restaurants" checked class="accent-[#4E5142]"> <span>Only impacts standalone dining curation—lodging selections just require standard allergy notifications.</span></label>
                                <label class="flex items-center gap-3 p-2.5 bg-white border border-stone-200 rounded-xl cursor-pointer"><input type="radio" name="t3_infrastructure" value="kitchenette" class="accent-[#4E5142]"><span class="font-medium text-stone-800">Highly critical — We require boutique lodging verified with cross-contamination tracking or isolated private kitchenettes.</span></label>
                            </div>
                        </div>
                        <div>
                            <label class="block text-[11px] font-semibold tracking-wider text-stone-500 uppercase mb-1">Q19: Core Deal-Breakers & Must-Haves</label>
                            <textarea name="t3_dealbreakers" rows="3" placeholder="e.g., 'Lodging must hold local eco-certified protocols,' 'No localized prop planes,' 'Must locate a textile workshop'..." class="w-full px-4 py-3 rounded-xl border border-stone-200 focus:border-[#4E5142] focus:ring-1 focus:ring-[#4E5142] outline-none bg-stone-50/40 transition"></textarea>
                        </div>
                    </div>

                    <!-- NEW DYNAMIC CONTAINER: FINE ART ONLY SPECS -->
                    <div id="art-only-fields" class="hidden space-y-5 border-b border-stone-200/50 pb-8 dynamic-tier-section">
                        <h4 class="font-serif font-semibold text-lg text-[#8C7A6B] flex items-center gap-2">
                            <span class="text-xs font-sans font-bold bg-[#8C7A6B]/15 text-[#8C7A6B] w-5 h-5 rounded-full inline-flex items-center justify-center">2</span> 
                            Fine Art Order & Commission Specifications
                        </h4>
                        
                        <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                            <div>
                                <label class="block text-[11px] font-semibold tracking-wider text-stone-500 uppercase mb-1">Select Asset Style / Type</label>
                                <select name="art_product_medium" class="w-full px-4 py-2.5 rounded-xl border border-stone-200 focus:border-[#8C7A6B] focus:ring-1 focus:ring-[#8C7A6B] outline-none bg-white text-xs transition">
                                    <option value="watercolor_commission_a4">Bespoke Original Watercolor Commission (Size A4 — $65.00)</option>
                                    <option value="acrylic_commission_a4">Bespoke Original Acrylic Commission (Size A4 — $90.00)</option>
                                    <option value="standalone_print_8x10">Standalone Portfolio Landscape Print (Size 8x10 — $35.00)</option>
                                </select>
                            </div>
                            <div>
                                <label class="block text-[11px] font-semibold tracking-wider text-stone-500 uppercase mb-1">Target Print Title or Reference Scene</label>
                                <input type="text" name="art_target_subject" placeholder="e.g., 'Misty Basin Canoe Sketch' or 'Custom Landscape Memory'" class="w-full px-4 py-2.5 rounded-xl border border-stone-200 focus:border-[#8C7A6B] focus:ring-1 focus:ring-[#8C7A6B] outline-none bg-white text-xs transition">
                            </div>
                        </div>

                        <div>
                            <label class="block text-[11px] font-semibold tracking-wider text-stone-500 uppercase mb-1">Visual Memory Summary or Custom Sketch Parameters</label>
                            <textarea name="art_creative_details" rows="4" placeholder="For Commissions: Summarize the environmental landscape, colors, or visual textures you want framed. (Reminder: I focus strictly on environment-first scenes; no portraits or facial details). For Prints: Add any shipping instructions..." class="w-full px-4 py-3 rounded-xl border border-stone-200 focus:border-[#8C7A6B] focus:ring-1 focus:ring-[#8C7A6B] outline-none bg-stone-50/40 transition"></textarea>
                        </div>
                    </div>

                </div>

                <!-- SECTION 4: FINAL SUBMISSION & BOUNDARIES -->
                <div class="space-y-5 pt-2">
                    <h4 class="font-serif font-semibold text-lg text-[#3D4035] flex items-center gap-2">
                        <span id="final-section-num" class="text-xs font-sans font-bold bg-[#8C7A6B]/15 text-[#8C7A6B] w-5 h-5 rounded-full inline-flex items-center justify-center">4</span> 
                        Final Submission & Framework Execution
                    </h4>

                    <div>
                        <label class="block text-[11px] font-semibold tracking-wider text-stone-500 uppercase mb-1">Is there anything else close to your heart that will help customize this asset into an absolute masterpiece?</label>
                        <textarea name="client_final_thoughts" rows="4" placeholder="Share specific vision statements, unique boundaries, or formatting alignment tracking expectations..." class="w-full px-4 py-3 rounded-xl border border-stone-200 focus:border-[#8C7A6B] focus:ring-1 focus:ring-[#8C7A6B] outline-none bg-stone-50/40 transition"></textarea>
                    </div>

                    <div class="p-4 bg-[#8C7A6B]/5 border border-[#8C7A6B]/20 rounded-2xl">
                        <label class="flex items-start gap-3.5 cursor-pointer select-none text-xs leading-relaxed text-stone-600">
                            <input type="checkbox" name="retainer_acknowledgment_check" required class="mt-1 rounded accent-[#8C7A6B] w-4 h-4">
                            <span>
                                <strong class="text-stone-800 font-semibold block uppercase tracking-wider text-[10px] text-[#8C7A6B]">Retainer & Processing Acknowledgment</strong> 
                                I understand that upon submitting this discovery form, a digital invoice mapping to my portfolio selection will be delivered directly to my email. Once payment is securely processed, work on my custom asset layout will initiate.
                            </span>
                        </label>
                    </div>
                </div>

                <!-- Submission Interaction -->
                <button type="submit" id="submit-btn" class="w-full bg-[#4E5142] hover:bg-[#3D4035] text-white font-medium text-sm py-4 rounded-xl shadow-md transition-all duration-300 transform active:scale-[0.98]">
                    Submit Discovery Profile
                </button>
            </form>

            <!-- EXACT VERBATIM CUSTOM SUCCESS ALERT STATE -->
            <div id="success-message" class="hidden text-center py-10 space-y-4">
                <div class="inline-flex items-center justify-center w-12 h-12 rounded-full bg-emerald-50 text-emerald-600 border border-emerald-100 mb-1">
                    <svg class="w-6 h-6" fill="none" stroke="currentColor" stroke-width="2.5" viewBox="0 0 24 24">
                        <path stroke-linecap="round" stroke-linejoin="round" d="M5 13l4 4L19 7"></path>
                    </svg>
                </div>
                <h4 class="text-xl font-serif font-medium text-stone-800 px-4 leading-relaxed text-center">
                    Thank you for submitting the discovery form. you will receive an email from us soon. We look forward to curating a seamless journey for you and yours.
                </h4>
            </div>
        </section>

        <!-- Connection & Media Hub -->
        <section class="max-w-xl mx-auto border-t border-stone-200/60 pt-12 text-center">
            <span class="text-xs tracking-[0.2em] text-[#8C7A6B] uppercase font-bold">Connection & Media</span>
            <h3 class="text-2xl font-medium text-[#3D4035] mt-2 mb-6">Stay Immersed in the Journey</h3>
            
            <div class="space-y-3 text-left">
                <a href="https://your-newsletter.beehiiv.com" target="_blank" class="flex items-center justify-between bg-white hover:bg-stone-50 text-[#3D4035] border border-stone-200/60 rounded-xl px-6 py-4 shadow-sm transition transform hover:-translate-y-0.5">
                    <span class="font-medium text-sm flex items-center gap-3">
                        ✉️ <span class="tracking-wide">Subscribe to the Conscious Compass Dispatch</span>
                    </span>
                    <span class="text-xs text-[#8C7A6B]">Join on Beehiiv ➔</span>
                </a>

                <a href="https://youtube.com/@yourchannel" target="_blank" class="flex items-center justify-between bg-white hover:bg-stone-50 text-[#3D4035] border border-stone-200/60 rounded-xl px-6 py-4 shadow-sm transition transform hover:-translate-y-0.5">
                    <span class="font-medium text-sm flex items-center gap-3">
                        🎥 <span class="tracking-wide">Watch Art & Slow Travel Vlogs</span>
                    </span>
                    <span class="text-xs text-[#8C7A6B]">Watch on YouTube ➔</span>
                </a>

                <a href="https://instagram.com/yourusername" target="_blank" class="flex items-center justify-between bg-white hover:bg-stone-50 text-[#3D4035] border border-stone-200/60 rounded-xl px-6 py-4 shadow-sm transition transform hover:-translate-y-0.5">
                    <span class="font-medium text-sm flex items-center gap-3">
                        📸 <span class="tracking-wide">Follow Murals & Field Sketches</span>
                    </span>
                    <span class="text-xs text-[#8C7A6B]">Follow on Instagram ➔</span>
                </a>
            </div>
        </section>

    </main>

    <!-- Footer -->
    <footer class="border-t border-stone-200/40 bg-stone-100/30 py-8 text-center text-xs text-stone-500">
        <p>© 2026 The Conscious Compass Travel Co. All rights reserved.</p>
        <p class="mt-1 italic">Slow Travel. Fine Artistry. Uncompromised Safety.</p>
    </footer>

    <!-- Interactive Logic Execution Engine Scripts -->
    <script>
        function toggleAbout() {
            const extendedSection = document.getElementById('about-extended');
            const toggleText = document.getElementById('about-toggle-text');
            const toggleIcon = document.getElementById('about-toggle-icon');
            
            if (extendedSection.classList.contains('hidden')) {
                extendedSection.classList.remove('hidden');
                toggleText.innerText = "Collapse Story";
                toggleIcon.classList.add('rotate-180');
            } else {
                extendedSection.classList.add('hidden');
                toggleText.innerText = "Read My Full Story";
                toggleIcon.classList.remove('rotate-180');
            }
        }

        function toggleFAQ(id) {
            const faqContent = document.getElementById(`faq-${id}`);
            const faqIcon = document.getElementById(`icon-${id}`);
            
            if (faqContent.style.maxHeight && faqContent.style.maxHeight !== '0px') {
                // Smoothly close drawer container
                faqContent.style.maxHeight = '0px';
                faqContent.style.opacity = '0';
                faqIcon.classList.remove('rotate-180');
            } else {
                // Smoothly expand height parameters relative to child footprint
                faqContent.style.maxHeight = faqContent.scrollHeight + 'px';
                faqContent.style.opacity = '1';
                faqIcon.classList.add('rotate-180');
            }
        }

        // --- FORM LIVE BRANCHING LOGIC ENGINE ---
        document.addEventListener('DOMContentLoaded', function() {
            const partyRadios = document.querySelectorAll('input[name="party_dynamics"]');
            const familyAgesWrapper = document.getElementById('family-ages-wrapper');
            
            partyRadios.forEach(radio => {
                radio.addEventListener('change', function() {
                    if (this.value === 'family') {
                        familyAgesWrapper.classList.remove('hidden');
                    } else {
                        familyAgesWrapper.classList.add('hidden');
                    }
                });
            });

            const activeEnergyCheckbox = document.getElementById('energy-active-trigger');
            const agilityFieldsWrapper = document.getElementById('agility-fields-wrapper');
            
            activeEnergyCheckbox.addEventListener('change', function() {
                if (this.checked && !agilityFieldsWrapper.parentElement.classList.contains('hidden')) {
                    agilityFieldsWrapper.classList.remove('hidden');
                } else {
                    agilityFieldsWrapper.classList.add('hidden');
                }
            });

            const frameworkRadios = document.querySelectorAll('.framework-type-trigger');
            const travelCoreSection = document.getElementById('travel-core-fields');
            const artOnlySection = document.getElementById('art-only-fields');
            const finalSectionNum = document.getElementById('final-section-num');
            
            const tier1Div = document.getElementById('tier-1-fields');
            const tier2Div = document.getElementById('tier-2-fields');
            const tier3Div = document.getElementById('tier-3-fields');

            frameworkRadios.forEach(radio => {
                radio.addEventListener('change', function() {
                    tier1Div.classList.add('hidden');
                    tier2Div.classList.add('hidden');
                    tier3Div.classList.add('hidden');
                    artOnlySection.classList.add('hidden');
                    travelCoreSection.classList.add('hidden');

                    const selection = this.value;

                    if (selection === 'art_commission' || selection === 'art_print') {
                        artOnlySection.classList.remove('hidden');
                        finalSectionNum.innerText = "3";
                    } else {
                        travelCoreSection.classList.remove('hidden');
                        finalSectionNum.innerText = "4";
                        
                        if (selection === 'tier_1') tier1Div.classList.remove('hidden');
                        if (selection === 'tier_2') tier2Div.classList.remove('hidden');
                        if (selection === 'tier_3') tier3Div.classList.remove('hidden');
                        
                        if (activeEnergyCheckbox.checked) {
                            agilityFieldsWrapper.classList.remove('hidden');
                        }
                    }
                });
            });
        });

        // --- ARTISTIC WATERCOLOR HUMMINGBIRD PHYSICAL SIMULATION INTERFACE ---
        (function() {
            const container = document.getElementById('hummingbird-container');
            const svg = document.getElementById('hummingbird-svg');
            const overwing = document.getElementById('overwing');
            const underwing = document.getElementById('underwing');
            
            let lastScrollY = window.scrollY;
            let targetRotation = 0;
            let currentRotation = 0;
            let lastMouseX = -1000;
            let lastMouseY = -1000;
            let offsetX = 0;
            let offsetY = 0;
            let wingSpeed = 0.08; // Normal gentle gliding flap speed
            let animationFrameId = null;
            let baseBobTime = 0;

            // Handle scroll direction & intensity relative to rotation profiles
            window.addEventListener('scroll', function() {
                const currentScrollY = window.scrollY;
                const delta = currentScrollY - lastScrollY;
                lastScrollY = currentScrollY;
                
                targetRotation = delta * 0.15; // Shift angle intensity relative to drag friction
                targetRotation = Math.max(-30, Math.min(30, targetRotation));
            }, { passive: true });

            // Handle curious hovering interactions
            window.addEventListener('mousemove', function(e) {
                const rect = container.getBoundingClientRect();
                const birdX = rect.left + rect.width / 2;
                const birdY = rect.top + rect.height / 2;
                const dist = Math.hypot(e.clientX - birdX, e.clientY - birdY);

                if (dist < 180) {
                    // Flutter faster! Simulate wings in a high frequency blur state
                    wingSpeed = 0.02;
                    // Run a simple reactive offset vector to nudge the bird gently away
                    const angle = Math.atan2(birdY - e.clientY, birdX - birdX);
                    const push = (180 - dist) * 0.25;
                    offsetX = Math.cos(angle) * push;
                    offsetY = Math.sin(angle) * push;
                } else {
                    wingSpeed = 0.08; // Re-align to normal slow glide pacing
                    offsetX *= 0.95;  // Dampen pushback offset cleanly
                    offsetY *= 0.95;
                }
            });

            // Unified Render Animation Loop
            function step() {
                baseBobTime += 0.03;
                
                // Rotational dampening equations
                currentRotation += (targetRotation - currentRotation) * 0.08;
                targetRotation *= 0.95; // Gradually bleed off scrolling energy back to neutral orientation

                // Fluid organic bobbing sequence
                const bobY = Math.sin(baseBobTime) * 12;
                const bobX = Math.cos(baseBobTime * 0.5) * 4;

                const finalX = bobX + offsetX;
                const finalY = bobY + offsetY;

                // Apply matrices directly to layout structures
                container.style.transform = `translate3d(${finalX}px, ${finalY}px, 0) rotate(${currentRotation}deg)`;

                // Wing flapping cycle
                const flap = Math.sin(Date.now() * (1 / (wingSpeed * 1000)));
                const scaleWing = Math.max(0.1, (flap + 1) / 2); // Prevent wings from inside-out mirroring anomalies
                
                overwing.style.transform = `scaleY(${scaleWing})`;
                underwing.style.transform = `scaleY(${scaleWing})`;

                animationFrameId = requestAnimationFrame(step);
            }
            step();
        })();

        // Web3Forms Form Submission Pipeline Execution
        const form = document.getElementById('discover-form');
        const submitBtn = document.getElementById('submit-btn');
        const successMessage = document.getElementById('success-message');

        form.addEventListener('submit', function(e) {
            e.preventDefault();
            
            const apiKey = form.elements['access_key'].value;
            if (apiKey === 'YOUR_ACCESS_KEY_HERE') {
                alert("Please replace 'YOUR_ACCESS_KEY_HERE' inside the code with your free Web3Forms access key so submissions reach your email inbox safely!");
                return;
            }

            submitBtn.disabled = true;
            submitBtn.innerHTML = "Processing profile metrics...";

            const formData = new FormData(form);
            const object = Object.fromEntries(formData);
            
            const energyCheckboxes = document.querySelectorAll('input[name="trip_energy[]"]:checked');
            const energyValues = Array.from(energyCheckboxes).map(cb => cb.value);
            object['trip_energy_focus'] = energyValues.join(', ');

            const dietCheckboxes = document.querySelectorAll('input[name="t3_diet[]"]:checked');
            const dietValues = Array.from(dietCheckboxes).map(cb => cb.value);
            object['tier3_dietary_constraints'] = dietValues.join(', ');

            const json = JSON.stringify(object);

            fetch('https://api.web3forms.com/submit', {
                method: 'POST',
                headers: {
                    'Content-Type': 'application/json',
                    'Accept': 'application/json'
                },
                body: json
            })
            .then(async (response) => {
                let resJson = await response.json();
                if (response.status == 200) {
                    form.classList.add('hidden');
                    successMessage.classList.remove('hidden');
                } else {
                    alert(resJson.message || "Transmission failed. Please review your credentials.");
                    submitBtn.disabled = false;
                    submitBtn.innerHTML = "Submit Discovery Profile";
                }
            })
            .catch(error => {
                console.error(error);
                alert("An unexpected network transport interruption occurred.");
                submitBtn.disabled = false;
                submitBtn.innerHTML = "Submit Discovery Profile";
            });
        });
    </script>
</body>
</html>
