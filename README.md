# Bandlamudi-financial-serv<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bandlamudi Financial Services</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">
    <!-- FontAwesome for Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                    },
                    colors: {
                        brand: {
                            50: '#eff6ff',
                            100: '#dbeafe',
                            500: '#3b82f6', // Blue standard
                            600: '#2563eb',
                            800: '#1e40af',
                            900: '#1e3a8a', // Deep blue
                            gold: '#d97706', // Accent gold
                        }
                    }
                }
            }
        }
    </script>
    <style>
        .hero-bg {
            background-image: linear-gradient(rgba(30, 58, 138, 0.85), rgba(30, 58, 138, 0.7)), url('https://images.unsplash.com/photo-1565514020176-6c2235c87445?ixlib=rb-4.0.3&auto=format&fit=crop&w=1920&q=80');
            background-size: cover;
            background-position: center;
        }
        html {
            scroll-behavior: smooth;
        }
    </style>
</head>
<body class="font-sans text-gray-700 antialiased bg-gray-50">

    <!-- Navigation -->
    <nav class="bg-white shadow-md fixed w-full z-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between h-20">
                <div class="flex items-center">
                    <div class="flex-shrink-0 flex items-center gap-2">
                        <!-- Logo Icon -->
                        <div class="bg-brand-900 text-white p-2 rounded-lg">
                            <i class="fa-solid fa-chart-line text-2xl"></i>
                        </div>
                        <div class="flex flex-col">
                            <span class="font-bold text-xl text-brand-900 leading-tight">Bandlamudi</span>
                            <span class="text-xs font-semibold text-brand-600 tracking-wider">FINANCIAL SERVICES</span>
                        </div>
                    </div>
                </div>
                
                <!-- Desktop Menu -->
                <div class="hidden md:flex items-center space-x-8">
                    <a href="#home" class="text-gray-600 hover:text-brand-600 font-medium transition">Home</a>
                    <a href="#about" class="text-gray-600 hover:text-brand-600 font-medium transition">About Us</a>
                    <a href="#services" class="text-gray-600 hover:text-brand-600 font-medium transition">Services</a>
                    <a href="#contact" class="bg-brand-600 text-white px-5 py-2.5 rounded-full font-medium hover:bg-brand-800 transition shadow-lg shadow-brand-500/30">Apply Now</a>
                </div>

                <!-- Mobile menu button -->
                <div class="flex items-center md:hidden">
                    <button onclick="toggleMenu()" class="text-gray-500 hover:text-brand-600 focus:outline-none p-2">
                        <i class="fa-solid fa-bars text-2xl"></i>
                    </button>
                </div>
            </div>
        </div>

        <!-- Mobile Menu -->
        <div id="mobile-menu" class="hidden md:hidden bg-white border-t border-gray-100">
            <div class="px-2 pt-2 pb-3 space-y-1 sm:px-3">
                <a href="#home" onclick="toggleMenu()" class="block px-3 py-2 rounded-md text-base font-medium text-gray-700 hover:text-brand-600 hover:bg-gray-50">Home</a>
                <a href="#about" onclick="toggleMenu()" class="block px-3 py-2 rounded-md text-base font-medium text-gray-700 hover:text-brand-600 hover:bg-gray-50">About Us</a>
                <a href="#services" onclick="toggleMenu()" class="block px-3 py-2 rounded-md text-base font-medium text-gray-700 hover:text-brand-600 hover:bg-gray-50">Services</a>
                <a href="#contact" onclick="toggleMenu()" class="block px-3 py-2 rounded-md text-base font-medium text-brand-600 font-bold hover:bg-gray-50">Contact Us</a>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="hero-bg h-screen min-h-[600px] flex items-center relative">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 w-full pt-16">
            <div class="md:w-2/3 lg:w-1/2 text-white">
                <div class="inline-block bg-brand-gold text-white text-xs font-bold px-3 py-1 rounded-full mb-4 uppercase tracking-wide">
                    Trusted Financial Partner
                </div>
                <h1 class="text-4xl md:text-5xl lg:text-6xl font-bold leading-tight mb-6">
                    Turning Your Dreams Into Reality
                </h1>
                <p class="text-lg md:text-xl text-gray-200 mb-8 leading-relaxed">
                    We provide comprehensive loan solutions across Banking & Non-Banking sectors. From personal needs to business growth, Bandlamudi Financial Services is with you every step of the way.
                </p>
                <div class="flex flex-col sm:flex-row gap-4">
                    <a href="#contact" class="bg-white text-brand-900 px-8 py-3.5 rounded-full font-bold text-center hover:bg-gray-100 transition shadow-lg">
                        Get a Quote
                    </a>
                    <a href="#services" class="border-2 border-white text-white px-8 py-3.5 rounded-full font-bold text-center hover:bg-white hover:text-brand-900 transition">
                        View Services
                    </a>
                </div>
            </div>
        </div>
        
        <!-- Trust Indicators (Bottom of Hero) -->
        <div class="absolute bottom-0 w-full bg-brand-900/50 backdrop-blur-sm border-t border-white/10 hidden md:block">
            <div class="max-w-7xl mx-auto px-4 py-4 flex justify-between text-white text-sm font-medium opacity-90">
                <div class="flex items-center gap-2"><i class="fa-solid fa-check-circle text-brand-gold"></i> Quick Approval</div>
                <div class="flex items-center gap-2"><i class="fa-solid fa-check-circle text-brand-gold"></i> Low Interest Rates</div>
                <div class="flex items-center gap-2"><i class="fa-solid fa-check-circle text-brand-gold"></i> Transparent Process</div>
                <div class="flex items-center gap-2"><i class="fa-solid fa-check-circle text-brand-gold"></i> Banking & NBFC Partners</div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-20 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <h2 class="text-brand-900 text-3xl md:text-4xl font-bold mb-4">Who We Are</h2>
                <div class="h-1 w-20 bg-brand-gold mx-auto mb-6"></div>
                <p class="text-gray-600 text-lg">
                    Bandlamudi Financial Services bridges the gap between you and the financial support you need. Whether through traditional banking or the non-banking sector, we specialize in finding the perfect financial product tailored to your unique situation.
                </p>
            </div>
            
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8 text-center">
                <div class="p-6 bg-gray-50 rounded-xl hover:shadow-lg transition duration-300">
                    <div class="w-16 h-16 bg-brand-100 text-brand-600 rounded-full flex items-center justify-center mx-auto mb-4 text-2xl">
                        <i class="fa-solid fa-handshake"></i>
                    </div>
                    <h3 class="text-xl font-bold text-gray-900 mb-2">Expert Guidance</h3>
                    <p class="text-gray-600">We guide you through the complex world of finance to ensure you get the best deal.</p>
                </div>
                <div class="p-6 bg-gray-50 rounded-xl hover:shadow-lg transition duration-300">
                    <div class="w-16 h-16 bg-brand-100 text-brand-600 rounded-full flex items-center justify-center mx-auto mb-4 text-2xl">
                        <i class="fa-solid fa-bolt"></i>
                    </div>
                    <h3 class="text-xl font-bold text-gray-900 mb-2">Fast Processing</h3>
                    <p class="text-gray-600">Minimal documentation and quick disbursement channels to save your time.</p>
                </div>
                <div class="p-6 bg-gray-50 rounded-xl hover:shadow-lg transition duration-300">
                    <div class="w-16 h-16 bg-brand-100 text-brand-600 rounded-full flex items-center justify-center mx-auto mb-4 text-2xl">
                        <i class="fa-solid fa-shield-halved"></i>
                    </div>
                    <h3 class="text-xl font-bold text-gray-900 mb-2">Secure & Trusted</h3>
                    <p class="text-gray-600">Your privacy and security are our top priorities throughout the loan process.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section id="services" class="py-20 bg-gray-100">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <span class="text-brand-600 font-bold uppercase tracking-wider text-sm">Our Expertise</span>
                <h2 class="text-3xl md:text-4xl font-bold text-gray-900 mt-2">Comprehensive Loan Services</h2>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                
                <!-- Personal Loan -->
                <div class="bg-white rounded-xl shadow-sm hover:shadow-xl transition duration-300 overflow-hidden group">
                    <div class="h-2 bg-brand-500"></div>
                    <div class="p-8">
                        <div class="flex justify-between items-start mb-4">
                            <i class="fa-solid fa-user-tag text-3xl text-brand-600"></i>
                            <span class="bg-blue-100 text-blue-800 text-xs px-2 py-1 rounded font-bold">Popular</span>
                        </div>
                        <h3 class="text-xl font-bold text-gray-900 mb-3 group-hover:text-brand-600 transition">Personal Loans</h3>
                        <p class="text-gray-600 mb-4 text-sm">Flexible funds for your personal needs, weddings, medical emergencies, or travel.</p>
                        <a href="#contact" class="text-brand-600 font-bold text-sm hover:underline">Apply Now &rarr;</a>
                    </div>
                </div>

                <!-- Mortgage Loan -->
                <div class="bg-white rounded-xl shadow-sm hover:shadow-xl transition duration-300 overflow-hidden group">
                    <div class="h-2 bg-brand-600"></div>
                    <div class="p-8">
                        <div class="mb-4">
                            <i class="fa-solid fa-house-lock text-3xl text-brand-600"></i>
                        </div>
                        <h3 class="text-xl font-bold text-gray-900 mb-3 group-hover:text-brand-600 transition">Mortgage Loans</h3>
                        <p class="text-gray-600 mb-4 text-sm">Unlock the value of your property. Competitive interest rates against residential or commercial property.</p>
                        <a href="#contact" class="text-brand-600 font-bold text-sm hover:underline">Apply Now &rarr;</a>
                    </div>
                </div>

                <!-- Construction Loan -->
                <div class="bg-white rounded-xl shadow-sm hover:shadow-xl transition duration-300 overflow-hidden group">
                    <div class="h-2 bg-brand-800"></div>
                    <div class="p-8">
                        <div class="mb-4">
                            <i class="fa-solid fa-trowel-bricks text-3xl text-brand-600"></i>
                        </div>
                        <h3 class="text-xl font-bold text-gray-900 mb-3 group-hover:text-brand-600 transition">Construction Loans</h3>
                        <p class="text-gray-600 mb-4 text-sm">Building your dream home? We provide funds tailored to construction stages.</p>
                        <a href="#contact" class="text-brand-600 font-bold text-sm hover:underline">Apply Now &rarr;</a>
                    </div>
                </div>

                <!-- Purchase Loan -->
                <div class="bg-white rounded-xl shadow-sm hover:shadow-xl transition duration-300 overflow-hidden group">
                    <div class="h-2 bg-brand-gold"></div>
                    <div class="p-8">
                        <div class="mb-4">
                            <i class="fa-solid fa-cart-shopping text-3xl text-brand-gold"></i>
                        </div>
                        <h3 class="text-xl font-bold text-gray-900 mb-3 group-hover:text-brand-600 transition">Purchase Loans</h3>
                        <p class="text-gray-600 mb-4 text-sm">Financing for purchasing new plots, flats, or commercial spaces with ease.</p>
                        <a href="#contact" class="text-brand-600 font-bold text-sm hover:underline">Apply Now &rarr;</a>
                    </div>
                </div>

                <!-- Car Loan -->
                <div class="bg-white rounded-xl shadow-sm hover:shadow-xl transition duration-300 overflow-hidden group">
                    <div class="h-2 bg-gray-800"></div>
                    <div class="p-8">
                        <div class="mb-4">
                            <i class="fa-solid fa-car text-3xl text-gray-700"></i>
                        </div>
                        <h3 class="text-xl font-bold text-gray-900 mb-3 group-hover:text-brand-600 transition">Car Loans</h3>
                        <p class="text-gray-600 mb-4 text-sm">Drive your dream car today. New and used car loans with flexible repayment tenures.</p>
                        <a href="#contact" class="text-brand-600 font-bold text-sm hover:underline">Apply Now &rarr;</a>
                    </div>
                </div>

                <!-- Mudra Loan -->
                <div class="bg-white rounded-xl shadow-sm hover:shadow-xl transition duration-300 overflow-hidden group">
                    <div class="h-2 bg-green-600"></div>
                    <div class="p-8">
                        <div class="mb-4">
                            <i class="fa-solid fa-seedling text-3xl text-green-600"></i>
                        </div>
                        <h3 class="text-xl font-bold text-gray-900 mb-3 group-hover:text-brand-600 transition">Mudra Loans</h3>
                        <p class="text-gray-600 mb-4 text-sm">Supporting small businesses and entrepreneurs under the Pradhan Mantri MUDRA Yojana.</p>
                        <a href="#contact" class="text-brand-600 font-bold text-sm hover:underline">Apply Now &rarr;</a>
                    </div>
                </div>

                <!-- Education Loan -->
                <div class="bg-white rounded-xl shadow-sm hover:shadow-xl transition duration-300 overflow-hidden group">
                    <div class="h-2 bg-red-500"></div>
                    <div class="p-8">
                        <div class="mb-4">
                            <i class="fa-solid fa-graduation-cap text-3xl text-red-500"></i>
                        </div>
                        <h3 class="text-xl font-bold text-gray-900 mb-3 group-hover:text-brand-600 transition">Education Loans</h3>
                        <p class="text-gray-600 mb-4 text-sm">Invest in the future. Loans for higher studies in India and abroad.</p>
                        <a href="#contact" class="text-brand-600 font-bold text-sm hover:underline">Apply Now &rarr;</a>
                    </div>
                </div>
                
                 <!-- Other Services -->
                 <div class="bg-gray-50 rounded-xl border-2 border-dashed border-gray-300 flex flex-col items-center justify-center p-8">
                    <i class="fa-solid fa-plus text-4xl text-gray-400 mb-3"></i>
                    <h3 class="text-lg font-bold text-gray-600">And More...</h3>
                    <p class="text-sm text-gray-500 text-center mt-2">Contact us for custom financial requirements.</p>
                </div>

            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-20 bg-brand-900 relative">
        <!-- Decorative pattern -->
        <div class="absolute top-0 left-0 w-full h-full overflow-hidden opacity-10 pointer-events-none">
             <i class="fa-solid fa-chart-pie text-white absolute -top-10 -left-10 text-9xl"></i>
             <i class="fa-solid fa-coins text-white absolute bottom-10 right-10 text-9xl"></i>
        </div>

        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10">
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center">
                
                <!-- Contact Info -->
                <div class="text-white">
                    <h2 class="text-3xl md:text-4xl font-bold mb-6">Let's Discuss Your Financial Goals</h2>
                    <p class="text-blue-100 text-lg mb-8">
                        Ready to take the next step? Fill out the form or reach out to us directly. Our team is ready to assist you with Banking & Non-banking sector loans.
                    </p>
                    
                    <div class="space-y-6">
                        <div class="flex items-start gap-4">
                            <div class="bg-brand-600 p-3 rounded-lg">
                                <i class="fa-solid fa-phone text-xl"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-lg">Call Us</h4>
                                <p class="text-blue-100">+91 93813 24622</p>
                                <p class="text-xs text-blue-300">(Available 9 AM - 6 PM)</p>
                            </div>
                        </div>
                        
                        <div class="flex items-start gap-4">
                            <div class="bg-brand-600 p-3 rounded-lg">
                                <i class="fa-solid fa-envelope text-xl"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-lg">Email Us</h4>
                                <p class="text-blue-100">bandlamudifinancialservices07@gmail.com</p>
                            </div>
                        </div>

                        <div class="flex items-start gap-4">
                            <div class="bg-brand-600 p-3 rounded-lg">
                                <i class="fa-solid fa-location-dot text-xl"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-lg">Visit Us</h4>
                                <p class="text-blue-100">Bandlamudi Financial Services<br>Main Office, Guntur<br>Andhra Pradesh, India</p>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Contact Form -->
                <div class="bg-white rounded-2xl p-8 shadow-2xl">
                    <h3 class="text-2xl font-bold text-gray-800 mb-6">Quick Inquiry</h3>
                    <form onsubmit="ices-
