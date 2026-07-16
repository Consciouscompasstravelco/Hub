<!DOCTYPE html>
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
        }
        h1, h2, h3, .serif {
            font-family: 'Playfair Display', serif;
        }
    </style>
</head>
<body class="min-h-screen flex flex-col justify-between selection:bg-orange-100">

    <!-- Elegant Text Branding (Sits cleanly above the banner) -->
    <header class="py-8 px-4 text-center max-w-4xl mx-auto">
        <h1 class="text-3xl md:text-5xl font-semibold tracking-widest text-[#3D4035] uppercase">
            The Conscious Compass
        </h1>
        <p class="text-xs md:text-sm tracking-[0.25em] text-[#8C7A6B] uppercase mt-3 font-semibold">
            Travel Co. • Artistry & Curated Journeys
        </p>
    </header>

    <main class="w-full max-w-4xl mx-auto px-4 pb-16 flex-grow">
        <!-- Landscape Watercolor Banner Block -->
        <div class="relative w-full aspect-[21/9] rounded-2xl overflow-hidden shadow-sm bg-stone-100 border border-stone-200/40">
            <img id="banner" src="landscape.jpg" alt="Rainforest Canopy Artistry" class="w-full h-full object-cover object-[50%_40%] transition-opacity duration-500 opacity-0" onload="this.classList.remove('opacity-0')">
            
            <!-- Safe Fallback: If you haven't uploaded landscape.jpg yet, this ensures the page doesn't look broken -->
            <script>
                document.getElementById('banner').onerror = function() {
                    this.src = "https://images.unsplash.com/photo-1516026672322-bc52d61a55d5?auto=format&fit=crop&w=1200&q=80";
                };
            </script>
        </div>

        <!-- Artistic Philosophy Intro -->
        <div class="mt-12 text-center max-w-2xl mx-auto">
            <h2 class="text-2xl md:text-3xl font-medium text-[#4E5142] italic leading-relaxed">
                "We travel not to escape life, but for life not to escape us."
            </h2>
            <p class="text-sm md:text-base text-stone-600 leading-relaxed mt-6">
                Welcome. I curate slow, immersive, and sensory travel blueprints with an artist's lens. Specializing in rainforest sanctuaries, uncompromised vegan and gluten-free dietary safety, and river voyages, every detail is handled with absolute care.
            </p>
        </div>

        <!-- Multi-Step Discover Form Container -->
        <section class="mt-16 bg-white/60 backdrop-blur-md border border-stone-200/50 rounded-3xl p-6 md:p-10 shadow-sm max-w-2xl mx-auto">
            <h3 class="text-2xl font-semibold text-[#3D4035] text-center mb-2">Begin Your Journey</h3>
            <p class="text-xs text-stone-500 text-center mb-8">Fill out our Discover Form below to start planning your bespoke itinerary.</p>

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
                        <input type="text" name="destination" required class="w-full px-4 py-3 rounded-xl border border-stone-200 focus:border-[#8C7A6B] focus:ring-1 focus:ring-[#8C7A6B] outline-none bg-stone-50/50 text-sm transition" placeholder="e.g. Costa Rica Canopy, Colombia Highlands">
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
                        <label class="block text-xs font-semibold tracking-wider text-stone-600 uppercase mb-1">Dietary & Safety Priorities</label>
                        <textarea name="dietary" rows="3" class="w-full px-4 py-3 rounded-xl border border-stone-200 focus:border-[#8C7A6B] focus:ring-1 focus:ring-[#8C7A6B] outline-none bg-stone-50/50 text-sm transition" placeholder="e.g., Strict vegan & gluten-free food tracking, slow pace, specific physical parameters..."></textarea>
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

    <!-- Form Submit Handler Script -->
    <script>
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
