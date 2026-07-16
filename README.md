
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
<body class="min-h-screen flex flex-col justify-between selection:bg-stone-200">

    <!-- Elegant Text Branding (Sits cleanly above the banner) -->
    <header class="py-10 px-4 text-center max-w-4xl mx-auto">
        <h1 class="text-3xl md:text-5xl font-semibold tracking-widest text-[#3D4035] uppercase">
            The Conscious Compass
        </h1>
        <p class="text-xs md:text-sm tracking-[0.25em] text-[#8C7A6B] uppercase mt-4 font-semibold">
            Travel Co. • Artistry & Curated Journeys
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

        <!-- Section 1: Original Perfect Intro (About Me) -->
        <section class="max-w-2xl mx-auto mb-16 text-center">
            <h2 class="text-2xl md:text-3xl font-medium text-[#4E5142] italic leading-relaxed">
                "We travel not to escape life, but for life not to escape us."
            </h2>
            <p class="text-sm md:text-base text-stone-600 leading-relaxed mt-6">
                Welcome. I curate slow, immersive, and sensory travel blueprints with an artist's lens. Specializing in rainforest sanctuaries, uncompromised vegan and gluten-free dietary safety, and river voyages, every detail is handled with absolute care.
            </p>
        </section>

        <hr class="border-stone-200/60 my-16">

        <!-- Section 2: The Three Curated Service Tiers -->
        <section class="mb-20">
            <div class="text-center mb-12">
                <span class="text-xs tracking-[0.2em] text-[#8C7A6B] uppercase font-bold">Services & Blueprints</span>
                <h2 class="text-3xl md:text-4xl font-medium text-[#3D4035] mt-2">The Three Curated Tiers</h2>
                <p class="text-stone-500 text-sm mt-3">Choose the level of design, scaffolding, and support your journey requires.</p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <!-- Tier 1 -->
                <div class="bg-white border border-stone-200/60 rounded-2xl p-6 flex flex-col justify-between shadow-sm hover:shadow-md transition">
                    <div>
                        <span class="text-xs font-bold tracking-wider text-[#8C7A6B] uppercase">Tier 1</span>
                        <h3 class="text-xl font-bold text-[#3D4035] mt-1 mb-2">The Research Blueprint</h3>
                        <p class="text-2xl font-semibold text-[#4E5142] mb-4">$175</p>
                        <p class="text-stone-600 text-xs leading-relaxed mb-6">
                            For independent adventurers who love to wander but refuse to compromise on safety, dietary security, or localized transit stress.
                        </p>
                        <ul class="space-y-2 text-xs text-stone-600 border-t border-stone-100 pt-4">
                            <li class="flex items-start">✔️ Comprehensive Regional Transit Routing</li>
                            <li class="flex items-start">✔️ Deep-Dive Vegan & Gluten-Free Food Sourcing</li>
                            <li class="flex items-start">✔️ Custom Health & Emergency Protocol Maps</li>
                            <li class="flex items-start">✔️ Vetted Cross-Contamination Kitchen Checklists</li>
                        </ul>
                    </div>
                    <a href="#discover" class="block text-center mt-8 bg-stone-100 hover:bg-stone-200 text-[#3D4035] font-semibold text-xs py-3 rounded-lg transition">
                        Select Blueprint
                    </a>
                </div>

                <!-- Tier 2 -->
                <div class="bg-[#FAF6F0] border-2 border-[#8C7A6B]/30 rounded-2xl p-6 flex flex-col justify-between shadow-sm relative">
                    <div class="absolute -top-3 left-1/2 -translate-x-1/2 bg-[#8C7A6B] text-white text-[9px] tracking-wider uppercase py-1 px-3 rounded-full font-bold">
                        Most Popular
                    </div>
                    <div>
                        <span class="text-xs font-bold tracking-wider text-[#8C7A6B] uppercase mt-2 block">Tier 2</span>
                        <h3 class="text-xl font-bold text-[#3D4035] mt-1 mb-2">The Day-Hacker</h3>
                        <p class="text-2xl font-semibold text-[#4E5142] mb-4">$75 <span class="text-xs text-stone-500 font-normal">/ travel day</span></p>
                        <p class="text-stone-600 text-xs leading-relaxed mb-6">
                            Perfect balance. Structured, curated morning plans focusing on sensory activities, leaving the afternoon open for organic serendipity.
                        </p>
                        <ul class="space-y-2 text-xs text-stone-600 border-t border-stone-200/50 pt-4">
                            <li class="flex items-start">✔️ Daily Curated Morning Blueprints</li>
                            <li class="flex items-start">✔️ Interactive Custom GPX Maps (offline-capable)</li>
                            <li class="flex items-start">✔️ Detailed Safe-Dietary Dining Guides</li>
                            <li class="flex items-start">✔️ Intentional Slow-Stitch & Sketch Coordinates</li>
                        </ul>
                    </div>
                    <a href="#discover" class="block text-center mt-8 bg-[#4E5142] hover:bg-[#3D4035] text-white font-semibold text-xs py-3 rounded-lg transition">
                        Select Day-Hacker
                    </a>
                </div>

                <!-- Tier 3 -->
                <div class="bg-white border border-stone-200/60 rounded-2xl p-6 flex flex-col justify-between shadow-sm hover:shadow-md transition">
                    <div>
                        <span class="text-xs font-bold tracking-wider text-[#8C7A6B] uppercase">Tier 3</span>
                        <h3 class="text-xl font-bold text-[#3D4035] mt-1 mb-2">Custom Trip Retainer</h3>
                        <p class="text-2xl font-semibold text-[#4E5142] mb-4">$450+</p>
                        <p class="text-stone-600 text-xs leading-relaxed mb-6">
                            An end-to-end editorial trip masterpiece. I serve as your dedicated travel architect, drafting a fully personalized, sensory journey.
                        </p>
                        <ul class="space-y-2 text-xs text-stone-600 border-t border-stone-100 pt-4">
                            <li class="flex items-start">✔️ Completely Bespoke Daily Itineraries</li>
                            <li class="flex items-start">✔️ Hand-Picked Boutique Lodging Selection</li>
                            <li class="flex items-start">✔️ Direct, Commission-Free Booking Portals</li>
                            <li class="flex items-start">✔️ Dedicated Pre-Trip Consultations</li>
                        </ul>
                    </div>
                    <a href="#discover" class="block text-center mt-8 bg-stone-100 hover:bg-stone-200 text-[#3D4035] font-semibold text-xs py-3 rounded-lg transition">
                        Retain Architect
                    </a>
                </div>
            </div>
        </section>

        <hr class="border-stone-200/60 my-16">

        <!-- Section 3: Fine Art Travel Prints & Keepsakes -->
        <section class="mb-20">
            <div class="text-center mb-12">
                <span class="text-xs tracking-[0.2em] text-[#8C7A6B] uppercase font-bold">The Artist's Gallery</span>
                <h2 class="text-3xl md:text-4xl font-medium text-[#3D4035] mt-2">Travel Prints & Keepsakes</h2>
                <p class="text-stone-500 text-sm mt-3 max-w-lg mx-auto">
                    Bring the rich, misty atmosphere of the rainforest home. I offer custom, high-quality giclée prints of my watercolor landscapes and sketches.
                </p>
            </div>

            <div class="grid grid-cols-1 sm:grid-cols-2 gap-8 max-w-2xl mx-auto">
                <div class="bg-white p-3 rounded-2xl shadow-sm border border-stone-200/40">
                    <div class="aspect-[4/3] rounded-xl overflow-hidden bg-stone-100">
                        <img src="landscape.jpg" alt="Misty Canoe Watercolor Print" class="w-full h-full object-cover">
                    </div>
                    <div class="mt-4 px-2">
                        <h4 class="font-bold text-[#3D4035] text-sm">"Misty Basin Canoe Sketch"</h4>
                        <p class="text-xs text-stone-500 mt-1">Watercolors on cold-press archival paper. Inspired by cloud-forest waterways.</p>
                        <p class="text-xs font-semibold text-[#8C7A6B] mt-2">Available in custom sizing • Signed Edition</p>
                    </div>
                </div>

                <div class="bg-white p-3 rounded-2xl shadow-sm border border-stone-200/40 flex flex-col justify-center items-center text-center p-8">
                    <span class="text-xs tracking-wider uppercase text-[#8C7A6B] font-bold">Bespoke Keepsakes</span>
                    <h4 class="text-lg font-semibold text-[#3D4035] mt-2 mb-3">Custom Memory Illustrations</h4>
                    <p class="text-xs text-stone-500 leading-relaxed max-w-xs mb-6">
                        For Tier 3 clients, I offer custom original paintings of your favorite moments from your travel itinerary—framing a memory on your home walls forever.
                    </p>
                    <a href="#discover" class="bg-stone-100 hover:bg-stone-200 text-stone-700 text-xs font-semibold px-4 py-2 rounded-lg transition">
                        Inquire About Prints
                    </a>
                </div>
            </div>
        </section>

        <hr class="border-stone-200/60 my-16">

        <!-- Section 4: Interactive FAQ Directory -->
        <section class="mb-20 max-w-2xl mx-auto">
            <div class="text-center mb-12">
                <span class="text-xs tracking-[0.2em] text-[#8C7A6B] uppercase font-bold">Clarifying the Path</span>
                <h2 class="text-3xl md:text-4xl font-medium text-[#3D4035] mt-2">Frequently Asked Questions</h2>
            </div>

            <div class="space-y-4">
                <!-- FAQ Item 1 -->
                <div class="border border-stone-200/60 rounded-xl bg-white overflow-hidden">
                    <button class="w-full text-left p-5 font-semibold text-sm md:text-base text-[#3D4035] flex justify-between items-center focus:outline-none" onclick="toggleFAQ(1)">
                        <span>Why should I use an artist to plan my travel?</span>
                        <svg id="icon-1" class="w-4 h-4 text-stone-500 transform transition-transform duration-200" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" d="M19 9l-7 7-7-7"></path>
                        </svg>
                    </button>
                    <div id="faq-1" class="hidden px-5 pb-5 text-xs md:text-sm text-stone-600 leading-relaxed border-t border-stone-50 pt-3 bg-stone-50/30">
                        An artist curates with a sense of rhythm, atmosphere, and visual narrative. Instead of booking a chaotic list of popular attractions, I balance your itinerary like a painting—framing moments of quiet rest, breathtaking heights, and sensory details that standard agency formulas simply overlook.
                    </div>
                </div>

                <!-- FAQ Item 2 -->
                <div class="border border-stone-200/60 rounded-xl bg-white overflow-hidden">
                    <button class="w-full text-left p-5 font-semibold text-sm md:text-base text-[#3D4035] flex justify-between items-center focus:outline-none" onclick="toggleFAQ(2)">
                        <span>How do you guarantee vegan and gluten-free dietary safety?</span>
                        <svg id="icon-2" class="w-4 h-4 text-stone-500 transform transition-transform duration-200" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" d="M19 9l-7 7-7-7"></path>
                        </svg>
                    </button>
                    <div id="faq-2" class="hidden px-5 pb-5 text-xs md:text-sm text-stone-600 leading-relaxed border-t border-stone-50 pt-3 bg-stone-50/30">
                        I do not rely on standard search engine markers. I personally contact lodges, chefs, and kitchens to vet their supply chains, clarify cross-contamination protocols, and verify if kitchenettes are properly isolated. Your safety is handled with the absolute highest priority.
                    </div>
                </div>

                <!-- FAQ Item 3 -->
                <div class="border border-stone-200/60 rounded-xl bg-white overflow-hidden">
                    <button class="w-full text-left p-5 font-semibold text-sm md:text-base text-[#3D4035] flex justify-between items-center focus:outline-none" onclick="toggleFAQ(3)">
                        <span>Do you book the flights and hotels for me?</span>
                        <svg id="icon-3" class="w-4 h-4 text-stone-500 transform transition-transform duration-200" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" d="M19 9l-7 7-7-7"></path>
                        </svg>
                    </button>
                    <div id="faq-3" class="hidden px-5 pb-5 text-xs md:text-sm text-stone-600 leading-relaxed border-t border-stone-50 pt-3 bg-stone-50/30">
                        To maintain absolute clarity, financial safety, and zero hidden markups, you retain control of your booking details. I provide you with a high-end, compiled document containing direct, commission-free booking links. This allows you to secure all hotels and flights directly on your credit cards, while I design the seamless skeleton of the trip.
                    </div>
                </div>

                <!-- FAQ Item 4 -->
                <div class="border border-stone-200/60 rounded-xl bg-white overflow-hidden">
                    <button class="w-full text-left p-5 font-semibold text-sm md:text-base text-[#3D4035] flex justify-between items-center focus:outline-none" onclick="toggleFAQ(4)">
                        <span>What is your revision policy?</span>
                        <svg id="icon-4" class="w-4 h-4 text-stone-500 transform transition-transform duration-200" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" d="M19 9l-7 7-7-7"></path>
                        </svg>
                    </button>
                    <div id="faq-4" class="hidden px-5 pb-5 text-xs md:text-sm text-stone-600 leading-relaxed border-t border-stone-50 pt-3 bg-stone-50/30">
                        Every curated blueprint includes one round of complete aesthetic and logistical revisions. For the Custom Trip Retainer, we iterate together on draft concepts until the final picture matches your sensory vision perfectly.
                    </div>
                </div>
            </div>
        </section>

        <hr class="border-stone-200/60 my-16">

        <!-- Section 5: The Discovery Form -->
        <section id="discover" class="bg-white/60 backdrop-blur-md border border-stone-200/50 rounded-3xl p-6 md:p-10 shadow-sm max-w-2xl mx-auto">
            <h3 class="text-2xl font-semibold text-[#3D4035] text-center mb-2">Begin Your Journey</h3>
            <p class="text-xs text-stone-500 text-center mb-8">Fill out our Discovery Form below to outline your custom requirements and chosen tier.</p>

            <!-- Web3Forms Integration -->
            <form action="https://api.web3forms.com/submit" method="POST" id="discover-form" class="space-y-6">
                <!-- IMPORTANT: Paste your free Web3Forms Access Key here -->
                <input type="hidden" name="access_key" value="YOUR_ACCESS_KEY_HERE">
                <input type="hidden" name="subject" value="New Discovery Request - Conscious Compass">
                <input type="hidden" name="from_name" value="The Conscious Compass Website">
                <input type="hidden" name="redirect" value="">

                <!-- Input Fields -->
                <div class="space-y-4">
                    <div>
                        <label class="block text-xs font-semibold tracking-wider text-stone-600 uppercase mb-1">Your Full Name</label>
                        <input type="text" name="name" required class="w-full px-4 py-3 rounded-xl border border-stone-200 focus:border-[#8C7A6B] focus:ring-1 focus:ring-[#8C7A6B] outline-none bg-stone-50/50 text-sm transition" placeholder="Your Name">
                    </div>

                    <div>
                        <label class="block text-xs font-semibold tracking-wider text-stone-600 uppercase mb-1">Email Address</label>
                        <input type="email" name="email" required class="w-full px-4 py-3 rounded-xl border border-stone-200 focus:border-[#8C7A6B] focus:ring-1 focus:ring-[#8C7A6B] outline-none bg-stone-50/50 text-sm transition" placeholder="hello@example.com">
                    </div>

                    <div>
                        <label class="block text-xs font-semibold tracking-wider text-stone-600 uppercase mb-1">Where are we exploring? (Destination)</label>
                        <input type="text" name="destination" required class="w-full px-4 py-3 rounded-xl border border-stone-200 focus:border-[#8C7A6B] focus:ring-1 focus:ring-[#8C7A6B] outline-none bg-stone-50/50 text-sm transition" placeholder="e.g. Costa Rica Rainforest, Colombia Highland Canopy">
                    </div>

                    <div class="grid grid-cols-2 gap-4">
                        <div>
                            <label class="block text-xs font-semibold tracking-wider text-stone-600 uppercase mb-1">Travel Date</label>
                            <input type="date" name="travel_date" class="w-full px-4 py-3 rounded-xl border border-stone-200 focus:border-[#8C7A6B] focus:ring-1 focus:ring-[#8C7A6B] outline-none bg-stone-50/50 text-sm transition">
                        </div>
                        <div>
                            <label class="block text-xs font-semibold tracking-wider text-stone-600 uppercase mb-1">Duration (Days)</label>
                            <input type="number" name="duration" min="1" class="w-full px-4 py-3 rounded-xl border border-stone-200 focus:border-[#8C7A6B] focus:ring-1 focus:ring-[#8C7A6B] outline-none bg-stone-50/50 text-sm transition" placeholder="10">
                        </div>
                    </div>

                    <div>
                        <label class="block text-xs font-semibold tracking-wider text-stone-600 uppercase mb-1">Selected Tier</label>
                        <select name="service_tier" class="w-full px-4 py-3 rounded-xl border border-stone-200 focus:border-[#8C7A6B] focus:ring-1 focus:ring-[#8C7A6B] outline-none bg-stone-50/50 text-sm transition">
                            <option value="tier_1">Tier 1: The Research Blueprint ($175)</option>
                            <option value="tier_2">Tier 2: The Day-Hacker ($75/day)</option>
                            <option value="tier_3">Tier 3: The Custom Trip Retainer ($450+)</option>
                            <option value="art_prints">Fine Art Prints & Sketches Only</option>
                        </select>
                    </div>

                    <div>
                        <label class="block text-xs font-semibold tracking-wider text-stone-600 uppercase mb-1">Dietary & Safety Priorities</label>
                        <textarea name="dietary" rows="3" class="w-full px-4 py-3 rounded-xl border border-stone-200 focus:border-[#8C7A6B] focus:ring-1 focus:ring-[#8C7A6B] outline-none bg-stone-50/50 text-sm transition" placeholder="e.g., Strict vegan & gluten-free food tracking, slow pace, specific mobility requirements..."></textarea>
                    </div>
                </div>

                <!-- Interactive Submit Button -->
                <button type="submit" id="submit-btn" class="w-full bg-[#4E5142] hover:bg-[#3D4035] text-white font-medium text-sm py-4 rounded-xl shadow-md transition-all duration-300 transform active:scale-[0.98]">
                    Submit Discovery Request
                </button>
            </form>

            <!-- Dynamic AJAX Success Message -->
            <div id="success-message" class="hidden text-center py-8 space-y-4">
                <div class="inline-flex items-center justify-center w-16 h-16 rounded-full bg-emerald-50 border border-emerald-100 mb-2">
                    <svg class="w-8 h-8 text-emerald-600" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24">
                        <path stroke-linecap="round" stroke-linejoin="round" d="M5 13l4 4L19 7"></path>
                    </svg>
                </div>
                <h4 class="text-2xl font-medium text-stone-800">Bespoke Request Received</h4>
                <p class="text-sm text-stone-600 max-w-md mx-auto leading-relaxed">
                    Thank you. Your sensory profile has been securely received. I will review your preferences and reach out to outline your custom journey blueprint.
                </p>
            </div>
        </section>
    </main>

    <!-- Footer -->
    <footer class="border-t border-stone-200/40 bg-stone-100/30 py-8 text-center text-xs text-stone-500">
        <p>© 2026 The Conscious Compass Travel Co. All rights reserved.</p>
        <p class="mt-1 italic">Slow Travel. Fine Artistry. Uncompromised Safety.</p>
    </footer>

    <!-- Interactive FAQ Toggler & Form Submit Script -->
    <script>
        // FAQ Accordion Handler
        function toggleFAQ(id) {
            const faqContent = document.getElementById(`faq-${id}`);
            const faqIcon = document.getElementById(`icon-${id}`);
            
            if (faqContent.classList.contains('hidden')) {
                faqContent.classList.remove('hidden');
                faqIcon.classList.add('rotate-180');
            } else {
                faqContent.classList.add('hidden');
                faqIcon.classList.remove('rotate-180');
            }
        }

        // Web3Forms Submit Handler
        const form = document.getElementById('discover-form');
        const submitBtn = document.getElementById('submit-btn');
        const successMessage = document.getElementById('success-message');

        form.addEventListener('submit', function(e) {
            e.preventDefault();
            
            const apiKey = form.elements['access_key'].value;
            if (apiKey === 'YOUR_ACCESS_KEY_HERE') {
                alert("Please replace 'YOUR_ACCESS_KEY_HERE' inside the code with your free Web3Forms access key so submissions reach your email!");
                return;
            }

            submitBtn.disabled = true;
            submitBtn.innerHTML = "Sending secure request...";

            const formData = new FormData(form);
            const object = Object.fromEntries(formData);
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
                    alert(resJson.message || "Submission failed. Please try again.");
                    submitBtn.disabled = false;
                    submitBtn.innerHTML = "Submit Discovery Request";
                }
            })
            .catch(error => {
                console.error(error);
                alert("Something went wrong. Please check your connection.");
                submitBtn.disabled = false;
                submitBtn.innerHTML = "Submit Discovery Request";
            });
        });
    </script>
</body>
</html>
