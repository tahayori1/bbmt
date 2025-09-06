Of course! Here is a high-quality, professional, and fully responsive website template for Bozorgi Group, built with HTML, Tailwind CSS, and a touch of JavaScript.

This design incorporates all your requirements, including brand colors, SEO best practices, a mobile-first approach, and modern UI/UX principles.

### Key Features of this Template:
*   **Fully Responsive:** Looks great on all devices, from mobile phones to large desktops.
*   **SEO Optimized:** Includes all necessary meta tags, structured data (JSON-LD), and semantic HTML for high search engine visibility.
*   **High Performance:** Uses lazy loading for images and optimized assets for fast load times.
*   **Modern & Professional Design:** Clean layout with a sophisticated color palette of black, gold, and white, reflecting the premium quality of the brand.
*   **Interactive Elements:** Smooth scrolling, a responsive navigation menu, and subtle animations enhance the user experience.
*   **Clear CTAs:** Strategically placed "Quick Contact" and other call-to-action buttons to guide users.

---

### `index.html`

Copy and paste the following code into a file named `index.html`.

```html
<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bozorgi Group - Premium Building Materials Trading Since 1889</title>

    <!-- SEO Meta Tags -->
    <meta name="description" content="Bozorgi Group, a leading building materials supplier in Dubai, offers high-quality MDF, HDF, Hardwood, and more. With a legacy since 1889, we provide global trading solutions with honesty and transparency.">
    <meta name="keywords" content="Bozorgi Group, building materials, MDF, HDF, Polywood, Hardwood, Chipboard, HPL, Natural Veneer, wood trading, Dubai, UAE">
    <meta name="author" content="Bozorgi Group">
    <link rel="canonical" href="https://www.bozorgigroup.com/">
    <link rel="icon" type="image/png" href="https://lh3.googleusercontent.com/MQ1BMU25DGoAOhOlCsZz9oQ1HYJog_nHwoKyd5XyETcxWCoOpHhgduAD65Puw8PmhOvOOrJz6n8fN_nvJb437_cFNh1RNaNKenmI41ed3amHqDdPvucCajH1nTNzudc2orCfteU-4nDogbznW0Oa2YVihzwv6gHRwaJ-eArEC9Ye0FfmbaD2vg=w1280">

    <!-- Open Graph / Facebook -->
    <meta property="og:type" content="website">
    <meta property="og:url" content="https://www.bozorgigroup.com/">
    <meta property="og:title" content="Bozorgi Group - Premium Building Materials Trading Since 1889">
    <meta property="og:description" content="Discover premium building materials from a trusted global supplier with a rich history dating back to 1889.">
    <meta property="og:image" content="https://lh3.googleusercontent.com/MQ1BMU25DGoAOhOlCsZz9oQ1HYJog_nHwoKyd5XyETcxWCoOpHhgduAD65Puw8PmhOvOOrJz6n8fN_nvJb437_cFNh1RNaNKenmI41ed3amHqDdPvucCajH1nTNzudc2orCfteU-4nDogbznW0Oa2YVihzwv6gHRwaJ-eArEC9Ye0FfmbaD2vg=w1280">

    <!-- Twitter -->
    <meta property="twitter:card" content="summary_large_image">
    <meta property="twitter:url" content="https://www.bozorgigroup.com/">
    <meta property="twitter:title" content="Bozorgi Group - Premium Building Materials Trading Since 1889">
    <meta property="twitter:description" content="Discover premium building materials from a trusted global supplier with a rich history dating back to 1889.">
    <meta property="twitter:image" content="https://lh3.googleusercontent.com/MQ1BMU25DGoAOhOlCsZz9oQ1HYJog_nHwoKyd5XyETcxWCoOpHhgduAD65Puw8PmhOvOOrJz6n8fN_nvJb437_cFNh1RNaNKenmI41ed3amHqDdPvucCajH1nTNzudc2orCfteU-4nDogbznW0Oa2YVihzwv6gHRwaJ-eArEC9Ye0FfmbaD2vg=w1280">

    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>

    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@700;800&family=Poppins:wght@400;500;600&display=swap" rel="stylesheet">

    <!-- Custom Styles -->
    <style>
        body {
            font-family: 'Poppins', sans-serif;
            background-color: #f8f9fa;
        }
        h1, h2, h3, h4, h5, h6 {
            font-family: 'Montserrat', sans-serif;
        }
        .bg-primary-gold { background-color: #D4AF37; }
        .text-primary-gold { color: #D4AF37; }
        .border-primary-gold { border-color: #D4AF37; }
        .hover\:bg-accent-bronze:hover { background-color: #B88714; }
        
        .hero-section {
            background-image: linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.7)), url('https://images.unsplash.com/photo-1618221195710-dd6b41faaea6?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=2000&q=80');
            background-size: cover;
            background-position: center;
        }
        .timeline::before {
            content: '';
            position: absolute;
            left: 50%;
            transform: translateX(-50%);
            top: 0;
            bottom: 0;
            width: 4px;
            background-color: #D4AF37;
        }
        @media (max-width: 768px) {
            .timeline::before {
                left: 20px;
            }
        }
        .fade-in {
            opacity: 0;
            transform: translateY(20px);
            transition: opacity 0.6s ease-out, transform 0.6s ease-out;
        }
        .fade-in.visible {
            opacity: 1;
            transform: translateY(0);
        }
    </style>

    <!-- JSON-LD Structured Data -->
    <script type="application/ld+json">
    {
      "@context": "https://schema.org",
      "@type": "Organization",
      "name": "Bozorgi Group",
      "url": "https://www.bozorgigroup.com/",
      "logo": "https://lh3.googleusercontent.com/MQ1BMU25DGoAOhOlCsZz9oQ1HYJog_nHwoKyd5XyETcxWCoOpHhgduAD65Puw8PmhOvOOrJz6n8fN_nvJb437_cFNh1RNaNKenmI41ed3amHqDdPvucCajH1nTNzudc2orCfteU-4nDogbznW0Oa2YVihzwv6gHRwaJ-eArEC9Ye0FfmbaD2vg=w1280",
      "contactPoint": {
        "@type": "ContactPoint",
        "telephone": "+971-4-321-3030",
        "contactType": "customer service",
        "areaServed": "AE",
        "availableLanguage": "en"
      },
      "address": {
        "@type": "PostalAddress",
        "streetAddress": "Business Bay Street, Marasi Dr, Al Manara Tower, 8th floor, office No. 802",
        "addressLocality": "Dubai",
        "postalCode": "124361",
        "addressCountry": "AE"
      },
      "sameAs": [
        "https://www.facebook.com/AliBozorgiofficial/",
        "https://x.com/aliabozorgi",
        "https://www.instagram.com/alibozorgi.uae"
      ],
      "founder": {
        "@type": "Person",
        "name": "Bozorg Bozorgi"
      },
      "foundingDate": "1889",
      "description": "Bozorgi Building Material Company, under the brand BOZORGI GROUP, has been a trading company since 1988 with roots dating back to 1889. We specialize in supplying, importing, and exporting building materials globally."
    }
    </script>
</head>
<body class="bg-white text-gray-800">

    <!-- Header -->
    <header id="header" class="bg-black bg-opacity-80 backdrop-blur-md text-white sticky top-0 z-50 transition-all duration-300">
        <div class="container mx-auto px-6 py-3 flex justify-between items-center">
            <a href="#hero" class="flex items-center">
                <img src="https://lh3.googleusercontent.com/MQ1BMU25DGoAOhOlCsZz9oQ1HYJog_nHwoKyd5XyETcxWCoOpHhgduAD65Puw8PmhOvOOrJz6n8fN_nvJb437_cFNh1RNaNKenmI41ed3amHqDdPvucCajH1nTNzudc2orCfteU-4nDogbznW0Oa2YVihzwv6gHRwaJ-eArEC9Ye0FfmbaD2vg=w1280" alt="Bozorgi Group Logo" class="h-10 md:h-12 w-auto">
            </a>
            <nav class="hidden lg:flex items-center space-x-8">
                <a href="#about" class="hover:text-primary-gold transition duration-300">About Us</a>
                <a href="#products" class="hover:text-primary-gold transition duration-300">Products</a>
                <a href="#history" class="hover:text-primary-gold transition duration-300">History</a>
                <a href="#humanity" class="hover:text-primary-gold transition duration-300">Humanity First</a>
                <a href="#contact" class="bg-primary-gold text-black font-bold py-2 px-6 rounded-full hover:bg-accent-bronze transition duration-300">Quick Contact</a>
            </nav>
            <button id="mobile-menu-button" class="lg:hidden text-white focus:outline-none" aria-label="Open menu">
                <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7"></path></svg>
            </button>
        </div>
        <!-- Mobile Menu -->
        <div id="mobile-menu" class="hidden lg:hidden bg-black bg-opacity-95">
            <a href="#about" class="block text-center py-3 px-4 text-sm hover:bg-primary-gold hover:text-black transition duration-300">About Us</a>
            <a href="#products" class="block text-center py-3 px-4 text-sm hover:bg-primary-gold hover:text-black transition duration-300">Products</a>
            <a href="#history" class="block text-center py-3 px-4 text-sm hover:bg-primary-gold hover:text-black transition duration-300">History</a>
            <a href="#humanity" class="block text-center py-3 px-4 text-sm hover:bg-primary-gold hover:text-black transition duration-300">Humanity First</a>
            <a href="#contact" class="block text-center py-4 px-4 bg-primary-gold text-black font-bold hover:bg-accent-bronze transition duration-300">Quick Contact</a>
        </div>
    </header>

    <main>
        <!-- Hero Section -->
        <section id="hero" class="hero-section h-screen flex items-center justify-center text-white text-center">
            <div class="container mx-auto px-6">
                <h1 class="text-4xl md:text-6xl lg:text-7xl font-extrabold uppercase tracking-wider mb-4 fade-in">A Legacy of Quality</h1>
                <p class="text-lg md:text-2xl mb-8 max-w-3xl mx-auto font-light fade-in" style="transition-delay: 200ms;">Delivering premium building materials and global trading solutions since 1889.</p>
                <div class="space-x-4 fade-in" style="transition-delay: 400ms;">
                    <a href="#products" class="bg-primary-gold text-black font-bold py-3 px-8 rounded-full hover:bg-accent-bronze transition duration-300 text-lg">Our Products</a>
                    <a href="#contact" class="border-2 border-primary-gold text-white font-bold py-3 px-8 rounded-full hover:bg-primary-gold hover:text-black transition duration-300 text-lg">Request a Quote</a>
                </div>
            </div>
        </section>

        <!-- About Us Section -->
        <section id="about" class="py-20 md:py-32 bg-gray-50">
            <div class="container mx-auto px-6">
                <div class="text-center mb-16">
                    <h2 class="text-3xl md:text-4xl font-bold text-gray-900 mb-4 fade-in">Business Without Boundary</h2>
                    <div class="w-24 h-1 bg-primary-gold mx-auto fade-in"></div>
                </div>
                <div class="grid md:grid-cols-2 gap-12 items-center">
                    <div class="fade-in">
                        <img src="https://images.unsplash.com/photo-1581092921462-205217a3472c?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1287&q=80" alt="Modern business operations" class="rounded-lg shadow-2xl w-full h-auto object-cover">
                    </div>
                    <div class="fade-in" style="transition-delay: 200ms;">
                        <p class="mb-4 text-gray-600">Bozorgi Building Material Company, has operated under the motto “Business Without Boundary“ since 1988. We specialize in trading, exporting, and importing authorized goods worldwide, with a core focus on building materials.</p>
                        <p class="mb-6 text-gray-600">With decades of successful experience, we pride ourselves on our loyal customers and strong relationships with refineries and petrochemicals, ensuring we can meet any demand. Our competitive advantage is our customer-centric approach, creating win-win relationships built on trust and reliability.</p>
                        <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                            <div>
                                <h3 class="font-bold text-xl mb-2 text-gray-800">Our Vision</h3>
                                <p class="text-gray-600">To be a leading business and trading company in building materials by upholding our values of honesty and transparency.</p>
                            </div>
                            <div>
                                <h3 class="font-bold text-xl mb-2 text-gray-800">Our Mission</h3>
                                <p class="text-gray-600">To supply the best building materials, services, and prices to satisfy customers and expand our global reach using modern business systems.</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Products Section -->
        <section id="products" class="py-20 md:py-32 bg-white">
            <div class="container mx-auto px-6">
                <div class="text-center mb-16">
                    <h2 class="text-3xl md:text-4xl font-bold text-gray-900 mb-4 fade-in">Our Premium Product Range</h2>
                    <div class="w-24 h-1 bg-primary-gold mx-auto fade-in"></div>
                </div>
                <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 xl:grid-cols-4 gap-8">
                    <!-- Product Card -->
                    <div class="bg-gray-50 rounded-lg shadow-lg overflow-hidden group transform hover:-translate-y-2 transition-transform duration-300 fade-in">
                        <img loading="lazy" src="https://images.unsplash.com/photo-1620921098595-32e6a39b3a32?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1287&q=80" alt="MDF boards stacked" class="w-full h-56 object-cover">
                        <div class="p-6">
                            <h3 class="text-xl font-bold mb-2">MDF</h3>
                            <p class="text-gray-600 text-sm">Engineered wood from broken down hardwood or softwood residuals, combined with wax and resin.</p>
                        </div>
                    </div>
                    <!-- Product Card -->
                    <div class="bg-gray-50 rounded-lg shadow-lg overflow-hidden group transform hover:-translate-y-2 transition-transform duration-300 fade-in" style="transition-delay: 100ms;">
                        <img loading="lazy" src="https://images.unsplash.com/photo-1595475858853-2941151a669e?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1287&q=80" alt="HDF material" class="w-full h-56 object-cover">
                        <div class="p-6">
                            <h3 class="text-xl font-bold mb-2">HDF</h3>
                            <p class="text-gray-600 text-sm">High-density fiberboard, also known as hardboard, is a durable engineered wood product.</p>
                        </div>
                    </div>
                     <!-- Product Card -->
                    <div class="bg-gray-50 rounded-lg shadow-lg overflow-hidden group transform hover:-translate-y-2 transition-transform duration-300 fade-in" style="transition-delay: 200ms;">
                        <img loading="lazy" src="https://images.unsplash.com/photo-1604964665042-49a027251756?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1287&q=80" alt="Polywood material" class="w-full h-56 object-cover">
                        <div class="p-6">
                            <h3 class="text-xl font-bold mb-2">POLYWOOD</h3>
                            <p class="text-gray-600 text-sm">Made from thermoformed plastics derived from post-consumer bottle waste, such as milk and detergent bottles.</p>
                        </div>
                    </div>
                     <!-- Product Card -->
                    <div class="bg-gray-50 rounded-lg shadow-lg overflow-hidden group transform hover:-translate-y-2 transition-transform duration-300 fade-in" style="transition-delay: 300ms;">
                        <img loading="lazy" src="https://images.unsplash.com/photo-1616047006789-b7af5afb8c20?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1287&q=80" alt="Hardwood planks" class="w-full h-56 object-cover">
                        <div class="p-6">
                            <h3 class="text-xl font-bold mb-2">HARDWOOD</h3>
                            <p class="text-gray-600 text-sm">Wood from dicot trees, found in broad-leaved temperate and tropical forests. Known for its durability.</p>
                        </div>
                    </div>
                     <!-- Product Card -->
                     <div class="bg-gray-50 rounded-lg shadow-lg overflow-hidden group transform hover:-translate-y-2 transition-transform duration-300 fade-in">
                        <img loading="lazy" src="https://images.unsplash.com/photo-1542242194-6301b0b5389a?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1287&q=80" alt="Chipboard texture" class="w-full h-56 object-cover">
                        <div class="p-6">
                            <h3 class="text-xl font-bold mb-2">CHIPBOARD</h3>
                            <p class="text-gray-600 text-sm">Rigid sheets from compressed wood chips and resin, often coated or veneered for furniture and buildings.</p>
                        </div>
                    </div>
                     <!-- Product Card -->
                     <div class="bg-gray-50 rounded-lg shadow-lg overflow-hidden group transform hover:-translate-y-2 transition-transform duration-300 fade-in" style="transition-delay: 100ms;">
                        <img loading="lazy" src="https://images.unsplash.com/photo-1617103994332-9c9786a51270?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1335&q=80" alt="HPL laminate surface" class="w-full h-56 object-cover">
                        <div class="p-6">
                            <h3 class="text-xl font-bold mb-2">HPL</h3>
                            <p class="text-gray-600 text-sm">High-Pressure Decorative laminates used as furniture surface materials or wall paneling.</p>
                        </div>
                    </div>
                     <!-- Product Card -->
                     <div class="bg-gray-50 rounded-lg shadow-lg overflow-hidden group transform hover:-translate-y-2 transition-transform duration-300 fade-in" style="transition-delay: 200ms;">
                        <img loading="lazy" src="https://images.unsplash.com/photo-1593305885472-59c3a333069c?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1287&q=80" alt="Natural wood veneer" class="w-full h-56 object-cover">
                        <div class="p-6">
                            <h3 class="text-xl font-bold mb-2">NATURAL VENEER</h3>
                            <p class="text-gray-600 text-sm">Thin slices of wood, usually thinner than 3 mm, glued onto core panels for doors, cabinets, and furniture.</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>


        <!-- History Section -->
        <section id="history" class="py-20 md:py-32 bg-gray-900 text-white">
            <div class="container mx-auto px-6">
                <div class="text-center mb-16">
                    <h2 class="text-3xl md:text-4xl font-bold mb-4 fade-in">A Legacy Spanning Generations</h2>
                    <p class="text-gray-400 max-w-2xl mx-auto fade-in">The Bozorgi family's business tree from 1889 to the present day.</p>
                </div>
                <!-- Timeline -->
                <div class="relative timeline max-w-4xl mx-auto">
                    <!-- Timeline Item -->
                    <div class="mb-8 flex md:justify-end md:pr-10 relative fade-in">
                        <div class="md:w-1/2">
                            <div class="bg-gray-800 p-6 rounded-lg shadow-lg border-l-4 border-primary-gold">
                                <p class="text-primary-gold font-bold text-lg">1889 - 1951</p>
                                <h3 class="text-2xl font-bold mt-1">BOZORG BOZORGI</h3>
                                <p class="text-gray-300 mt-2">Founder of the timber business, laying the foundation for generations to come.</p>
                            </div>
                        </div>
                    </div>
                    <!-- Timeline Item -->
                    <div class="mb-8 flex md:justify-start md:pl-10 relative fade-in">
                        <div class="md:w-1/2">
                           <div class="bg-gray-800 p-6 rounded-lg shadow-lg border-r-4 md:border-r-0 md:border-l-4 border-primary-gold">
                                <p class="text-primary-gold font-bold text-lg">1909 - 1989</p>
                                <h3 class="text-2xl font-bold mt-1">ALIASGHAR BOZORGI</h3>
                                <p class="text-gray-300 mt-2">Started and grew the local hometown business with timber, building on his father's legacy.</p>
                            </div>
                        </div>
                    </div>
                    <!-- Timeline Item -->
                    <div class="mb-8 flex md:justify-end md:pr-10 relative fade-in">
                        <div class="md:w-1/2">
                           <div class="bg-gray-800 p-6 rounded-lg shadow-lg border-l-4 border-primary-gold">
                                <p class="text-primary-gold font-bold text-lg">1951 - 1990</p>
                                <h3 class="text-2xl font-bold mt-1">MUHAMMADALI BOZORGI</h3>
                                <p class="text-gray-300 mt-2">Expanded the local business, increasing its reach and influence in the region.</p>
                            </div>
                        </div>
                    </div>
                    <!-- Timeline Item -->
                    <div class="mb-8 flex md:justify-start md:pl-10 relative fade-in">
                        <div class="md:w-1/2">
                           <div class="bg-gray-800 p-6 rounded-lg shadow-lg border-r-4 md:border-r-0 md:border-l-4 border-primary-gold">
                                <p class="text-primary-gold font-bold text-lg">1988 - Present</p>
                                <h3 class="text-2xl font-bold mt-1">ALI BOZORGI</h3>
                                <p class="text-gray-300 mt-2">A revolutionary leader who introduced global trading with hi-tech materials. CEO at BBMTCo, making the AliBozorgi brand number one.</p>
                            </div>
                        </div>
                    </div>
                     <!-- Timeline Item -->
                     <div class="mb-8 flex md:justify-end md:pr-10 relative fade-in">
                        <div class="md:w-1/2">
                           <div class="bg-gray-800 p-6 rounded-lg shadow-lg border-l-4 border-primary-gold">
                                <p class="text-primary-gold font-bold text-lg">2020 - Now</p>
                                <h3 class="text-2xl font-bold mt-1">ALIASGHAR BOZORGI</h3>
                                <p class="text-gray-300 mt-2">Carrying the torch forward with Bozorgi Group, building on a rich family history of entrepreneurship and integrity.</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>


        <!-- Humanity First Section -->
        <section id="humanity" class="py-20 md:py-32 bg-gray-50">
            <div class="container mx-auto px-6">
                <div class="text-center mb-16">
                    <h2 class="text-3xl md:text-4xl font-bold text-gray-900 mb-4 fade-in">Humanity First!</h2>
                     <p class="text-gray-600 max-w-2xl mx-auto fade-in">We believe in sharing our success with the community and supporting causes that make a difference.</p>
                </div>
                <div class="grid md:grid-cols-2 gap-10 max-w-5xl mx-auto">
                    <!-- Charity Card 1 -->
                    <div class="bg-white p-8 rounded-lg shadow-xl text-center transform hover:scale-105 transition-transform duration-300 fade-in">
                        <div class="text-primary-gold mb-4">
                            <svg xmlns="http://www.w3.org/2000/svg" class="h-16 w-16 mx-auto" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="1"><path stroke-linecap="round" stroke-linejoin="round" d="M12 8v4l3 3m6-3a9 9 0 11-18 0 9 9 0 0118 0z" /></svg>
                        </div>
                        <h3 class="text-2xl font-bold mb-3">Supporting Abu-Ali Sina Hospital</h3>
                        <p class="text-gray-600 mb-6">Contributing to the establishment of an efficient organ transplant center to help the increasing number of patients in need.</p>
                        <a href="http://en.abualisina.net" target="_blank" rel="noopener noreferrer" class="font-bold text-primary-gold hover:text-accent-bronze transition">Visit Website &rarr;</a>
                    </div>
                    <!-- Charity Card 2 -->
                    <div class="bg-white p-8 rounded-lg shadow-xl text-center transform hover:scale-105 transition-transform duration-300 fade-in" style="transition-delay: 200ms;">
                        <div class="text-primary-gold mb-4">
                            <svg xmlns="http://www.w3.org/2000/svg" class="h-16 w-16 mx-auto" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="1"><path d="M12 14l9-5-9-5-9 5 9 5z" /><path d="M12 14l6.16-3.422a12.083 12.083 0 01.665 6.479A11.952 11.952 0 0012 20.055a11.952 11.952 0 00-6.824-5.998 12.078 12.078 0 01.665-6.479L12 14z" /><path stroke-linecap="round" stroke-linejoin="round" d="M12 14l9-5-9-5-9 5 9 5zm0 0l6.16-3.422a12.083 12.083 0 01.665 6.479A11.952 11.952 0 0012 20.055a11.952 11.952 0 00-6.824-5.998 12.078 12.078 0 01.665-6.479L12 14zm-4 6v-7.5l4-2.222 4 2.222V20M12 12.778L16.748 10 12 7.222 7.252 10 12 12.778z" /></svg>
                        </div>
                        <h3 class="text-2xl font-bold mb-3">Mohammad Ali Bozorgi Highschool</h3>
                        <p class="text-gray-600 mb-6">Founded in 1996 in Shiraz by Bozorgi Group to invest in the future by providing quality education for the next generation.</p>
                    </div>
                </div>
            </div>
        </section>
    </main>

    <!-- Footer -->
    <footer id="contact" class="bg-black text-white pt-20 pb-8">
        <div class="container mx-auto px-6">
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-10 mb-10">
                <!-- Column 1: About -->
                <div class="fade-in">
                    <img src="https://lh3.googleusercontent.com/MQ1BMU25DGoAOhOlCsZz9oQ1HYJog_nHwoKyd5XyETcxWCoOpHhgduAD65Puw8PmhOvOOrJz6n8fN_nvJb437_cFNh1RNaNKenmI41ed3amHqDdPvucCajH1nTNzudc2orCfteU-4nDogbznW0Oa2YVihzwv6gHRwaJ-eArEC9Ye0FfmbaD2vg=w1280" alt="Bozorgi Group Logo" class="h-12 mb-4">
                    <p class="text-gray-400">A global leader in building materials trading, committed to quality, integrity, and customer satisfaction since 1889.</p>
                </div>
                <!-- Column 2: Quick Links -->
                <div class="fade-in" style="transition-delay: 100ms;">
                    <h4 class="text-xl font-bold mb-4">Quick Links</h4>
                    <ul class="space-y-2">
                        <li><a href="#about" class="text-gray-400 hover:text-primary-gold transition">About Us</a></li>
                        <li><a href="#products" class="text-gray-400 hover:text-primary-gold transition">Our Products</a></li>
                        <li><a href="#history" class="text-gray-400 hover:text-primary-gold transition">Our History</a></li>
                        <li><a href="#humanity" class="text-gray-400 hover:text-primary-gold transition">Humanity First</a></li>
                    </ul>
                </div>
                <!-- Column 3: Contact Info -->
                <div class="fade-in" style="transition-delay: 200ms;">
                    <h4 class="text-xl font-bold mb-4">Contact Us</h4>
                    <ul class="space-y-3 text-gray-400">
                        <li class="flex items-start">
                             <svg class="w-5 h-5 mr-3 mt-1 flex-shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z"></path><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 11a3 3 0 11-6 0 3 3 0 016 0z"></path></svg>
                           <span>Dubai - UAE<br>Business Bay, Al Manara Tower<br>8th floor, Office No. 802<br>P.O.Box: 124361</span>
                        </li>
                        <li class="flex items-center">
                            <svg class="w-5 h-5 mr-3 flex-shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.13a11.042 11.042 0 005.516 5.516l1.13-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-1C9.716 21 3 14.284 3 6V5z"></path></svg>
                            <a href="tel:+97143213030" class="hover:text-primary-gold">+971 4 321 3030</a>
                        </li>
                         <li class="flex items-center">
                            <svg class="w-5 h-5 mr-3 flex-shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 18h.01M8 21h8a2 2 0 002-2V5a2 2 0 00-2-2H8a2 2 0 00-2 2v14a2 2 0 002 2z"></path></svg>
                            <a href="tel:+971523952892" class="hover:text-primary-gold">+971 52 395 2892</a>
                        </li>
                        <li class="flex items-center">
                            <svg class="w-5 h-5 mr-3 flex-shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"></path></svg>
                            <a href="mailto:info@bozorgigroup.com" class="hover:text-primary-gold">info@bozorgigroup.com</a>
                        </li>
                    </ul>
                </div>
                 <!-- Column 4: Social -->
                <div class="fade-in" style="transition-delay: 300ms;">
                    <h4 class="text-xl font-bold mb-4">Follow Us</h4>
                    <p class="text-gray-400 mb-4">Stay connected on our social networks.</p>
                    <div class="flex space-x-4">
                        <a href="https://www.facebook.com/AliBozorgiofficial/" target="_blank" rel="noopener noreferrer" aria-label="Facebook" class="text-gray-400 hover:text-primary-gold transition">
                           <svg class="w-7 h-7" fill="currentColor" viewBox="0 0 24 24"><path d="M9 8h-3v4h3v12h5v-12h3.642l.358-4h-4v-1.667c0-.955.192-1.333 1.115-1.333h2.885v-5h-3.808c-3.596 0-5.192 1.583-5.192 4.615v2.385z"/></svg>
                        </a>
                        <a href="https://x.com/aliabozorgi" target="_blank" rel="noopener noreferrer" aria-label="Twitter" class="text-gray-400 hover:text-primary-gold transition">
                            <svg class="w-7 h-7" fill="currentColor" viewBox="0 0 24 24"><path d="M18.244 2.25h3.308l-7.227 8.26 8.502 11.24H16.17l-5.214-6.817L4.99 21.75H1.68l7.73-8.835L1.254 2.25H8.08l4.713 6.231zm-1.161 17.52h1.833L7.084 4.126H5.117z"/></svg>
                        </a>
                        <a href="https://www.instagram.com/alibozorgi.uae" target="_blank" rel="noopener noreferrer" aria-label="Instagram" class="text-gray-400 hover:text-primary-gold transition">
                            <svg class="w-7 h-7" fill="currentColor" viewBox="0 0 24 24"><path d="M12 2.163c3.204 0 3.584.012 4.85.07 3.252.148 4.771 1.691 4.919 4.919.058 1.265.069 1.645.069 4.85s-.012 3.584-.07 4.85c-.148 3.225-1.664 4.771-4.919 4.919-1.266.058-1.644.07-4.85.07s-3.584-.012-4.85-.07c-3.252-.148-4.771-1.699-4.919-4.92-.058-1.265-.07-1.644-.07-4.85s.012-3.584.07-4.85c.148-3.225 1.664-4.771 4.919-4.919 1.266-.057 1.645-.069 4.85-.069zm0-2.163c-3.259 0-3.667.014-4.947.072-4.358.2-6.78 2.618-6.98 6.98-.059 1.281-.073 1.689-.073 4.948s.014 3.667.072 4.947c.2 4.358 2.618 6.78 6.98 6.98 1.281.058 1.689.072 4.948.072s3.667-.014 4.947-.072c4.354-.2 6.782-2.618 6.979-6.98.059-1.28.073-1.689.073-4.947s-.014-3.667-.072-4.947c-.196-4.354-2.617-6.78-6.979-6.98-1.281-.059-1.689-.073-4.948-.073zm0 5.838c-3.403 0-6.162 2.759-6.162 6.162s2.759 6.162 6.162 6.162 6.162-2.759 6.162-6.162-2.759-6.162-6.162-6.162zm0 10.162c-2.209 0-4-1.79-4-4s1.791-4 4-4 4 1.79 4 4-1.791 4-4 4zm6.406-11.845c-.796 0-1.441.645-1.441 1.44s.645 1.44 1.441 1.44 1.441-.645 1.441-1.44c0-.795-.645-1.44-1.441-1.44z"/></svg>
                        </a>
                    </div>
                </div>
            </div>
            <div class="border-t border-gray-800 pt-6 mt-10 text-center text-gray-500 text-sm">
                <p>&copy; <span id="current-year"></span> Bozorgi Group. All Rights Reserved.</p>
            </div>
        </div>
    </footer>


    <script>
        document.addEventListener('DOMContentLoaded', function() {
            // Mobile Menu Toggle
            const mobileMenuButton = document.getElementById('mobile-menu-button');
            const mobileMenu = document.getElementById('mobile-menu');
            mobileMenuButton.addEventListener('click', () => {
                mobileMenu.classList.toggle('hidden');
            });

            // Close mobile menu when a link is clicked
            const mobileNavLinks = mobileMenu.querySelectorAll('a');
            mobileNavLinks.forEach(link => {
                link.addEventListener('click', () => {
                    mobileMenu.classList.add('hidden');
                });
            });

            // Set current year in footer
            document.getElementById('current-year').textContent = new Date().getFullYear();

            // Intersection Observer for fade-in animations
            const faders = document.querySelectorAll('.fade-in');
            const appearOptions = {
                threshold: 0.2, // Trigger when 20% of the element is visible
                rootMargin: "0px 0px -50px 0px" // Start animation a bit later
            };

            const appearOnScroll = new IntersectionObserver(function(entries, appearOnScroll) {
                entries.forEach(entry => {
                    if (!entry.isIntersecting) {
                        return;
                    } else {
                        entry.target.classList.add('visible');
                        appearOnScroll.unobserve(entry.target);
                    }
                });
            }, appearOptions);

            faders.forEach(fader => {
                appearOnScroll.observe(fader);
            });
        });
    </script>
</body>
</html>
```