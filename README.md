<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>RF Designs — Interior Architecture Studio</title>
    <meta name="description" content="RF Designs is an elite interior architecture studio crafting quietly extraordinary residences and workplaces. Warm minimalism, precise materiality, and enduring calm." />

    <!-- Tailwind (CDN) -->
    <script src="https://cdn.tailwindcss.com"></script>

    <!-- Fonts: Cormorant Garamond (serif headlines) + Inter (neutral text) -->
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@400;500;600;700&family=Inter:wght@300;400;500;600&display=swap" rel="stylesheet" />

    <style>
        :root {
            color-scheme: light;
            --bg-beige: #F7F4EF;
            --bg-paper: #FFFCF9;
            --charcoal: #1F1F1F;
            --charcoal-2: #2A2A2A;
            --muted: #6B665F;
            --gold: #C9A86A;
            --gold-2: #DCC6A0;
            --line: #E8E2D9;
        }
        html { scroll-behavior: smooth; }
        body {
            font-family: 'Inter', system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
            background: var(--bg-beige);
            color: var(--charcoal-2);
            -webkit-font-smoothing: antialiased;
            -moz-osx-font-smoothing: grayscale;
            text-rendering: optimizeLegibility;
        }
        .serif { font-family: "Cormorant Garamond", Georgia, "Times New Roman", serif; }
        /* Subtle paper texture for the showcase frame */
        .paper-texture {
            background-image:
                radial-gradient(1200px 600px at 80% -10%, rgba(201,168,106,0.06), transparent 60%),
                radial-gradient(800px 400px at 10% 110%, rgba(30,30,30,0.04), transparent 50%),
                linear-gradient(0deg, rgba(0,0,0,0.015) 1px, transparent 1px);
            background-size: auto, auto, 100% 24px;
        }
        /* Gold focus ring that doesn't fight the minimal aesthetic */
        .focus-gold:focus {
            outline: none;
            border-color: var(--gold) !important;
            box-shadow: 0 0 0 3px rgba(201,168,106,0.18);
        }
        /* Soft, editorial link underline */
        .link-underline {
            background-image: linear-gradient(transparent calc(100% - 1px), rgba(201,168,106,0.45) 1px);
            background-repeat: no-repeat;
            background-size: 100% 100%;
        }
        /* Hide number input spinners */
        input[type=number]::-webkit-inner-spin-button,
        input[type=number]::-webkit-outer-spin-button { -webkit-appearance: none; margin: 0; }
        /* Nice scrollbar for the showcase only (kept minimal) */
        .showcase-scroll::-webkit-scrollbar { height: 10px; width: 10px; }
        .showcase-scroll::-webkit-scrollbar-thumb { background: #DED5C7; border-radius: 999px; border: 2px solid #FFFCF9; }
        .showcase-scroll::-webkit-scrollbar-thumb:hover { background: #C9A86A; }
    </style>
</head>

<body class="bg-[#F3EFE7]">
    <!-- Page background with very soft vignettes -->
    <div class="min-h-screen w-full relative">
        <div class="pointer-events-none absolute inset-0 overflow-hidden">
            <div class="absolute -top-1/3 right-[-10%] h-[520px] w-[520px] rounded-full blur-[120px] bg-[radial-gradient(circle_at_center,_rgba(201,168,106,0.18),_transparent_60%)]"></div>
            <div class="absolute -bottom-1/4 left-[-12%] h-[560px] w-[560px] rounded-full blur-[130px] bg-[radial-gradient(circle_at_center,_rgba(31,31,31,0.08),_transparent_60%)]"></div>
        </div>

        <!-- Centered showcase frame (Dribbble / portfolio presentation) -->
        <div class="max-w-[1340px] mx-auto px-4 sm:px-6 lg:px-8 py-8 lg:py-12">
            <!-- Editorial header note -->
            <div class="flex items-center justify-between gap-4 mb-5 text-[11px] tracking-[0.22em] text-[#6B665F] uppercase">
                <span>RF DESIGNS • INTERIOR ARCHITECTURE • NEW YORK / LONDON</span>
                <span class="hidden sm:inline-flex items-center gap-3">
                    <span class="inline-flex items-center gap-2">
                        <span class="h-1.5 w-1.5 rounded-full bg-[#C9A86A]"></span>
                        AVAILABLE FOR SELECT COMMISSIONS • 2026
                    </span>
                    <span class="h-3 w-px bg-[#E8E2D9]"></span>
                    <span>1440 • 16:9 • SHOWCASE</span>
                </span>
            </div>

            <!-- The actual site lives inside this frame -->
            <div class="rounded-[28px] bg-[#FFFCF9] shadow-[0_30px_80px_rgba(31,31,31,0.12),0_2px_12px_rgba(31,31,31,0.06)] ring-1 ring-black/5 overflow-hidden paper-texture">
                <!-- Fake browser bar (Mac style) – subtle, editorial, not gimmicky -->
                <div class="h-11 bg-[#F1EBE2] border-b border-[#E8E2D9] flex items-center px-4 gap-2">
                    <div class="flex items-center gap-1.5 pr-3 mr-3 border-r border-[#E3DCCC]/70">
                        <span class="h-3 w-3 rounded-full bg-[#FF5F56] shadow-inner"></span>
                        <span class="h-3 w-3 rounded-full bg-[#FFBD2E] shadow-inner"></span>
                        <span class="h-3 w-3 rounded-full bg-[#27C93F] shadow-inner"></span>
                    </div>
                    <div class="hidden md:flex items-center gap-2 text-[11px] text-[#6B665F] tracking-wide">
                        <span class="inline-flex items-center gap-1.5 px-2.5 py-1 rounded-md bg-white/70 border border-[#E8E2D9] text-[#4A453E]">
                            <svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.75" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true"><path d="M10 14l-4 4m0-4l4 4"/><path d="M14 10l4-4m0 4l-4-4"/><rect x="3" y="3" width="18" height="18" rx="2"/></svg>
                            rf-designs.com
                        </span>
                        <span class="text-[#A79E91]">/</span>
                        <span>studio • work • journal • contact</span>
                    </div>
                    <div class="ml-auto hidden lg:flex items-center gap-3 text-[10px] tracking-[0.2em] text-[#928A7E] uppercase">
                        <span>DESKTOP</span>
                        <span class="h-3 w-px bg-[#E3DCCC]"></span>
                        <span>UI • 2026</span>
                    </div>
                </div>

                <!-- SITE CONTENT -->
                <div class="showcase-scroll bg-[#FFFCF9]">
                    <!-- NAVIGATION -->
                    <header class="sticky top-0 z-40 backdrop-blur supports-[backdrop-filter]:bg-[#FFFCF9]/80 bg-[#FFFCF9]/95 border-b border-[#EFE6DA]">
                        <div class="max-w-[1120px] mx-auto px-5 sm:px-8 lg:px-0 h-[72px] flex items-center justify-between">
                            <a href="#" class="flex items-center gap-3 group">
                                <div class="h-10 w-10 rounded-[12px] bg-[#111] text-[#F6F1E7] grid place-items-center serif text-[22px] leading-none tracking-tight shadow-sm">
                                    RF
                                </div>
                                <div class="leading-tight">
                                    <div class="serif text-[22px] tracking-[-0.02em] text-[#1F1F1F]">RF Designs</div>
                                    <div class="text-[10px] tracking-[0.28em] text-[#7A7266] uppercase -mt-1">Interior Architecture</div>
                                </div>
                            </a>

                            <nav class="hidden lg:flex items-center gap-9 text-[13.5px] tracking-[0.01em] text-[#403A33]">
                                <a href="#work" class="hover:text-[#1F1F1F] transition-colors">Work</a>
                                <a href="#studio" class="hover:text-[#1F1F1F] transition-colors">Studio</a>
                                <a href="#services" class="hover:text-[#1F1F1F] transition-colors">Services</a>
                                <a href="#journal" class="hover:text-[#1F1F1F] transition-colors">Journal</a>
                                <span class="h-5 w-px bg-[#E8E2D9]"></span>
                                <a href="#contact" class="inline-flex items-center gap-2 pl-3 pr-3.5 h-9 rounded-full bg-[#111] text-white hover:translate-y-[1px] active:translate-y-[2px] transition-all shadow-sm">
                                    <span>Contact</span>
                                    <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.75" stroke-linecap="round" stroke-linejoin="round"><path d="M7 17L17 7"/><path d="M9 7h8v8"/></svg>
                                </a>
                            </nav>

                            <!-- Mobile simple -->
                            <a href="#contact" class="lg:hidden inline-flex items-center gap-1.5 text-xs font-medium px-3 h-9 rounded-full bg-[#111] text-white">
                                Contact
                            </a>
                        </div>
                    </header>

                    <!-- HERO: split editorial + prominent contact form -->
                    <section class="border-b border-[#EFE6DA]">
                        <div class="max-w-[1120px] mx-auto px-5 sm:px-8 lg:px-0 py-14 lg:py-20 grid lg:grid-cols-12 gap-10 lg:gap-14 items-start">
                            <!-- Left: editorial headline -->
                            <div class="lg:col-span-7">
                                <div class="inline-flex items-center gap-2 text-[10.5px] tracking-[0.26em] uppercase text-[#7A6F5F] bg-[#F6F1E7] border border-[#E8DFCF] rounded-full px-3 py-1.5">
                                    <span class="h-1.5 w-1.5 rounded-full bg-[#C9A86A]"></span>
                                    New York • London • Tulum
                                </div>

                                <h1 class="serif mt-6 text-[52px] sm:text-[66px] lg:text-[78px] leading-[0.9] tracking-[-0.03em] text-[#1A1A1A] max-w-[14ch]">
                                    Interior architecture for the quietly extraordinary.
                                </h1>

                                <p class="mt-7 text-[17px] leading-[1.7] text-[#4A453E] max-w-[62ch] font-light">
                                    We design residences and workplaces with a restrained material palette, precise daylight, and the kind of calm that feels inevitable. Every project is led by partners, built by artisans, and resolved down to the last millimeter.
                                </p>

                                <div class="mt-9 flex flex-wrap items-center gap-5 text-[12px] text-[#6B6256]">
                                    <div class="flex items-center gap-3">
                                        <span class="h-px w-10 bg-[#D9CFC0]"></span>
                                        <span class="tracking-[0.18em] uppercase">Selected Recognition</span>
                                    </div>
                                    <div class="flex flex-wrap items-center gap-x-5 gap-y-2">
                                        <span>AD100</span>
                                        <span class="text-[#D0C6B6]">•</span>
                                        <span>Dezeen Awards</span>
                                        <span class="text-[#D0C6B6]">•</span>
                                        <span>Interior Design Hall of Fame</span>
                                    </div>
                                </div>

                                <!-- Mini metrics strip, editorial -->
                                <div class="mt-10 grid grid-cols-3 max-w-xl gap-6 border-t border-[#EFE6DA] pt-6">
                                    <div>
                                        <div class="serif text-3xl leading-none text-[#1F1F1F]">27</div>
                                        <div class="mt-1 text-[11px] tracking-[0.18em] uppercase text-[#7A7266]">Completed Projects</div>
                                    </div>
                                    <div>
                                        <div class="serif text-3xl leading-none text-[#1F1F1F]">9.8/10</div>
                                        <div class="mt-1 text-[11px] tracking-[0.18em] uppercase text-[#7A7266]">Client NPS (5yr)</div>
                                    </div>
                                    <div>
                                        <div class="serif text-3xl leading-none text-[#1F1F1F]">12–16 mo</div>
                                        <div class="mt-1 text-[11px] tracking-[0.18em] uppercase text-[#7A7266]">Typical Timeline</div>
                                    </div>
                                </div>
                            </div>

                            <!-- Right: PROMINENT CONTACT FORM CARD -->
                            <div class="lg:col-span-5 lg:pl-2">
                                <div class="relative">
                                    <!-- Soft lighting bloom behind card -->
                                    <div class="absolute -inset-6 bg-[radial-gradient(60%_60%_at_50%_0%,rgba(201,168,106,0.18),transparent_70%)] blur-2xl pointer-events-none"></div>

                                    <div id="contact" class="relative rounded-[28px] bg-white border border-[#E9E1D4] shadow-[0_20px_60px_rgba(17,17,17,0.10),0_1px_0_rgba(255,255,255,0.6)_inset] overflow-hidden">
                                        <div class="p-6 sm:p-8">
                                            <div class="flex items-start justify-between gap-4">
                                                <div>
                                                    <div class="inline-flex items-center gap-2 text-[10px] tracking-[0.24em] uppercase text-[#7A6F5F] bg-[#F8F4EC] border border-[#E8DFCF] rounded-full px-2.5 py-1">
                                                        ENQUIRY • PARTNER-LED
                                                    </div>
                                                    <h2 class="serif mt-3 text-[32px] leading-[0.95] tracking-[-0.02em] text-[#141414]">Begin a conversation</h2>
                                                    <p class="mt-2 text-[13.5px] leading-relaxed text-[#5C554D]">Tell us about your place and timing. We respond to qualified inquiries within two business hours, with discretion.</p>
                                                </div>
                                                <div class="hidden sm:flex h-11 w-11 items-center justify-center rounded-full bg-[#111] text-white shadow-sm">
                                                    <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" aria-hidden="true"><path d="M21 15a4 4 0 0 1-4 4H7l-4 4V7a4 4 0 0 1 4-4h10a4 4 0 0 1 4 4z"/><path d="M8 9h8M8 13h6"/></svg>
                                                </div>
                                            </div>

                                            <form id="contactForm" class="mt-6 space-y-4" novalidate>
                                                <div class="grid sm:grid-cols-2 gap-3">
                                                    <div>
                                                        <label class="block text-[11px] tracking-[0.14em] uppercase text-[#7A7266] mb-1.5">Full name</label>
                                                        <input required type="text" name="name" placeholder="Eleanor Vance"
                                                            class="w-full h-11 rounded-xl bg-[#FCFAF7] border border-[#E7DED0] px-3.5 text-[14px] text-[#2A2520] placeholder-[#A99F91] focus-gold transition" />
                                                    </div>
                                                    <div>
                                                        <label class="block text-[11px] tracking-[0.14em] uppercase text-[#7A7266] mb-1.5">Email</label>
                                                        <input required type="email" name="email" placeholder="eleanor@studio.com"
                                                            class="w-full h-11 rounded-xl bg-[#FCFAF7] border border-[#E7DED0] px-3.5 text-[14px] text-[#2A2520] placeholder-[#A99F91] focus-gold transition" />
                                                    </div>
                                                </div>

                                                <div class="grid sm:grid-cols-2 gap-3">
                                                    <div>
                                                        <label class="block text-[11px] tracking-[0.14em] uppercase text-[#7A7266] mb-1.5">Phone (optional)</label>
                                                        <input type="tel" name="phone" placeholder="+1 (212) 555-0148"
                                                            class="w-full h-11 rounded-xl bg-[#FCFAF7] border border-[#E7DED0] px-3.5 text-[14px] text-[#2A2520] placeholder-[#A99F91] focus-gold transition" />
                                                    </div>
                                                    <div>
                                                        <label class="block text-[11px] tracking-[0.14em] uppercase text-[#7A7266] mb-1.5">Project type</label>
                                                        <div class="relative">
                                                            <select name="type" required
                                                                class="appearance-none w-full h-11 rounded-xl bg-[#FCFAF7] border border-[#E7DED0] px-3.5 pr-10 text-[14px] text-[#2A2520] focus-gold transition">
                                                                <option value="" disabled selected>Select…</option>
                                                                <option>Private Residence</option>
                                                                <option>Pied-à-terre / Penthouse</option>
                                                                <option>Corporate Headquarters</option>
                                                                <option>Boutique Hospitality</option>
                                                                <option>Gallery / Retail</option>
                                                            </select>
                                                            <svg class="pointer-events-none absolute right-3 top-1/2 -translate-y-1/2" width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="#8A8173" stroke-width="1.75" stroke-linecap="round" stroke-linejoin="round"><path d="M6 9l6 6 6-6"/></svg>
                                                        </div>
                                                    </div>
                                                </div>

                                                <div class="grid sm:grid-cols-2 gap-3">
                                                    <div>
                                                        <label class="block text-[11px] tracking-[0.14em] uppercase text-[#7A7266] mb-1.5">Location</label>
                                                        <input type="text" name="location" placeholder="New York, NY — TriBeCa" 
                                                            class="w-full h-11 rounded-xl bg-[#FCFAF7] border border-[#E7DED0] px-3.5 text-[14px] text-[#2A2520] placeholder-[#A99F91] focus-gold transition" />
                                                    </div>
                                                    
