# Hub
Boutique Travel planner. A curated journey for you and yours.
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>The Conscious Compass | Custom Travel Curation & Intelligence</title>
    <!-- Google Fonts: Editorial Serif and clean sans-serif UI -->
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400..900;1,400..900&family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        brand: {
                            forest: '#1e2d28',
                            forestLight: '#2a3c36',
                            sage: '#6b8277',
                            linen: '#faf9f6',
                            linenDark: '#f4f3ef',
                            accent: '#c29a53',
                            charcoal: '#2c2e2a'
                        }
                    },
                    fontFamily: {
                        serif: ['"Playfair Display"', 'Georgia', 'serif'],
                        sans: ['Inter', 'sans-serif']
                    }
                }
            }
        }
    </script>
    <style>
        /* Smooth transitions for tabs and accordions */
        .transition-all-300 {
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
        }
        /* Custom scrollbar for premium aesthetic */
        ::-webkit-scrollbar {
            width: 6px;
        }
        ::-webkit-scrollbar-track {
            background: #faf9f6;
        }
        ::-webkit-scrollbar-thumb {
            background: #cbd1b6;
            border-radius: 3px;
        }
        ::-webkit-scrollbar-thumb:hover {
            background: #6b8277;
        }
    </style>
</head>
<body class="bg-brand-linen text-brand-charcoal font-sans min-h-screen flex flex-col justify-between">

    <!-- Hero / Cinematic Cover Photo Section -->
    <div class="w-full h-48 md:h-64 relative overflow-hidden bg-brand-forest">
        <!-- Background image with local fallback -->
        <img src="landscape.jpg" 
             onerror="this.src='https://images.unsplash.com/photo-1507525428034-b723cf961d3e?auto=format&fit=crop&w=1200&q=80'" 
             alt="Bespoke Travel Landscape" 
             class="w-full h-full object-cover opacity-80 mix-blend-multiply transition-all-300">
        <div class="absolute inset-0 bg-gradient-to-t from-brand-linen/40 via-transparent to-transparent"></div>
    </div>

    <!-- Header / Profile Segment -->
    <header class="w-full max-w-2xl mx-auto px-6 -mt-16 md:-mt-24 relative z-10 text-center pb-6">
        <div class="relative w-28 h-28 md:w-36 md:h-36 mx-auto mb-4 rounded-full overflow-hidden border-4 border-brand-linen bg-white shadow-md">
            <!-- Portrait picture with initials fallback -->
            <img src="portrait.jpg" 
                 onerror="this.style.display='none'; document.getElementById('avatar-fallback').style.display='flex';" 
                 alt="Holly E. Meinert" 
                 class="w-full h-full object-cover">
            <div id="avatar-fallback" class="hidden w-full h-full bg-brand-forest flex items-center justify-center text-brand-linen font-serif text-3xl md:text-4xl font-bold italic">
                CC
            </div>
        </div>
        <h1 class="font-serif text-3xl md:text-4xl font-bold tracking-wide text-brand-forest mb-1">The Conscious Compass</h1>
        <p class="font-serif italic text-brand-sage text-md md:text-lg mb-3">Bespoke Travel Design & Curation</p>
        <p class="max-w-md mx-auto text-sm text-brand-charcoal/90 leading-relaxed font-light">
            Bespoke travel design at the intersection of artistic exploration, flawless logistics, and deeply intentional curation.
        </p>
    </header>

    <!-- Interactive Tab Bar -->
    <nav class="w-full max-w-2xl mx-auto px-4 mb-6">
        <div class="bg-brand-linenDark p-1 rounded-xl flex items-center justify-between shadow-inner text-xs md:text-sm font-medium overflow-x-auto whitespace-nowrap gap-1">
            <button onclick="switchTab('links')" id="tab-links" class="tab-btn flex-1 py-2 px-3 rounded-lg text-center transition-all-300 bg-brand-forest text-white shadow-sm">
                Hub Links
            </button>
            <button onclick="switchTab('services')" id="tab-services" class="tab-btn flex-1 py-2 px-3 rounded-lg text-center transition-all-300 text-brand-forest hover:bg-brand-linen/60">
                Our Tiers
            </button>
            <button onclick="switchTab('intake')" id="tab-intake" class="tab-btn flex-1 py-2 px-3 rounded-lg text-center transition-all-300 text-brand-forest hover:bg-brand-linen/60">
                Discovery Form
            </button>
            <button onclick="switchTab('about')" id="tab-about" class="tab-btn flex-1 py-2 px-3 rounded-lg text-center transition-all-300 text-brand-forest hover:bg-brand-linen/60">
                About & Art
            </button>
            <button onclick="switchTab('faq')" id="tab-faq" class="tab-btn flex-1 py-2 px-3 rounded-lg text-center transition-all-300 text-brand-forest hover:bg-brand-linen/60">
                FAQs
            </button>
        </div>
    </nav>

    <!-- Main Container for Active Content View -->
    <main class="w-full max-w-2xl mx-auto px-4 flex-grow mb-12">

        <!-- TAB 1: LINK HUB -->
        <div id="view-links" class="tab-view space-y-4">
            <!-- Action Highlight Card -->
            <div class="bg-brand-forest text-brand-linen p-6 rounded-2xl shadow-md border border-brand-forestLight relative overflow-hidden">
                <div class="absolute top-0 right-0 w-24 h-24 bg-brand-accent/10 rounded-full blur-xl"></div>
                <span class="inline-block text-[10px] font-semibold uppercase tracking-widest text-brand-accent mb-2">Interactive Masterclass</span>
                <h3 class="font-serif text-xl font-bold mb-2">Ready to Design Your Trip?</h3>
                <p class="text-xs text-brand-linen/80 font-light mb-4 leading-relaxed">
                    Skip the endless planning loops. Open our tailored multi-step discovery form right inside this app to share your parameters.
                </p>
                <button onclick="switchTab('intake')" class="inline-flex items-center text-xs font-semibold uppercase tracking-wider text-brand-accent border border-brand-accent/40 bg-brand-forestLight/50 px-4 py-2 rounded-lg hover:bg-brand-accent hover:text-brand-forest hover:border-transparent transition-all-300">
                    Open Discovery Form
                    <svg class="w-4 h-4 ml-1.5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M14 5l7 7m0 0l-7 7m7-7H3"/></svg>
                </button>
            </div>

            <!-- Dynamic Link list -->
            <div class="space-y-3">
                <a href="#" onclick="switchTab('services'); return false;" class="group flex items-center justify-between p-4 bg-white hover:bg-brand-linenDark border border-brand-linenDark rounded-xl shadow-sm transition-all-300 hover:translate-x-1">
                    <div class="flex items-center space-x-3">
                        <div class="p-2 bg-brand-linenDark rounded-lg text-brand-forest group-hover:bg-white transition-all-300">
                            <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5H7a2 2 0 00-2 2v12a2 2 0 002 2h10a2 2 0 002-2V7a2 2 0 00-2-2h-2M9 5a2 2 0 002 2h2a2 2 0 002-2M9 5a2 2 0 012-2h2a2 2 0 012 2"/></svg>
                        </div>
                        <div>
                            <h4 class="text-sm font-semibold text-brand-forest">Explore Service Offerings & Tiers</h4>
                            <p class="text-xs text-brand-charcoal/60 font-light">From $175 Research Dossiers to Full Custom Retainers</p>
                        </div>
                    </div>
                    <svg class="w-4 h-4 text-brand-sage group-hover:text-brand-forest" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7"/></svg>
                </a>

                <a href="#" onclick="switchTab('faq'); return false;" class="group flex items-center justify-between p-4 bg-white hover:bg-brand-linenDark border border-brand-linenDark rounded-xl shadow-sm transition-all-300 hover:translate-x-1">
                    <div class="flex items-center space-x-3">
                        <div class="p-2 bg-brand-linenDark rounded-lg text-brand-forest group-hover:bg-white transition-all-300">
                            <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M8.228 9c.549-1.165 2.03-2 3.772-2 2.21 0 4 1.343 4 3 0 1.4-1.278 2.575-3.006 2.907-.542.104-.994.54-.994 1.093m0 3h.01M21 12a9 9 0 11-18 0 9 9 0 0118 0z"/></svg>
                        </div>
                        <div>
                            <h4 class="text-sm font-semibold text-brand-forest">Frequently Asked Questions</h4>
                            <p class="text-xs text-brand-charcoal/60 font-light">Understand our fee structures & non-agency design model</p>
                        </div>
                    </div>
                    <svg class="w-4 h-4 text-brand-sage group-hover:text-brand-forest" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7"/></svg>
                </a>

                <a href="#" onclick="switchTab('about'); return false;" class="group flex items-center justify-between p-4 bg-white hover:bg-brand-linenDark border border-brand-linenDark rounded-xl shadow-sm transition-all-300 hover:translate-x-1">
                    <div class="flex items-center space-x-3">
                        <div class="p-2 bg-brand-linenDark rounded-lg text-brand-forest group-hover:bg-white transition-all-300">
                            <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 16l4.586-4.586a2 2 0 012.828 0L16 16m-2-2l1.586-1.586a2 2 0 012.828 0L20 14m-6-6h.01M6 20h12a2 2 0 002-2V6a2 2 0 00-2-2H6a2 2 0 00-2 2v12a2 2 0 002 2z"/></svg>
                        </div>
                        <div>
                            <h4 class="text-sm font-semibold text-brand-forest">Artistic Portfolios & Fine Art Prints</h4>
                            <p class="text-xs text-brand-charcoal/60 font-light">View curation frames, design philosophy, and shop logs</p>
                        </div>
                    </div>
                    <svg class="w-4 h-4 text-brand-sage group-hover:text-brand-forest" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7"/></svg>
                </a>
            </div>
        </div>

        <!-- TAB 2: SERVICE OFFERINGS -->
        <div id="view-services" class="tab-view hidden space-y-6">
            <div class="text-center max-w-md mx-auto mb-6">
                <h3 class="font-serif text-2xl font-bold text-brand-forest">Tailored Design Frameworks</h3>
                <p class="text-xs text-brand-charcoal/60 mt-1 font-light">Uncompromised custom research and chronological masterworks, anchored in value.</p>
            </div>

            <!-- Tier 1 Card -->
            <div class="bg-white border border-brand-linenDark p-6 rounded-2xl shadow-sm space-y-4 hover:shadow-md transition-all-300">
                <div class="flex justify-between items-start">
                    <div>
                        <span class="text-[10px] font-semibold uppercase tracking-widest text-brand-sage bg-brand-linenDark px-2 py-1 rounded">Tier 1</span>
                        <h4 class="font-serif text-xl font-bold text-brand-forest mt-2">The Deep-Dive Research Blueprint</h4>
                    </div>
                    <div class="text-right">
                        <span class="text-2xl font-serif font-bold text-brand-forest">$175</span>
                        <p class="text-[9px] text-brand-charcoal/50 uppercase tracking-wider font-semibold">Flat Dossier</p>
                    </div>
                </div>
                <p class="text-xs text-brand-charcoal/80 font-light leading-relaxed">
                    Designed for independent explorers who manage their own bookings but demand expert spatial intelligence to eliminate anxiety surrounding entry paperwork, regional transit, and neighborhood safety parameters.
                </p>
                <div class="bg-brand-linen font-light text-xs p-4 rounded-xl border border-brand-linenDark space-y-2">
                    <p class="font-semibold text-brand-forest uppercase tracking-wider text-[9px]">Included Deliverables:</p>
                    <div class="grid grid-cols-2 gap-2 text-brand-charcoal/90">
                        <span class="flex items-center"><svg class="w-3.5 h-3.5 text-brand-accent mr-1.5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5" d="M5 13l4 4L19 7"/></svg>Transit Matrices</span>
                        <span class="flex items-center"><svg class="w-3.5 h-3.5 text-brand-accent mr-1.5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5" d="M5 13l4 4L19 7"/></svg>Entry Compliance</span>
                        <span class="flex items-center"><svg class="w-3.5 h-3.5 text-brand-accent mr-1.5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5" d="M5 13l4 4L19 7"/></svg>Safety Briefs</span>
                        <span class="flex items-center"><svg class="w-3.5 h-3.5 text-brand-accent mr-1.5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5" d="M5 13l4 4L19 7"/></svg>Gear Checklists</span>
                    </div>
                </div>
                <button onclick="startIntakeWithTier('tier1')" class="w-full text-center text-xs font-semibold uppercase tracking-wider bg-brand-linenDark hover:bg-brand-forest hover:text-white text-brand-forest py-3 rounded-xl transition-all-300">
                    Secure Research Blueprint
                </button>
            </div>

            <!-- Tier 2 Card -->
            <div class="bg-white border border-brand-linenDark p-6 rounded-2xl shadow-sm space-y-4 hover:shadow-md transition-all-300">
                <div class="flex justify-between items-start">
                    <div>
                        <span class="text-[10px] font-semibold uppercase tracking-widest text-brand-sage bg-brand-linenDark px-2 py-1 rounded">Tier 2</span>
                        <h4 class="font-serif text-xl font-bold text-brand-forest mt-2">The "Day-Hacker" Partial Itinerary</h4>
                    </div>
                    <div class="text-right">
                        <span class="text-2xl font-serif font-bold text-brand-forest">$75</span>
                        <p class="text-[9px] text-brand-charcoal/50 uppercase tracking-wider font-semibold">Per Planned Day</p>
                    </div>
                </div>
                <p class="text-xs text-brand-charcoal/80 font-light leading-relaxed">
                    A highly strategic execution plugin for travelers who have the frame of their vacation figured out, but require minute-by-minute architectural routing, curated dining, and logistical linkage for specific high-friction days. *(2-Day Minimum)*
                </p>
                <div class="bg-brand-linen font-light text-xs p-4 rounded-xl border border-brand-linenDark space-y-2">
                    <p class="font-semibold text-brand-forest uppercase tracking-wider text-[9px]">Included Deliverables:</p>
                    <div class="grid grid-cols-2 gap-2 text-brand-charcoal/90">
                        <span class="flex items-center"><svg class="w-3.5 h-3.5 text-brand-accent mr-1.5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5" d="M5 13l4 4L19 7"/></svg>Time-Blocked pacing</span>
                        <span class="flex items-center"><svg class="w-3.5 h-3.5 text-brand-accent mr-1.5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5" d="M5 13l4 4L19 7"/></svg>Transit connection maps</span>
                        <span class="flex items-center"><svg class="w-3.5 h-3.5 text-brand-accent mr-1.5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5" d="M5 13l4 4L19 7"/></svg>Artisan/Store matches</span>
                        <span class="flex items-center"><svg class="w-3.5 h-3.5 text-brand-accent mr-1.5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5" d="M5 13l4 4L19 7"/></svg>Custom Dining recommendations</span>
                    </div>
                </div>
                <button onclick="startIntakeWithTier('tier2')" class="w-full text-center text-xs font-semibold uppercase tracking-wider bg-brand-linenDark hover:bg-brand-forest hover:text-white text-brand-forest py-3 rounded-xl transition-all-300">
                    Secure Day-Hacker Plugin
                </button>
            </div>

            <!-- Tier 3 Card -->
            <div class="bg-brand-forest text-brand-linen p-6 rounded-2xl shadow-md border border-brand-forestLight space-y-4 relative overflow-hidden">
                <div class="absolute top-0 right-0 w-32 h-32 bg-brand-accent/5 rounded-full blur-2xl"></div>
                <div class="flex justify-between items-start">
                    <div>
                        <span class="text-[10px] font-semibold uppercase tracking-widest text-brand-accent bg-brand-forestLight px-2 py-1 rounded">Tier 3</span>
                        <h4 class="font-serif text-xl font-bold text-brand-linen mt-2">The All-Inclusive Custom Retainer</h4>
                    </div>
                    <div class="text-right">
                        <span class="text-2xl font-serif font-bold text-brand-linen">$450+</span>
                        <p class="text-[9px] text-brand-accent uppercase tracking-wider font-semibold">Flagship Design</p>
                    </div>
                </div>
                <p class="text-xs text-brand-linen/80 font-light leading-relaxed">
                    Our flagship design experience. A beautifully mapped, end-to-end master document coordinating hotel vetting, dietary checks, topography synchronization, and physical pacing with an uncompromising artistic lens.
                </p>
                <div class="bg-brand-forestLight/50 font-light text-xs p-4 rounded-xl border border-brand-forestLight space-y-2 text-brand-linen/95">
                    <p class="font-semibold text-brand-accent uppercase tracking-wider text-[9px]">The Master Framework Deliverables:</p>
                    <div class="grid grid-cols-2 gap-2">
                        <span class="flex items-center"><svg class="w-3.5 h-3.5 text-brand-accent mr-1.5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5" d="M5 13l4 4L19 7"/></svg>Chronological timeline</span>
                        <span class="flex items-center"><svg class="w-3.5 h-3.5 text-brand-accent mr-1.5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5" d="M5 13l4 4L19 7"/></svg>Boutique hotel lists</span>
                        <span class="flex items-center"><svg class="w-3.5 h-3.5 text-brand-accent mr-1.5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5" d="M5 13l4 4L19 7"/></svg>Allergen verification</span>
                        <span class="flex items-center"><svg class="w-3.5 h-3.5 text-brand-accent mr-1.5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5" d="M5 13l4 4L19 7"/></svg>Two revision rounds</span>
                    </div>
                </div>
                <button onclick="startIntakeWithTier('tier3')" class="w-full text-center text-xs font-semibold uppercase tracking-wider bg-brand-accent hover:bg-white text-brand-forest hover:text-brand-forest py-3 rounded-xl transition-all-300 shadow">
                    Apply for Custom Trip Retainer
                </button>
            </div>
        </div>

        <!-- TAB 3: LIVE DISCOVERY FORM -->
        <div id="view-intake" class="tab-view hidden bg-white border border-brand-linenDark rounded-2xl shadow-sm p-6 relative">
            
            <!-- Progress Stepper Tracker -->
            <div class="flex items-center justify-between mb-8 pb-4 border-b border-brand-linenDark text-xs font-semibold uppercase tracking-widest text-brand-sage">
                <span id="step-indicator">Step 1 of 5</span>
                <div class="w-1/2 bg-brand-linenDark h-1.5 rounded-full overflow-hidden">
                    <div id="step-progress" class="bg-brand-accent h-full transition-all-300" style="width: 20%;"></div>
                </div>
            </div>

            <!-- Custom Error Notification Panel (Avoids alert blocks) -->
            <div id="error-alert-box" class="hidden mb-6 p-4 bg-red-50 border border-red-200 text-red-800 rounded-xl text-sm font-light">
                <span class="font-semibold text-xs uppercase tracking-wider block mb-1">Attention Required</span>
                <span id="error-alert-message"></span>
            </div>

            <form id="discoveryForm" onsubmit="handleFormSubmission(event)" class="space-y-6">
                
                <!-- STEP 1: CONTACT & SERVICE SELECTION -->
                <div id="form-step-1" class="form-step space-y-4">
                    <h3 class="font-serif text-lg font-bold text-brand-forest">Step 1: The Core Foundation</h3>
                    
                    <div class="space-y-3">
                        <div>
                            <label class="block text-xs font-semibold uppercase tracking-wider text-brand-charcoal/80 mb-1.5">First & Last Name *</label>
                            <input type="text" id="clientName" required class="w-full p-3 bg-brand-linenDark border border-transparent focus:border-brand-sage focus:bg-white outline-none rounded-xl text-sm transition-all-300">
                        </div>
                        <div class="grid grid-cols-1 md:grid-cols-2 gap-3">
                            <div>
                                <label class="block text-xs font-semibold uppercase tracking-wider text-brand-charcoal/80 mb-1.5">Email Address *</label>
                                <input type="email" id="clientEmail" required class="w-full p-3 bg-brand-linenDark border border-transparent focus:border-brand-sage focus:bg-white outline-none rounded-xl text-sm transition-all-300">
                            </div>
                            <div>
                                <label class="block text-xs font-semibold uppercase tracking-wider text-brand-charcoal/80 mb-1.5">Phone Number *</label>
                                <input type="tel" id="clientPhone" required class="w-full p-3 bg-brand-linenDark border border-transparent focus:border-brand-sage focus:bg-white outline-none rounded-xl text-sm transition-all-300">
                            </div>
                        </div>
                        <div>
                            <label class="block text-xs font-semibold uppercase tracking-wider text-brand-charcoal/80 mb-1.5">Travel Party Dynamics *</label>
                            <select id="partyType" required onchange="toggleChildrenInput()" class="w-full p-3 bg-brand-linenDark border border-transparent focus:border-brand-sage focus:bg-white outline-none rounded-xl text-sm transition-all-300">
                                <option value="solo">Just me (Solo traveler)</option>
                                <option value="couple">Me and a partner/spouse</option>
                                <option value="family">A family trip</option>
                                <option value="group">A group of friends or extended family</option>
                            </select>
                        </div>
                        <div id="childrenAgesContainer" class="hidden">
                            <label class="block text-xs font-semibold uppercase tracking-wider text-brand-charcoal/80 mb-1.5">Please list the ages of any children traveling:</label>
                            <input type="text" id="childrenAges" placeholder="e.g. 8, 11" class="w-full p-3 bg-brand-linenDark border border-transparent focus:border-brand-sage focus:bg-white outline-none rounded-xl text-sm transition-all-300">
                        </div>
                        <div>
                            <label class="block text-xs font-semibold uppercase tracking-wider text-brand-charcoal/80 mb-1.5">Premium Service Selection *</label>
                            <select id="selectedTier" required class="w-full p-3 bg-brand-linenDark border border-transparent focus:border-brand-sage focus:bg-white outline-none rounded-xl text-sm font-semibold text-brand-forest transition-all-300">
                                <option value="tier1">Tier 1: The Deep-Dive Research Blueprint ($175)</option>
                                <option value="tier2">Tier 2: The "Day-Hacker" Partial Itinerary ($75/day)</option>
                                <option value="tier3">Tier 3: The All-Inclusive Custom Trip Retainer ($450+)</option>
                            </select>
                        </div>
                    </div>
                </div>

                <!-- STEP 2: DESTINATION, ENERGY & AGILITY CONDITIONAL -->
                <div id="form-step-2" class="form-step hidden space-y-4">
                    <h3 class="font-serif text-lg font-bold text-brand-forest">Step 2: Destination & Travel Energy</h3>
                    
                    <div class="space-y-4">
                        <div class="grid grid-cols-1 md:grid-cols-2 gap-3">
                            <div>
                                <label class="block text-xs font-semibold uppercase tracking-wider text-brand-charcoal/80 mb-1.5">Where are you heading? *</label>
                                <input type="text" id="destination" required placeholder="e.g. Costa Rica, Kyoto" class="w-full p-3 bg-brand-linenDark border border-transparent focus:border-brand-sage focus:bg-white outline-none rounded-xl text-sm transition-all-300">
                            </div>
                            <div>
                                <label class="block text-xs font-semibold uppercase tracking-wider text-brand-charcoal/80 mb-1.5">Estimated Travel Dates *</label>
                                <input type="text" id="travelDates" required placeholder="e.g. October 14 - 24, 2026" class="w-full p-3 bg-brand-linenDark border border-transparent focus:border-brand-sage focus:bg-white outline-none rounded-xl text-sm transition-all-300">
                            </div>
                        </div>

                        <div>
                            <label class="block text-xs font-semibold uppercase tracking-wider text-brand-charcoal/80 mb-2">When you close your eyes, what is the focus? * (Select up to 2)</label>
                            <div class="space-y-2">
                                <label class="flex items-start text-sm font-light text-brand-charcoal cursor-pointer">
                                    <input type="checkbox" name="vibeFocus" value="culture" class="mt-1 mr-2 rounded border-gray-300 text-brand-forest focus:ring-brand-sage">
                                    <span>Deep immersion into local culture, arts, and history</span>
                                </label>
                                <label class="flex items-start text-sm font-light text-brand-charcoal cursor-pointer">
                                    <input type="checkbox" name="vibeFocus" value="adventure" id="activeAdventureCheckbox" onchange="togglePhysicalAgilityQuestion()" class="mt-1 mr-2 rounded border-gray-300 text-brand-forest focus:ring-brand-sage">
                                    <span class="font-medium text-brand-forest">Active exploration, hiking, and navigating diverse topographies 🏔️</span>
                                </label>
                                <label class="flex items-start text-sm font-light text-brand-charcoal cursor-pointer">
                                    <input type="checkbox" name="vibeFocus" value="nature" class="mt-1 mr-2 rounded border-gray-300 text-brand-forest focus:ring-brand-sage">
                                    <span>Unplugged relaxation, nature, and slow-paced wandering</span>
                                </label>
                                <label class="flex items-start text-sm font-light text-brand-charcoal cursor-pointer">
                                    <input type="checkbox" name="vibeFocus" value="culinary" class="mt-1 mr-2 rounded border-gray-300 text-brand-forest focus:ring-brand-sage">
                                    <span>Culinary journeys, local markets, and food scenes</span>
                                </label>
                                <label class="flex items-start text-sm font-light text-brand-charcoal cursor-pointer">
                                    <input type="checkbox" name="vibeFocus" value="sustainable" class="mt-1 mr-2 rounded border-gray-300 text-brand-forest focus:ring-brand-sage">
                                    <span>Eco-conscious, sustainable, and wildlife-focused travel</span>
                                </label>
                            </div>
                        </div>

                        <!-- CONDITIONAL: Hidden unless Hiking/Adventure selected -->
                        <div id="physicalAgilityContainer" class="hidden p-4 bg-brand-linenDark border border-brand-accent/20 rounded-2xl space-y-3 transition-all-300">
                            <label class="block text-xs font-semibold uppercase tracking-wider text-brand-forest mb-1.5">🏔️ Physical Agility & Terrain Comfort</label>
                            <p class="text-[11px] text-brand-charcoal/60 font-light -mt-2 mb-2 leading-relaxed">
                                Because international landscapes and climate checks vary greatly, please select your comfort profile:
                            </p>
                            <div class="space-y-2">
                                <label class="flex items-start text-sm font-light text-brand-charcoal cursor-pointer">
                                    <input type="radio" name="agilityProfile" value="scenic" class="mt-1 mr-2 text-brand-forest focus:ring-brand-sage">
                                    <div>
                                        <strong class="text-xs text-brand-forest uppercase tracking-wider">The Scenic Soles (Leisurely)</strong>
                                        <p class="text-[11px] text-brand-charcoal/60 font-light">Flat, well-maintained paths, boardwalks, and short strolls under 2 miles.</p>
                                    </div>
                                </label>
                                <label class="flex items-start text-sm font-light text-brand-charcoal cursor-pointer">
                                    <input type="radio" name="agilityProfile" value="steady" class="mt-1 mr-2 text-brand-forest focus:ring-brand-sage">
                                    <div>
                                        <strong class="text-xs text-brand-forest uppercase tracking-wider">The Steady Trekkers (Moderate)</strong>
                                        <p class="text-[11px] text-brand-charcoal/60 font-light">Uneven dirt trails, moderate elevation, 3-5 miles, breaking a sweat.</p>
                                    </div>
                                </label>
                                <label class="flex items-start text-sm font-light text-brand-charcoal cursor-pointer">
                                    <input type="radio" name="agilityProfile" value="summit" class="mt-1 mr-2 text-brand-forest focus:ring-brand-sage">
                                    <div>
                                        <strong class="text-xs text-brand-forest uppercase tracking-wider">The Summit Seekers (Advanced)</strong>
                                        <p class="text-[11px] text-brand-charcoal/60 font-light">Steep technical climbs, rocky scrambles, river crossings, 6+ miles.</p>
                                    </div>
                                </label>
                                <label class="flex items-start text-sm font-light text-brand-charcoal cursor-pointer">
                                    <input type="radio" name="agilityProfile" value="mobility" class="mt-1 mr-2 text-brand-forest focus:ring-brand-sage">
                                    <div>
                                        <strong class="text-xs text-brand-forest uppercase tracking-wider">Mobility-Conscious</strong>
                                        <p class="text-[11px] text-brand-charcoal/60 font-light">Routes strictly flat, paved, or accessible for wheelchairs, strollers, etc.</p>
                                    </div>
                                </label>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- STEP 3: CULINARY ADVENTUROUSNESS & ENVIRONMENTAL COMFORT -->
                <div id="form-step-3" class="form-step hidden space-y-4">
                    <h3 class="font-serif text-lg font-bold text-brand-forest">Step 3: Culinary & Structural Style</h3>
                    
                    <div class="space-y-4">
                        <div>
                            <label class="block text-xs font-semibold uppercase tracking-wider text-brand-charcoal/80 mb-2">How would you describe your culinary adventurousness? *</label>
                            <div class="space-y-2">
                                <label class="flex items-start text-sm font-light text-brand-charcoal cursor-pointer">
                                    <input type="radio" name="culinaryStyle" value="safe" required class="mt-1 mr-2 text-brand-forest focus:ring-brand-sage">
                                    <div>
                                        <strong class="text-xs text-brand-forest uppercase tracking-wider">The Play-It-Safe Diner</strong>
                                        <p class="text-[11px] text-brand-charcoal/60 font-light">Familiar flavor profiles, well-reviewed standard restaurants, predictable spaces.</p>
                                    </div>
                                </label>
                                <label class="flex items-start text-sm font-light text-brand-charcoal cursor-pointer">
                                    <input type="radio" name="culinaryStyle" value="casual" class="mt-1 mr-2 text-brand-forest focus:ring-brand-sage">
                                    <div>
                                        <strong class="text-xs text-brand-forest uppercase tracking-wider">The Curious Casual</strong>
                                        <p class="text-[11px] text-brand-charcoal/60 font-light">Happy to try popular regional items, but lean toward highly accessible, sit-down spots.</p>
                                    </div>
                                </label>
                                <label class="flex items-start text-sm font-light text-brand-charcoal cursor-pointer">
                                    <input type="radio" name="culinaryStyle" value="explorer" class="mt-1 mr-2 text-brand-forest focus:ring-brand-sage">
                                    <div>
                                        <strong class="text-xs text-brand-forest uppercase tracking-wider">The Culinary Explorer 🌶️</strong>
                                        <p class="text-[11px] text-brand-charcoal/60 font-light">Take me to street food, night markets, and hyper-local stalls. I love trying unusual ingredients.</p>
                                    </div>
                                </label>
                                <label class="flex items-start text-sm font-light text-brand-charcoal cursor-pointer">
                                    <input type="radio" name="culinaryStyle" value="fine" class="mt-1 mr-2 text-brand-forest focus:ring-brand-sage">
                                    <div>
                                        <strong class="text-xs text-brand-forest uppercase tracking-wider">The Fine Diner</strong>
                                        <p class="text-[11px] text-brand-charcoal/60 font-light">Prioritizes Michelin stars, world-renowned chefs, tasting menus, and high-end gastronomy.</p>
                                    </div>
                                </label>
                            </div>
                        </div>

                        <div>
                            <label class="block text-xs font-semibold uppercase tracking-wider text-brand-charcoal/80 mb-2">Environmental & Structural Comfort Zone *</label>
                            <div class="space-y-2">
                                <label class="flex items-start text-sm font-light text-brand-charcoal cursor-pointer">
                                    <input type="radio" name="comfortZone" value="comfortable" required class="mt-1 mr-2 text-brand-forest focus:ring-brand-sage">
                                    <span>Keep it seamless & comfortable—I prefer curated boutique accommodations and straightforward, private transit.</span>
                                </label>
                                <label class="flex items-start text-sm font-light text-brand-charcoal cursor-pointer">
                                    <input type="radio" name="comfortZone" value="adventurous" class="mt-1 mr-2 text-brand-forest focus:ring-brand-sage">
                                    <span>I love an adventure—I'm entirely comfortable navigating local train systems, regional transit, and ferries independently.</span>
                                </label>
                                <label class="flex items-start text-sm font-light text-brand-charcoal cursor-pointer">
                                    <input type="radio" name="comfortZone" value="mixed" class="mt-1 mr-2 text-brand-forest focus:ring-brand-sage">
                                    <span>A beautiful mix—structured comfort for my base camp hotels, but fully adventurous and exploratory during the day.</span>
                                </label>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- STEP 4: SERVICE OFFERING DEEP DIVES (DYNAMICALLY ADJUSTED IN JS) -->
                <div id="form-step-4" class="form-step hidden space-y-4">
                    <h3 class="font-serif text-lg font-bold text-brand-forest">Step 4: Your Specific Tier Focus</h3>
                    
                    <!-- Dynamic Field Container (Populated by Javascript based on selected Tier) -->
                    <div id="dynamic-fields-container" class="space-y-4">
                        <!-- Content injected via showStep() -->
                    </div>
                </div>

                <!-- STEP 5: FINAL AGREEMENTS & BOUNDARIES -->
                <div id="form-step-5" class="form-step hidden space-y-4">
                    <h3 class="font-serif text-lg font-bold text-brand-forest">Step 5: Final Submission</h3>
                    
                    <div class="space-y-4">
                        <div>
                            <label class="block text-xs font-semibold uppercase tracking-wider text-brand-charcoal/80 mb-1.5">Is there anything else close to your heart that will help me make this trip an absolute masterpiece? (Optional)</label>
                            <textarea id="finalThoughts" rows="4" class="w-full p-3 bg-brand-linenDark border border-transparent focus:border-brand-sage focus:bg-white outline-none rounded-xl text-sm transition-all-300 resize-none"></textarea>
                        </div>

                        <div class="p-4 bg-brand-linenDark border border-brand-accent/20 rounded-xl space-y-3">
                            <span class="inline-block text-[10px] font-semibold uppercase tracking-widest text-brand-accent">Retainer & Timeline Acknowledgment</span>
                            <label class="flex items-start text-xs font-light text-brand-charcoal/90 cursor-pointer leading-relaxed">
                                <input type="checkbox" id="retainerAgreement" required class="mt-1 mr-2.5 rounded border-gray-300 text-brand-forest focus:ring-brand-sage">
                                <span>I understand that upon submitting this discovery form, an electronic invoice for my selected planning tier will be delivered to my email. Once payment is securely processed, work on my custom travel blueprint or research dossier will begin, with a standard turnaround time of 5-7 business days. *</span>
                            </label>
                        </div>
                    </div>
                </div>

                <!-- NAVIGATION BUTTON PANEL -->
                <div class="flex items-center justify-between pt-4 border-t border-brand-linenDark">
                    <button type="button" id="prevBtn" onclick="prevStep()" class="px-5 py-2.5 text-xs font-semibold uppercase tracking-wider text-brand-sage hover:text-brand-forest invisible transition-all-300">
                        Back
                    </button>
                    <button type="button" id="nextBtn" onclick="nextStep()" class="px-6 py-3 text-xs font-semibold uppercase tracking-wider bg-brand-forest hover:bg-brand-forestLight text-white rounded-xl transition-all-300 shadow">
                        Continue
                    </button>
                    <button type="submit" id="submitBtn" class="px-6 py-3 text-xs font-semibold uppercase tracking-wider bg-brand-accent hover:bg-brand-accent/80 text-brand-forest rounded-xl transition-all-300 shadow hidden">
                        Submit Blueprint Request
                    </button>
                </div>

            </form>

            <!-- Success Portal Overlay (Hidden unless submitted) -->
            <div id="success-portal" class="absolute inset-0 bg-white rounded-2xl flex flex-col items-center justify-center text-center p-8 hidden z-10">
                <div class="w-16 h-16 bg-brand-linenDark rounded-full flex items-center justify-center text-brand-accent mb-4">
                    <svg class="w-8 h-8" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5" d="M5 13l4 4L19 7"/></svg>
                </div>
                <h3 class="font-serif text-2xl font-bold text-brand-forest mb-2">Discovery Plan Submitted</h3>
                <p class="text-sm text-brand-charcoal/80 max-w-sm mx-auto font-light leading-relaxed mb-6">
                    Your details have been successfully locked into our secure system. Your digital retainer invoice will land in your inbox shortly.
                </p>
                <div class="p-4 bg-brand-linenDark rounded-xl text-left text-xs max-w-xs space-y-2 mb-6 font-light">
                    <p class="font-bold text-brand-forest uppercase tracking-wider text-[9px]">Timeline Tracker:</p>
                    <p>• Retainer Invoice sent via email.</p>
                    <p>• Blueprint design begins upon payment.</p>
                    <p>• Final dossier delivery: 5-7 business days.</p>
                </div>
                <button onclick="resetDiscoveryForm()" class="px-5 py-2.5 text-xs font-semibold uppercase tracking-wider text-brand-forest bg-brand-linenDark hover:bg-brand-forest hover:text-white rounded-lg transition-all-300">
                    Return to Hub
                </button>
            </div>

        </div>

        <!-- TAB 4: ABOUT ME & TRAVEL ART -->
        <div id="view-about" class="tab-view hidden space-y-6">
            <!-- Biography Card -->
            <div class="bg-white border border-brand-linenDark p-6 rounded-2xl shadow-sm space-y-4">
                <h3 class="font-serif text-2xl font-bold text-brand-forest">Meet Your Travel Architect</h3>
                
                <p class="text-sm font-light text-brand-charcoal/90 leading-relaxed italic">
                    An exceptional travel experience is born from the tension between raw adventure and meticulous design. It requires a planner who looks past generic, glossy brochures and instead understands how to read a landscape, decode unpredictable infrastructure, and engage intentionally with local community networks.
                </p>
                
                <p class="text-sm font-light text-brand-charcoal/90 leading-relaxed">
                    My career has been defined by the art of <strong class="text-brand-forest">curation</strong>. As a multidisciplinary artist and educator, I have spent years exploring the intersection of visual storytelling, global connectivity, and geographic navigation. In the art world, curation is about selecting, organizing, and presenting elements to tell a profound, cohesive story. In high-end travel design, I apply that exact same artistic lens. I do not just book trips; I <strong class="text-brand-forest">curate</strong> immersive, sensory, and highly intentional environments for you to experience.
                </p>
                
                <p class="text-sm font-light text-brand-charcoal/90 leading-relaxed">
                    My design philosophy is built from firsthand, real-world experience navigating diverse international terrains—from the dense canopy systems of Central America to complex, transit-heavy urban landscapes. Having mapped out and executed deep-dive family travels and eco-conscious expeditions across the globe, I launched **The Conscious Compass Travel Co.** to provide travelers with an entirely new standard of travel intelligence.
                </p>

                <!-- Personal Dietary Callout -->
                <div class="bg-brand-linen p-4 rounded-xl border border-brand-linenDark space-y-1">
                    <span class="inline-block text-[10px] font-semibold uppercase tracking-widest text-brand-accent">Specialized Authority</span>
                    <h5 class="text-xs font-semibold text-brand-forest uppercase tracking-wider">Uncompromised Dietary Curation</h5>
                    <p class="text-xs text-brand-charcoal/80 font-light leading-relaxed">
                        As a family that travels the world on a strictly vegan and gluten-free framework, I navigate the hyper-vigilance of cross-contamination protocols firsthand. I curate your dining layouts with the exact same uncompromised standards I use to protect my own family.
                    </p>
                </div>
            </div>

            <!-- Stylized Portfolio / Travel Art print directory -->
            <div class="space-y-4">
                <div class="text-center">
                    <h4 class="font-serif text-lg font-bold text-brand-forest">Fine Art Prints & Landscape Logs</h4>
                    <p class="text-xs text-brand-charcoal/60 font-light">Select portfolios captured on-site. Click any piece to acquire a fine art print.</p>
                </div>

                <div class="grid grid-cols-2 gap-4">
                    <!-- Photo Card 1 -->
                    <a href="https://your-print-shop-link.com" target="_blank" class="group block relative rounded-xl overflow-hidden shadow-sm aspect-video bg-brand-forest">
                        <!-- Image with fallback -->
                        <img src="gallery1.jpg" 
                             onerror="this.src='https://images.unsplash.com/photo-1516026672322-bc52d61a55d5?auto=format&fit=crop&w=400&q=85'" 
                             alt="Cloud Canopies" 
                             class="w-full h-full object-cover transition-all-300 group-hover:scale-105">
                        <div class="absolute inset-0 bg-brand-forestLight/30 group-hover:bg-brand-forestLight/60 transition-all-300 flex flex-col justify-end p-3">
                            <span class="text-white font-serif italic text-xs block truncate mb-1">I. Cloud Canopies</span>
                            <span class="text-[9px] text-brand-accent uppercase tracking-widest font-semibold bg-brand-forest/80 px-2 py-0.5 rounded self-start opacity-0 group-hover:opacity-100 transition-all-300">Purchase Fine Art Print ↗</span>
                        </div>
                    </a>
                    
                    <!-- Photo Card 2 -->
                    <a href="https://your-print-shop-link.com" target="_blank" class="group block relative rounded-xl overflow-hidden shadow-sm aspect-video bg-brand-sage">
                        <img src="gallery2.jpg" 
                             onerror="this.src='https://images.unsplash.com/photo-1464822759023-fed622ff2c3b?auto=format&fit=crop&w=400&q=85'" 
                             alt="Mountain Corridors" 
                             class="w-full h-full object-cover transition-all-300 group-hover:scale-105">
                        <div class="absolute inset-0 bg-brand-forest/30 group-hover:bg-brand-forest/60 transition-all-300 flex flex-col justify-end p-3">
                            <span class="text-white font-serif italic text-xs block truncate mb-1">II. Mountain Corridors</span>
                            <span class="text-[9px] text-brand-accent uppercase tracking-widest font-semibold bg-brand-forest/80 px-2 py-0.5 rounded self-start opacity-0 group-hover:opacity-100 transition-all-300">Purchase Fine Art Print ↗</span>
                        </div>
                    </a>

                    <!-- Photo Card 3 -->
                    <a href="https://your-print-shop-link.com" target="_blank" class="group block relative rounded-xl overflow-hidden shadow-sm aspect-video bg-brand-charcoal">
                        <img src="gallery3.jpg" 
                             onerror="this.src='https://images.unsplash.com/photo-1513519245088-0e12902e5a38?auto=format&fit=crop&w=400&q=85'" 
                             alt="Artisan Guilds" 
                             class="w-full h-full object-cover transition-all-300 group-hover:scale-105">
                        <div class="absolute inset-0 bg-brand-forestLight/30 group-hover:bg-brand-forestLight/60 transition-all-300 flex flex-col justify-end p-3">
                            <span class="text-white font-serif italic text-xs block truncate mb-1">III. Artisan Guilds</span>
                            <span class="text-[9px] text-brand-accent uppercase tracking-widest font-semibold bg-brand-forest/80 px-2 py-0.5 rounded self-start opacity-0 group-hover:opacity-100 transition-all-300">Purchase Fine Art Print ↗</span>
                        </div>
                    </a>

                    <!-- Photo Card 4 -->
                    <a href="https://your-print-shop-link.com" target="_blank" class="group block relative rounded-xl overflow-hidden shadow-sm aspect-video bg-brand-accent">
                        <img src="gallery4.jpg" 
                             onerror="this.src='https://images.unsplash.com/photo-1505118380757-91f5f5632de0?auto=format&fit=crop&w=400&q=85'" 
                             alt="Coastal Horizons" 
                             class="w-full h-full object-cover transition-all-300 group-hover:scale-105">
                        <div class="absolute inset-0 bg-brand-forest/20 group-hover:bg-brand-forest/50 transition-all-300 flex flex-col justify-end p-3">
                            <span class="text-brand-forest font-serif italic text-xs block truncate mb-1">IV. Coastal Horizons</span>
                            <span class="text-[9px] text-brand-forest uppercase tracking-widest font-semibold bg-brand-linenDark px-2 py-0.5 rounded self-start opacity-0 group-hover:opacity-100 transition-all-300">Purchase Fine Art Print ↗</span>
                        </div>
                    </a>
                </div>
            </div>
        </div>

        <!-- TAB 5: STRATEGIC FAQs -->
        <div id="view-faq" class="tab-view hidden space-y-4">
            <div class="text-center max-w-md mx-auto mb-6">
                <h3 class="font-serif text-2xl font-bold text-brand-forest">Strategic Intelligence</h3>
                <p class="text-xs text-brand-charcoal/60 mt-1 font-light">Disarming friction, protecting boundaries, and defining value.</p>
            </div>

            <!-- Accordion FAQ 1 -->
            <div class="bg-white border border-brand-linenDark rounded-xl overflow-hidden shadow-sm transition-all-300">
                <button onclick="toggleAccordion('faq-1')" class="w-full text-left p-4 flex items-center justify-between focus:outline-none bg-white hover:bg-brand-linenDark">
                    <span class="text-sm font-semibold text-brand-forest">Why pay a planning fee when I can book myself or use an agent for free?</span>
                    <svg id="icon-faq-1" class="w-4 h-4 text-brand-sage transform transition-transform duration-300" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7"/></svg>
                </button>
                <div id="content-faq-1" class="max-h-0 overflow-hidden transition-all duration-300 ease-in-out">
                    <p class="p-4 text-xs font-light text-brand-charcoal/85 leading-relaxed bg-brand-linen border-t border-brand-linenDark">
                        Traditional agents survive on backend commissions, meaning their suggestions often skew toward generic resort networks that match standard payout frameworks. We operate entirely independent of commissions. You are paying for custom curation, deep international logistical vetting, and complete spatial authority. Our recommendations are driven strictly by your specific safety, comfort, and culinary profiles.
                    </p>
                </div>
            </div>

            <!-- Accordion FAQ 2 -->
            <div class="bg-white border border-brand-linenDark rounded-xl overflow-hidden shadow-sm transition-all-300">
                <button onclick="toggleAccordion('faq-2')" class="w-full text-left p-4 flex items-center justify-between focus:outline-none bg-white hover:bg-brand-linenDark">
                    <span class="text-sm font-semibold text-brand-forest">Since you are a design-only planner, how do bookings get made?</span>
                    <svg id="icon-faq-2" class="w-4 h-4 text-brand-sage transform transition-transform duration-300" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7"/></svg>
                </button>
                <div id="content-faq-2" class="max-h-0 overflow-hidden transition-all duration-300 ease-in-out">
                    <p class="p-4 text-xs font-light text-brand-charcoal/85 leading-relaxed bg-brand-linen border-t border-brand-linenDark">
                        We map the blueprint; you execute the bookings. Your completed dossier contains direct, vetted reservation links for all curated accommodations, transit networks, and excursions. This puts you in absolute control over your private travel dates, rewards points, and direct vendor cancellation parameters with zero hidden markups.
                    </p>
                </div>
            </div>

            <!-- Accordion FAQ 3 -->
            <div class="bg-white border border-brand-linenDark rounded-xl overflow-hidden shadow-sm transition-all-300">
                <button onclick="toggleAccordion('faq-3')" class="w-full text-left p-4 flex items-center justify-between focus:outline-none bg-white hover:bg-brand-linenDark">
                    <span class="text-sm font-semibold text-brand-forest">What happens if a flight gets delayed or cancelled?</span>
                    <svg id="icon-faq-3" class="w-4 h-4 text-brand-sage transform transition-transform duration-300" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7"/></svg>
                </button>
                <div id="content-faq-3" class="max-h-0 overflow-hidden transition-all duration-300 ease-in-out">
                    <p class="p-4 text-xs font-light text-brand-charcoal/85 leading-relaxed bg-brand-linen border-t border-brand-linenDark">
                        Because we are a design and research dossier service, contracts for your stays are directly held between you and the respective providers. While we do not provide 24/7 in-trip rebooking, your custom blueprint is built with high time tolerances to absorb delays, and we supply explicit local alternative routes and emergency details directly inside your dossier for immediate self-navigation.
                    </p>
                </div>
            </div>

            <!-- Accordion FAQ 4 -->
            <div class="bg-white border border-brand-linenDark rounded-xl overflow-hidden shadow-sm transition-all-300">
                <button onclick="toggleAccordion('faq-4')" class="w-full text-left p-4 flex items-center justify-between focus:outline-none bg-white hover:bg-brand-linenDark">
                    <span class="text-sm font-semibold text-brand-forest">I have strict dietary boundaries. Can you safely accommodate me?</span>
                    <svg id="icon-faq-4" class="w-4 h-4 text-brand-sage transform transition-transform duration-300" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7"/></svg>
                </button>
                <div id="content-faq-4" class="max-h-0 overflow-hidden transition-all duration-300 ease-in-out">
                    <p class="p-4 text-xs font-light text-brand-charcoal/85 leading-relaxed bg-brand-linen border-t border-brand-linenDark">
                        Uncompromised dietary vetting is one of our primary specialties. My family navigates a strict, dual-layer vegan and gluten-free framework on international journeys. We do not trust arbitrary blog recommendations. We analyze regional ingredients, contact kitchen frameworks, and identify rooms with dedicated private kitchenettes so you can travel without culinary anxiety.
                    </p>
                </div>
            </div>
        </div>

    </main>

    <!-- Footer Branding -->
    <footer class="w-full text-center py-8 border-t border-brand-linenDark mt-12 bg-white text-xs font-light text-brand-charcoal/60">
        <div class="max-w-2xl mx-auto px-4 space-y-2">
            <p class="font-serif italic text-brand-forest text-sm font-medium">The Conscious Compass Travel Co.</p>
            <p>Intentional • Eco-Conscious • Immersive</p>
            <p class="text-[10px] text-brand-charcoal/40 mt-4">&copy; 2026 The Conscious Compass. All rights reserved.</p>
        </div>
    </footer>

    <!-- Javascript Engine -->
    <script>
        // Tab Navigation State
        function switchTab(tabId) {
            // Hide all tab content
            document.querySelectorAll('.tab-view').forEach(view => {
                view.classList.add('hidden');
            });
            // Reset active style on buttons
            document.querySelectorAll('.tab-btn').forEach(btn => {
                btn.className = "tab-btn flex-1 py-2 px-3 rounded-lg text-center transition-all-300 text-brand-forest hover:bg-brand-linen/60";
            });

            // Show selected content
            const activeView = document.getElementById('view-' + tabId);
            if (activeView) activeView.classList.remove('hidden');

            // Set active style on button
            const activeBtn = document.getElementById('tab-' + tabId);
            if (activeBtn) activeBtn.className = "tab-btn flex-1 py-2 px-3 rounded-lg text-center transition-all-300 bg-brand-forest text-white shadow-sm";

            // If entering intake tab, initialize first step
            if (tabId === 'intake') {
                showStep(currentStep);
            }

            // Scroll to tab bar on mobile
            window.scrollTo({ top: 120, behavior: 'smooth' });
        }

        // Accordion Toggle States
        function toggleAccordion(faqId) {
            const content = document.getElementById('content-' + faqId);
            const icon = document.getElementById('icon-' + faqId);

            if (content.style.maxHeight && content.style.maxHeight !== '0px') {
                content.style.maxHeight = '0px';
                icon.style.transform = 'rotate(0deg)';
            } else {
                // Close any open ones first
                document.querySelectorAll('[id^="content-faq-"]').forEach(el => {
                    el.style.maxHeight = '0px';
                });
                document.querySelectorAll('[id^="icon-faq-"]').forEach(el => {
                    el.style.transform = 'rotate(0deg)';
                });

                // Open selected
                content.style.maxHeight = content.scrollHeight + 'px';
                icon.style.transform = 'rotate(180deg)';
            }
        }

        // Discovery Form Multi-step State
        let currentStep = 1;
        const totalSteps = 5;

        function showStep(step) {
            // Clear any old error state on load
            const errorBox = document.getElementById('error-alert-box');
            errorBox.classList.add('hidden');

            // Hide all steps
            document.querySelectorAll('.form-step').forEach(el => el.classList.add('hidden'));
            
            // Show current step
            document.getElementById('form-step-' + step).classList.remove('hidden');

            // Update Progress UI Indicators
            document.getElementById('step-indicator').textContent = `Step ${step} of ${totalSteps}`;
            document.getElementById('step-progress').style.width = `${(step / totalSteps) * 100}%`;

            // Adjust buttons visibility
            const prevBtn = document.getElementById('prevBtn');
            const nextBtn = document.getElementById('nextBtn');
            const submitBtn = document.getElementById('submitBtn');

            if (step === 1) {
                prevBtn.classList.add('invisible');
            } else {
                prevBtn.classList.remove('invisible');
            }

            if (step === totalSteps) {
                nextBtn.classList.add('hidden');
                submitBtn.classList.remove('hidden');
            } else {
                nextBtn.classList.remove('hidden');
                submitBtn.classList.add('hidden');
            }

            // Execute conditional dynamic fields injection in Step 4
            if (step === 4) {
                injectDynamicFields();
            }
        }

        function nextStep() {
            if (validateStep(currentStep)) {
                if (currentStep < totalSteps) {
                    currentStep++;
                    showStep(currentStep);
                }
            }
        }

        function prevStep() {
            if (currentStep > 1) {
                currentStep--;
                showStep(currentStep);
            }
        }

        // Show inline alerts instead of browser alert() boxes
        function showFormError(message) {
            const errorBox = document.getElementById('error-alert-box');
            const errorMsg = document.getElementById('error-alert-message');
            errorMsg.textContent = message;
            errorBox.classList.remove('hidden');
            window.scrollTo({ top: 120, behavior: 'smooth' });
        }

        // Validate individual steps prior to advancing
        function validateStep(step) {
            const currentStepEl = document.getElementById('form-step-' + step);
            const inputs = currentStepEl.querySelectorAll('input[required], select[required], textarea[required]');
            let isValid = true;

            // Clear any previous inputs highlighted in red
            currentStepEl.querySelectorAll('.border-red-400').forEach(input => {
                input.classList.remove('border-red-400');
            });

            inputs.forEach(input => {
                if (input.type === 'radio') {
                    // Check if at least one radio of the group is checked
                    const name = input.name;
                    const checkedRadio = currentStepEl.querySelector(`input[name="${name}"]:checked`);
                    if (!checkedRadio) {
                        isValid = false;
                        input.focus();
                    }
                } else if (!input.value.trim()) {
                    isValid = false;
                    input.classList.add('border-red-400');
                    input.focus();
                }
            });

            // If a required element failed basic criteria
            if (!isValid) {
                showFormError('Please fill out all required fields marked with an asterisk (*) to continue.');
                return false;
            }

            // Validate Step 2 Vibe Checkboxes (Choose up to 2)
            if (step === 2) {
                const checkedBoxes = currentStepEl.querySelectorAll('input[name="vibeFocus"]:checked');
                if (checkedBoxes.length === 0) {
                    showFormError('Please select at least one primary trip energy focus.');
                    return false;
                } else if (checkedBoxes.length > 2) {
                    showFormError('Please select a maximum of 2 primary trip energies to keep your focus curated.');
                    return false;
                }
            }

            return true;
        }

        // Conditional Logic: Party Dynamics
        function toggleChildrenInput() {
            const partyType = document.getElementById('partyType').value;
            const container = document.getElementById('childrenAgesContainer');
            if (partyType === 'family') {
                container.classList.remove('hidden');
            } else {
                container.classList.add('hidden');
            }
        }

        // Conditional Logic: Active exploration physical check
        function togglePhysicalAgilityQuestion() {
            const checkbox = document.getElementById('activeAdventureCheckbox');
            const container = document.getElementById('physicalAgilityContainer');
            
            if (checkbox.checked) {
                container.classList.remove('hidden');
                // Make the radio fields required
                container.querySelectorAll('input[type="radio"]').forEach(radio => {
                    radio.required = true;
                });
            } else {
                container.classList.add('hidden');
                container.querySelectorAll('input[type="radio"]').forEach(radio => {
                    radio.required = false;
                    radio.checked = false;
                });
            }
        }

        // Strategic Conditional Logic: Inject fields into Step 4 based on Tier Selected in Step 1
        function injectDynamicFields() {
            const selectedTier = document.getElementById('selectedTier').value;
            const container = document.getElementById('dynamic-fields-container');
            container.innerHTML = ''; // reset

            if (selectedTier === 'tier1') {
                container.innerHTML = `
                    <div class="space-y-4">
                        <span class="inline-block text-[10px] font-semibold uppercase tracking-widest text-brand-sage bg-brand-linenDark px-2 py-1 rounded">Tier 1 Target Fields</span>
                        <div>
                            <label class="block text-xs font-semibold uppercase tracking-wider text-brand-charcoal/80 mb-2">What are the top 3 friction points keeping you up at night? *</label>
                            <div class="space-y-2 text-sm font-light">
                                <label class="flex items-center cursor-pointer"><input type="checkbox" name="tier1Friction" value="transit" class="mr-2 rounded border-gray-300 text-brand-forest focus:ring-brand-sage"> Navigating public transit, rail, or regional ferries</label>
                                <label class="flex items-center cursor-pointer"><input type="checkbox" name="tier1Friction" value="bureaucracy" class="mr-2 rounded border-gray-300 text-brand-forest focus:ring-brand-sage"> Visas, passports, entry protocols, & compliance</label>
                                <label class="flex items-center cursor-pointer"><input type="checkbox" name="tier1Friction" value="safety" class="mr-2 rounded border-gray-300 text-brand-forest focus:ring-brand-sage"> Neighborhood safety, local scams, and solo security</label>
                                <label class="flex items-center cursor-pointer"><input type="checkbox" name="tier1Friction" value="packing" class="mr-2 rounded border-gray-300 text-brand-forest focus:ring-brand-sage"> Correct gear and cultural dress codes for variable terrain</label>
                                <label class="flex items-center cursor-pointer"><input type="checkbox" name="tier1Friction" value="sustainability" class="mr-2 rounded border-gray-300 text-brand-forest focus:ring-brand-sage"> Sourcing certified eco-tours or local artisans</label>
                            </div>
                        </div>
                        <div>
                            <label class="block text-xs font-semibold uppercase tracking-wider text-brand-charcoal/80 mb-1.5">Describe your specific anxieties or excitement for this destination: *</label>
                            <textarea id="tier1Anxieties" required rows="3" placeholder="e.g. Navigating trains with luggage, finding safe areas in the evening..." class="w-full p-3 bg-brand-linenDark border border-transparent focus:border-brand-sage focus:bg-white outline-none rounded-xl text-sm transition-all-300 resize-none"></textarea>
                        </div>
                    </div>
                `;
            } else if (selectedTier === 'tier2') {
                container.innerHTML = `
                    <div class="space-y-4">
                        <span class="inline-block text-[10px] font-semibold uppercase tracking-widest text-brand-sage bg-brand-linenDark px-2 py-1 rounded">Tier 2 Target Fields</span>
                        <div>
                            <label class="block text-xs font-semibold uppercase tracking-wider text-brand-charcoal/80 mb-1.5">How many active days do you need us to surgically design? * (2-Day Minimum)</label>
                            <input type="number" id="tier2Days" required min="2" max="30" class="w-full p-3 bg-brand-linenDark border border-transparent focus:border-brand-sage focus:bg-white outline-none rounded-xl text-sm transition-all-300">
                        </div>
                        <div>
                            <label class="block text-xs font-semibold uppercase tracking-wider text-brand-charcoal/80 mb-1.5">Please describe the specific dates or portions of the trip we are taking over: *</label>
                            <textarea id="tier2Description" required rows="3" placeholder="e.g. Days 3, 4, & 5 while we are traveling between region hubs..." class="w-full p-3 bg-brand-linenDark border border-transparent focus:border-brand-sage focus:bg-white outline-none rounded-xl text-sm transition-all-300 resize-none"></textarea>
                        </div>
                        <div>
                            <label class="block text-xs font-semibold uppercase tracking-wider text-brand-charcoal/80 mb-1.5">What do you already have booked for these specific days?</label>
                            <textarea id="tier2Bookings" rows="3" placeholder="e.g. Mountain Eco-Lodge is booked, arriving via train at 2pm..." class="w-full p-3 bg-brand-linenDark border border-transparent focus:border-brand-sage focus:bg-white outline-none rounded-xl text-sm transition-all-300 resize-none"></textarea>
                        </div>
                        <div>
                            <label class="block text-xs font-semibold uppercase tracking-wider text-brand-charcoal/80 mb-1.5">Do you have specific dietary boundaries or allergies I should keep in mind for these days?</label>
                            <input type="text" id="tier2Dietary" placeholder="e.g. Vegan, Celiac-safe, none" class="w-full p-3 bg-brand-linenDark border border-transparent focus:border-brand-sage focus:bg-white outline-none rounded-xl text-sm transition-all-300">
                        </div>
                    </div>
                `;
            } else if (selectedTier === 'tier3') {
                container.innerHTML = `
                    <div class="space-y-4">
                        <span class="inline-block text-[10px] font-semibold uppercase tracking-widest text-brand-sage bg-brand-linenDark px-2 py-1 rounded">Tier 3 Target Fields</span>
                        <div>
                            <label class="block text-xs font-semibold uppercase tracking-wider text-brand-charcoal/80 mb-1.5">Estimated Total Budget * (Excluding design fee)</label>
                            <select id="tier3Budget" required class="w-full p-3 bg-brand-linenDark border border-transparent focus:border-brand-sage focus:bg-white outline-none rounded-xl text-sm transition-all-300">
                                <option value="3k-5k">$3,000 – $5,000</option>
                                <option value="5k-10k">$5,000 – $10,000</option>
                                <option value="10k-15k">$10,000 – $15,000</option>
                                <option value="15k+">$15,000+</option>
                            </select>
                        </div>
                        <div>
                            <label class="block text-xs font-semibold uppercase tracking-wider text-brand-charcoal/80 mb-1.5">What is your travel pacing preference? *</label>
                            <select id="tier3Pacing" required class="w-full p-3 bg-brand-linenDark border border-transparent focus:border-brand-sage focus:bg-white outline-none rounded-xl text-sm transition-all-300">
                                <option value="slow">Slow & Immersive (Unpack once, slow cultural absorption)</option>
                                <option value="balanced">Balanced (Structured mornings, spontaneous open afternoons)</option>
                                <option value="dynamic">Dynamic Explorer (Moving hubs and hotels every 2-3 days)</option>
                            </select>
                        </div>
                        <div>
                            <label class="block text-xs font-semibold uppercase tracking-wider text-brand-charcoal/80 mb-2">Dietary Restrictions & Accommodations (Check all that apply)</label>
                            <div class="space-y-1 text-sm font-light">
                                <label class="flex items-center cursor-pointer"><input type="checkbox" name="tier3Dietary" value="vegetarian" class="mr-2 rounded border-gray-300 text-brand-forest focus:ring-brand-sage"> Vegetarian</label>
                                <label class="flex items-center cursor-pointer"><input type="checkbox" name="tier3Dietary" value="vegan" class="mr-2 rounded border-gray-300 text-brand-forest focus:ring-brand-sage"> Vegan</label>
                                <label class="flex items-center cursor-pointer"><input type="checkbox" name="tier3Dietary" value="celiac" class="mr-2 rounded border-gray-300 text-brand-forest focus:ring-brand-sage"> Gluten-Free / Celiac</label>
                                <label class="flex items-center cursor-pointer"><input type="checkbox" name="tier3Dietary" value="allergies" id="tier3AllergiesCheckbox" onchange="toggleAllergiesSpecifyInput()" class="mr-2 rounded border-gray-300 text-brand-forest focus:ring-brand-sage"> Severe Food Allergies</label>
                            </div>
                        </div>
                        <div id="allergiesSpecifyContainer" class="hidden">
                            <label class="block text-xs font-semibold uppercase tracking-wider text-brand-charcoal/80 mb-1.5">Please specify all severe allergies:</label>
                            <input type="text" id="tier3AllergiesSpecify" placeholder="e.g. Peanuts, Dairy" class="w-full p-3 bg-brand-linenDark border border-transparent focus:border-brand-sage focus:bg-white outline-none rounded-xl text-sm transition-all-300">
                        </div>
                        <div>
                            <label class="block text-xs font-semibold uppercase tracking-wider text-brand-charcoal/80 mb-2">How strictly do these dietary needs affect lodging? *</label>
                            <div class="space-y-2 text-sm font-light">
                                <label class="flex items-start cursor-pointer">
                                    <input type="radio" name="tier3AccommodationImpact" value="basic" required class="mt-1 mr-2 text-brand-forest focus:ring-brand-sage">
                                    <span>Only restaurants—the hotels themselves just need a basic heads-up.</span>
                                </label>
                                <label class="flex items-start cursor-pointer">
                                    <input type="radio" name="tier3AccommodationImpact" value="critical" class="mt-1 mr-2 text-brand-forest focus:ring-brand-sage">
                                    <span>Critical—we require hotels with dedicated cross-contamination-free kitchens, or boutique rooms with private kitchenettes to prepare safe meals.</span>
                                </label>
                            </div>
                        </div>
                        <div>
                            <label class="block text-xs font-semibold uppercase tracking-wider text-brand-charcoal/80 mb-1.5">Are there any absolute deal-breakers or must-haves? *</label>
                            <textarea id="tier3Dealbreakers" required rows="3" placeholder="e.g. Eco-certified properties only, absolutely no small planes..." class="w-full p-3 bg-brand-linenDark border border-transparent focus:border-brand-sage focus:bg-white outline-none rounded-xl text-sm transition-all-300 resize-none"></textarea>
                        </div>
                    </div>
                `;
            }
        }

        // Tier 3 Allergies helper
        function toggleAllergiesSpecifyInput() {
            const checkbox = document.getElementById('tier3AllergiesCheckbox');
            const container = document.getElementById('allergiesSpecifyContainer');
            if (checkbox && checkbox.checked) {
                container.classList.remove('hidden');
            } else if (container) {
                container.classList.add('hidden');
                document.getElementById('tier3AllergiesSpecify').value = '';
            }
        }

        // Launch Form directly pre-selecting a tier
        function startIntakeWithTier(tierValue) {
            switchTab('intake');
            document.getElementById('selectedTier').value = tierValue;
        }

        // Form Submit Actions
        function handleFormSubmission(event) {
            event.preventDefault();
            
            // Clear any old error alert boxes on submit attempt
            document.getElementById('error-alert-box').classList.add('hidden');

            // Validate step 5
            const agreement = document.getElementById('retainerAgreement');
            if (!agreement.checked) {
                showFormError('You must acknowledge the Retainer & Timeline parameters before submitting.');
                return;
            }
function resetDiscoveryForm() {
            // Reset state
            document.getElementById('discoveryForm').reset();
            currentStep = 1;
            
            // Hide portal
            document.getElementById('success-portal').classList.add('hidden');
            
            // Return to Hub Links Tab
            switchTab('links');
        }
    </script>
</body>
</html>
            // Show Custom Success portal
            document.getElementById('success-portal').classList.remove('hidden');
        }

        // Form Reset Actions
