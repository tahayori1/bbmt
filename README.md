Of course. Here is a comprehensive, single-file website template for Bozorgi Group, built with expert principles in design, user experience, and SEO.

This template includes a sticky header, a captivating hero section, detailed content areas for products, company history, and philanthropic efforts, and a professional dark footer. It is fully responsive, interactive, and optimized for performance and search engines.

Simply save the following code as an `index.html` file and open it in your browser.

```html
<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    
    <!-- SEO Meta Tags -->
    <title>Bozorgi Group | Premium Building Materials Since 1889</title>
    <meta name="description" content="Bozorgi Group, a leading trading company since 1988, specializes in supplying high-quality building materials including MDF, HDF, Hardwood, and more. Business Without Boundary.">
    <meta name="keywords" content="Bozorgi Group, Building Materials, MDF, HDF, Polywood, Hardwood, Chipboard, HPL, Natural Veneer, Wood Products, Dubai, UAE">
    <meta name="author" content="Bozorgi Group">
    <link rel="canonical" href="https://www.bozorgigroup.com">
    <link rel="icon" href="https://lh3.googleusercontent.com/MQ1BMU25DGoAOhOlCsZz9oQ1HYJog_nHwoKyd5XyETcxWCoOpHhgduAD65Puw8PmhOvOOrJz6n8fN_nvJb437_cFNh1RNaNKenmI41ed3amHqDdPvucCajH1nTNzudc2orCfteU-4nDogbznW0Oa2YVihzwv6gHRwaJ-eArEC9Ye0FfmbaD2vg=w1280">

    <!-- Open Graph / Facebook -->
    <meta property="og:type" content="website">
    <meta property="og:url" content="https://www.bozorgigroup.com">
    <meta property="og:title" content="Bozorgi Group | Premium Building Materials Since 1889">
    <meta property="og:description" content="Supplying premium building materials worldwide with a legacy of quality and trust. Explore our range of MDF, HDF, Hardwood, and more.">
    <meta property="og:image" content="https://lh3.googleusercontent.com/MQ1BMU25DGoAOhOlCsZz9oQ1HYJog_nHwoKyd5XyETcxWCoOpHhgduAD65Puw8PmhOvOOrJz6n8fN_nvJb437_cFNh1RNaNKenmI41ed3amHqDdPvucCajH1nTNzudc2orCfteU-4nDogbznW0Oa2YVihzwv6gHRwaJ-eArEC9Ye0FfmbaD2vg=w1280">

    <!-- Twitter -->
    <meta property="twitter:card" content="summary_large_image">
    <meta property="twitter:url" content="https://www.bozorgigroup.com">
    <meta property="twitter:title" content="Bozorgi Group | Premium Building Materials Since 1889">
    <meta property="twitter:description" content="Supplying premium building materials worldwide with a legacy of quality and trust. Explore our range of MDF, HDF, Hardwood, and more.">
    <meta property="twitter:image" content="https://lh3.googleusercontent.com/MQ1BMU25DGoAOhOlCsZz9oQ1HYJog_nHwoKyd5XyETcxWCoOpHhgduAD65Puw8PmhOvOOrJz6n8fN_nvJb437_cFNh1RNaNKenmI41ed3amHqDdPvucCajH1nTNzudc2orCfteU-4nDogbznW0Oa2YVihzwv6gHRwaJ-eArEC9Ye0FfmbaD2vg=w1280">

    <!-- Tailwind CSS via CDN -->
    <script src="https://cdn.tailwindcss.com"></script>

    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">

    <!-- Custom CSS and Tailwind Configuration -->
    <style type="text/tailwindcss">
        @layer base {
            body {
                font-family: 'Poppins', sans-serif;
            }
            .section-padding {
                @apply py-16 sm:py-24 px-6 lg:px-8;
            }
            .section-title {
                @apply text-3xl font-bold tracking-tight text-black sm:text-4xl text-center;
            }
            .section-subtitle {
                @apply mt-2 text-lg leading-8 text-gray-600 text-center;
            }
        }
        @layer components {
            .cta-button-primary {
                @apply rounded-md bg-gold px-4 py-2.5 text-sm font-semibold text-black shadow-sm hover:bg-bronze focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-gold transition-colors duration-300;
            }
            .cta-button-secondary {
                @apply rounded-md border border-gold px-4 py-2.5 text-sm font-semibold text-gold shadow-sm hover:bg-gold hover:text-black focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-gold transition-colors duration-300;
            }
            .nav-link {
                @apply text-sm font-semibold leading-6 text-black hover:text-gold transition-colors;
            }
            .product-card {
                @apply bg-white p-8 rounded-lg shadow-lg transform hover:-translate-y-2 transition-transform duration-300 border-t-4 border-gold;
            }
            .timeline-item {
                @apply relative pl-8 sm:pl-32 py-6 group;
            }
            .timeline-item:last-child {
                @apply pb-0;
            }
            .timeline-item::before {
                @apply content-[''] absolute left-0 sm:left-12 top-5 w-px h-full bg-gray-300;
            }
            .timeline-item:last-child::before {
                @apply h-0;
            }
            .timeline-marker {
                @apply content-[''] absolute left-[-5.5px] sm:left-[42.5px] top-5 w-3 h-3 rounded-full bg-gray-300 group-hover:bg-gold transition-colors;
            }

            /* Scroll Animations */
            .reveal {
                opacity: 0;
                transform: translateY(30px);
                transition: opacity 0.6s ease-out, transform 0.6s ease-out;
            }
            .reveal-visible {
                opacity: 1;
                transform: translateY(0);
            }
        }
    </style>
    <script>
      tailwind.config = {
        theme: {
          extend: {
            colors: {
              gold: '#D4AF37',
              bronze: '#B88714',
              'primary-black': '#000000',
            }
          }
        }
      }
    </script>
    
    <!-- Structured Data (JSON-LD) -->
    <script type="application/ld+json">
    {
      "@context": "https://schema.org",
      "@type": "Organization",
      "name": "Bozorgi Group",
      "url": "https://www.bozorgigroup.com",
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
        "streetAddress": "Business Bay Street . Marasi Dr Al Manara Tower 8 floor office No. 802",
        "addressLocality": "Dubai",
        "postalCode": "124361",
        "addressCountry": "AE"
      },
      "sameAs": [
        "https://www.facebook.com/AliBozorgiofficial/",
        "https://x.com/aliabozorgi",
        "https://www.instagram.com/alibozorgi.uae"
      ]
    }
    </script>

</head>
<body class="bg-gray-50 text-gray-800 antialiased">
    <!-- Header -->
    <header id="header" class="bg-white/80 backdrop-blur-md fixed top-0 left-0 right-0 z-50 transition-shadow duration-300">
        <nav class="mx-auto flex max-w-7xl items-center justify-between p-6 lg:px-8" aria-label="Global">
            <a href="#home" class="flex items-center -m-1.5 p-1.5">
                <span class="sr-only">Bozorgi Group</span>
                <img class="h-10 w-auto" src="https://lh3.googleusercontent.com/MQ1BMU25DGoAOhOlCsZz9oQ1HYJog_nHwoKyd5XyETcxWCoOpHhgduAD65Puw8PmhOvOOrJz6n8fN_nvJb437_cFNh1RNaNKenmI41ed3amHqDdPvucCajH1nTNzudc2orCfteU-4nDogbznW0Oa2YVihzwv6gHRwaJ-eArEC9Ye0FfmbaD2vg=w1280" alt="Bozorgi Group Logo">
            </a>
            <div class="flex lg:hidden">
                <button type="button" id="mobile-menu-button" class="-m-2.5 inline-flex items-center justify-center rounded-md p-2.5 text-gray-700">
                    <span class="sr-only">Open main menu</span>
                    <svg class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" aria-hidden="true">
                        <path stroke-linecap="round" stroke-linejoin="round" d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5" />
                    </svg>
                </button>
            </div>
            <div class="hidden lg:flex lg:gap-x-12">
                <a href="#home" class="nav-link nav-item">Home</a>
                <a href="#products" class="nav-link nav-item">Products</a>
                <a href="#about" class="nav-link nav-item">About Us</a>
                <a href="#history" class="nav-link nav-item">Our History</a>
                <a href="#humanity" class="nav-link nav-item">Humanity First</a>
            </div>
            <div class="hidden lg:flex lg:flex-1 lg:justify-end">
                <a href="#contact" class="cta-button-primary">Quick Contact</a>
            </div>
        </nav>
        <!-- Mobile menu, show/hide based on menu open state. -->
        <div id="mobile-menu" class="hidden lg:hidden" role="dialog" aria-modal="true">
            <div class="fixed inset-0 z-50"></div>
            <div class="fixed inset-y-0 right-0 z-50 w-full overflow-y-auto bg-white px-6 py-6 sm:max-w-sm sm:ring-1 sm:ring-gray-900/10">
                <div class="flex items-center justify-between">
                    <a href="#home" class="-m-1.5 p-1.5">
                        <span class="sr-only">Bozorgi Group</span>
                        <img class="h-8 w-auto" src="https://lh3.googleusercontent.com/MQ1BMU25DGoAOhOlCsZz9oQ1HYJog_nHwoKyd5XyETcxWCoOpHhgduAD65Puw8PmhOvOOrJz6n8fN_nvJb437_cFNh1RNaNKenmI41ed3amHqDdPvucCajH1nTNzudc2orCfteU-4nDogbznW0Oa2YVihzwv6gHRwaJ-eArEC9Ye0FfmbaD2vg=w1280" alt="">
                    </a>
                    <button type="button" id="mobile-menu-close-button" class="-m-2.5 rounded-md p-2.5 text-gray-700">
                        <span class="sr-only">Close menu</span>
                        <svg class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" aria-hidden="true">
                            <path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12" />
                        </svg>
                    </button>
                </div>
                <div class="mt-6 flow-root">
                    <div class="-my-6 divide-y divide-gray-500/10">
                        <div class="space-y-2 py-6">
                            <a href="#home" class="-mx-3 block rounded-lg px-3 py-2 text-base font-semibold leading-7 text-gray-900 hover:bg-gray-50 mobile-nav-item">Home</a>
                            <a href="#products" class="-mx-3 block rounded-lg px-3 py-2 text-base font-semibold leading-7 text-gray-900 hover:bg-gray-50 mobile-nav-item">Products</a>
                            <a href="#about" class="-mx-3 block rounded-lg px-3 py-2 text-base font-semibold leading-7 text-gray-900 hover:bg-gray-50 mobile-nav-item">About Us</a>
                            <a href="#history" class="-mx-3 block rounded-lg px-3 py-2 text-base font-semibold leading-7 text-gray-900 hover:bg-gray-50 mobile-nav-item">Our History</a>
                            <a href="#humanity" class="-mx-3 block rounded-lg px-3 py-2 text-base font-semibold leading-7 text-gray-900 hover:bg-gray-50 mobile-nav-item">Humanity First</a>
                        </div>
                        <div class="py-6">
                            <a href="#contact" class="w-full text-center cta-button-primary mobile-nav-item">Quick Contact</a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </header>

    <main>
        <!-- Hero Section -->
        <section id="home" class="relative bg-black isolate pt-14">
            <div class="absolute inset-x-0 -top-40 -z-10 transform-gpu overflow-hidden blur-3xl sm:-top-80" aria-hidden="true">
                <div class="relative left-[calc(50%-11rem)] aspect-[1155/678] w-[36.125rem] -translate-x-1/2 rotate-[30deg] bg-gradient-to-tr from-[#D4AF37] to-[#B88714] opacity-20 sm:left-[calc(50%-30rem)] sm:w-[72.1875rem]" style="clip-path: polygon(74.1% 44.1%, 100% 61.6%, 97.5% 26.9%, 85.5% 0.1%, 80.7% 2%, 72.5% 32.5%, 60.2% 62.4%, 52.4% 68.1%, 47.5% 58.3%, 45.2% 34.5%, 27.5% 76.7%, 0.1% 64.9%, 17.9% 100%, 27.6% 76.8%, 76.1% 97.7%, 74.1% 44.1%)"></div>
            </div>
            <div class="py-24 sm:py-32 lg:pb-40">
                <div class="mx-auto max-w-7xl px-6 lg:px-8">
                    <div class="mx-auto max-w-3xl text-center">
                        <h1 class="text-4xl font-bold tracking-tight text-white sm:text-6xl">Building on a Legacy of Quality</h1>
                        <p class="mt-6 text-lg leading-8 text-gray-300">"Business Without Boundary" — Supplying premium wood and building materials worldwide since 1889, blending tradition with modern excellence.</p>
                        <div class="mt-10 flex items-center justify-center gap-x-6">
                            <a href="#products" class="cta-button-primary">Our Products</a>
                            <a href="#about" class="cta-button-secondary">Learn More &rarr;</a>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Products Section -->
        <section id="products" class="section-padding bg-white">
            <div class="mx-auto max-w-7xl">
                <div class="text-center reveal">
                    <h2 class="section-title">Our Premium Product Range</h2>
                    <p class="section-subtitle">Engineered for excellence, our materials are the foundation of quality construction.</p>
                </div>
                <div class="mt-16 grid grid-cols-1 gap-8 md:grid-cols-2 lg:grid-cols-3">
                    <div class="product-card reveal">
                        <h3 class="text-xl font-semibold text-black">MDF</h3>
                        <p class="mt-2 text-gray-600">Medium-Density Fibreboard, an engineered wood product made from broken down hardwood or softwood residuals, wax, and a resin binder.</p>
                    </div>
                    <div class="product-card reveal" style="transition-delay: 100ms;">
                        <h3 class="text-xl font-semibold text-black">HDF</h3>
                        <p class="mt-2 text-gray-600">High-Density Fibreboard (Hardboard) is a type of fiberboard, which is an engineered wood product known for its durability and strength.</p>
                    </div>
                    <div class="product-card reveal" style="transition-delay: 200ms;">
                        <h3 class="text-xl font-semibold text-black">POLYWOOD</h3>
                        <p class="mt-2 text-gray-600">Made from thermoformed plastics and derived from post-consumer bottle waste. A sustainable and highly durable choice.</p>
                    </div>
                    <div class="product-card reveal" style="transition-delay: 0ms;">
                        <h3 class="text-xl font-semibold text-black">HARDWOOD</h3>
                        <p class="mt-2 text-gray-600">Sourced from dicot trees in broad-leaved temperate and tropical forests. Known for its natural beauty and long-lasting performance.</p>
                    </div>
                    <div class="product-card reveal" style="transition-delay: 100ms;">
                        <h3 class="text-xl font-semibold text-black">CHIPBOARD</h3>
                        <p class="mt-2 text-gray-600">Rigid sheets made from compressed wood chips and resin, often coated or veneered, used widely in furniture and buildings.</p>
                    </div>
                    <div class="product-card reveal" style="transition-delay: 200ms;">
                        <h3 class="text-xl font-semibold text-black">HPL & Natural Veneer</h3>
                        <p class="mt-2 text-gray-600">High-Pressure Decorative Laminates and thin slices of natural wood, perfect for furniture surfaces, wall paneling, and doors.</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- About Us Section -->
        <section id="about" class="section-padding">
            <div class="mx-auto max-w-7xl">
                <div class="grid grid-cols-1 gap-y-16 lg:grid-cols-2 lg:gap-x-16">
                    <div class="reveal">
                        <h2 class="text-3xl font-bold tracking-tight text-black sm:text-4xl text-left">About Bozorgi Group</h2>
                        <p class="mt-4 text-gray-600">Bozorgi Building Material Company, operating under the brand BOZORGI GROUP since 1988, was founded on the motto “Business Without Boundary“. We specialize in the global trade, export, and import of authorized goods, with a core focus on high-quality building materials.</p>
                        <p class="mt-4 text-gray-600">Our competitive advantage lies in our customer-centric approach, building win-win relationships, and leveraging a vast network of suppliers to meet demands efficiently. The trust of our customers and suppliers is our greatest asset and the cornerstone of our strength.</p>
                        <a href="#contact" class="mt-6 inline-block cta-button-primary">Partner with Us</a>
                    </div>
                    <div class="space-y-8 reveal" style="transition-delay: 200ms;">
                        <div class="bg-white p-6 rounded-lg shadow-md border-l-4 border-gold">
                            <h3 class="text-lg font-semibold text-black">Our Vision</h3>
                            <p class="mt-2 text-gray-600">To be a leading business and trading company in Building Materials by upholding our values of honesty and transparency on both national and international fronts.</p>
                        </div>
                        <div class="bg-white p-6 rounded-lg shadow-md border-l-4 border-bronze">
                            <h3 class="text-lg font-semibold text-black">Our Mission</h3>
                            <p class="mt-2 text-gray-600">To supply premium building materials with the best services and prices, satisfying our customers and expanding our business through experienced teams and modern systems.</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- History Section -->
        <section id="history" class="section-padding bg-white">
            <div class="mx-auto max-w-4xl">
                <div class="text-center reveal">
                    <h2 class="section-title">A Legacy Forged Through Generations</h2>
                    <p class="section-subtitle">Our history is the bedrock of our business. A family tree rooted in timber since 1889.</p>
                </div>
                <div class="mt-16 flow-root">
                    <div role="list" class="-mb-8">
                        <!-- Timeline Item -->
                        <div class="timeline-item reveal">
                           <span class="timeline-marker"></span>
                            <div class="flex-grow sm:ml-12">
                                <p class="text-sm text-gray-500">1889 - 1951</p>
                                <h4 class="font-bold text-lg text-black mt-1">Bozorg Bozorgi</h4>
                                <p class="text-gray-600">Founder of the timber business, laying the groundwork for a century-spanning legacy.</p>
                            </div>
                        </div>
                        <!-- Timeline Item -->
                        <div class="timeline-item reveal">
                           <span class="timeline-marker"></span>
                            <div class="flex-grow sm:ml-12">
                                <p class="text-sm text-gray-500">1909 - 1989</p>
                                <h4 class="font-bold text-lg text-black mt-1">Aliasghar Bozorgi</h4>
                                <p class="text-gray-600">Transformed the local hometown business with timber, beginning its journey of growth.</p>
                            </div>
                        </div>
                         <!-- Timeline Item -->
                        <div class="timeline-item reveal">
                           <span class="timeline-marker"></span>
                            <div class="flex-grow sm:ml-12">
                                <p class="text-sm text-gray-500">1951 - 1990</p>
                                <h4 class="font-bold text-lg text-black mt-1">Muhammadali Bozorgi</h4>
                                <p class="text-gray-600">Championed the expansion of the local business, increasing its reach and reputation.</p>
                            </div>
                        </div>
                         <!-- Timeline Item -->
                        <div class="timeline-item reveal">
                           <span class="timeline-marker"></span>
                            <div class="flex-grow sm:ml-12">
                                <p class="text-sm text-gray-500">1988 - Present</p>
                                <h4 class="font-bold text-lg text-black mt-1">Ali Bozorgi</h4>
                                <p class="text-gray-600">A revolutionary leader who introduced the idea of global trading with hi-tech materials, making AliBozorgi a number one brand.</p>
                            </div>
                        </div>
                        <!-- Timeline Item -->
                        <div class="timeline-item reveal">
                           <span class="timeline-marker"></span>
                            <div class="flex-grow sm:ml-12">
                                <p class="text-sm text-gray-500">2020 - Now</p>
                                <h4 class="font-bold text-lg text-black mt-1">Aliasghar Bozorgi & Bozorgi Group</h4>
                                <p class="text-gray-600">After years as a partner and consultant, the next generation continues the legacy under the unified Bozorgi Group banner.</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Humanity First Section -->
        <section id="humanity" class="section-padding">
            <div class="mx-auto max-w-7xl">
                <div class="text-center reveal">
                     <h2 class="text-3xl font-bold tracking-tight text-gold sm:text-4xl text-center">HUMANITY FIRST!</h2>
                    <p class="section-subtitle">We believe in sharing our success with the community. It's not just business; it's about building a better world.</p>
                </div>
                <div class="mt-16 grid grid-cols-1 gap-8 md:grid-cols-2">
                    <div class="bg-white p-8 rounded-lg shadow-md reveal">
                         <img src="https://images.unsplash.com/photo-1581093450021-4a7360e9a1local?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1170&q=80" alt="Abu-Ali Sina Hospital" class="rounded-md object-cover h-48 w-full mb-6" loading="lazy" width="500" height="300">
                        <h3 class="text-xl font-semibold text-black">Supporting Abu-Ali Sina Hospital</h3>
                        <p class="mt-2 text-gray-600">We proudly support the Organ Transplantation Center at Abu Ali Sina Hospital, aiding their vital work in saving lives through efficient organ transplantation.</p>
                        <a href="http://en.abualisina.net" target="_blank" rel="noopener noreferrer" class="font-semibold text-gold hover:text-bronze mt-4 inline-block">Visit Website &rarr;</a>
                    </div>
                    <div class="bg-white p-8 rounded-lg shadow-md reveal" style="transition-delay: 200ms;">
                        <img src="https://images.unsplash.com/photo-1562774053-701939374585?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1172&q=80" alt="Mohammad Ali Bozorgi Highschool" class="rounded-md object-cover h-48 w-full mb-6" loading="lazy" width="500" height="300">
                        <h3 class="text-xl font-semibold text-black">Mohammad Ali Bozorgi Highschool</h3>
                        <p class="mt-2 text-gray-600">Founded in 1996 in Shiraz by Bozorgi Group, this high school is our commitment to empowering the next generation through education.</p>
                    </div>
                </div>
            </div>
        </section>
    </main>

    <!-- Footer -->
    <footer id="contact" class="bg-primary-black text-white section-padding" aria-labelledby="footer-heading">
        <h2 id="footer-heading" class="sr-only">Footer</h2>
        <div class="mx-auto max-w-7xl">
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-12">
                <!-- Company Info -->
                <div class="md:col-span-2 lg:col-span-1">
                    <img class="h-12 w-auto" src="https://lh3.googleusercontent.com/MQ1BMU25DGoAOhOlCsZz9oQ1HYJog_nHwoKyd5XyETcxWCoOpHhgduAD65Puw8PmhOvOOrJz6n8fN_nvJb437_cFNh1RNaNKenmI41ed3amHqDdPvucCajH1nTNzudc2orCfteU-4nDogbznW0Oa2YVihzwv6gHRwaJ-eArEC9Ye0FfmbaD2vg=w1280" alt="Bozorgi Group Logo">
                    <p class="mt-4 text-sm leading-6 text-gray-300">A global leader in building materials trading, committed to excellence, integrity, and customer satisfaction since 1988.</p>
                </div>
                <!-- Contact Details -->
                <div>
                   <h3 class="text-base font-semibold leading-6 text-gold">Get in Touch</h3>
                   <ul role="list" class="mt-6 space-y-4">
                       <li class="flex items-start">
                           <svg class="h-5 w-5 text-gold mt-1 flex-shrink-0" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" fill="currentColor" aria-hidden="true"><path fill-rule="evenodd" d="M9.69 18.933l.003.001C9.89 19.02 10 19 10 19s.11.02.308-.066l.002-.001.006-.003.018-.008a5.741 5.741 0 00.281-.14c.186-.1.4-.27.615-.454L16 14.55V9.5a6 6 0 10-12 0v5.05l5.095 4.095zM10 12a2 2 0 100-4 2 2 0 000 4z" clip-rule="evenodd" /></svg>
                           <span class="ml-3 text-sm text-gray-300">Dubai, UAE <br>Business Bay, Marasi Dr <br>Al Manara Tower, 8th Floor, Office 802 <br>P.O.Box: 124361</span>
                       </li>
                       <li class="flex items-center">
                            <svg class="h-5 w-5 text-gold flex-shrink-0" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" fill="currentColor" aria-hidden="true"><path d="M2 3.5A1.5 1.5 0 013.5 2h1.148a1.5 1.5 0 011.465 1.175l.716 3.223a1.5 1.5 0 01-1.052 1.767l-.933.267c-.41.117-.643.555-.48.95a11.542 11.542 0 006.254 6.254c.395.163.833-.07.95-.48l.267-.933a1.5 1.5 0 011.767-1.052l3.223.716A1.5 1.5 0 0118 15.352V16.5a1.5 1.5 0 01-1.5 1.5h-1.5A13.5 13.5 0 012 3.5z" /></svg>
                            <a href="tel:+971523952892" class="ml-3 text-sm text-gray-300 hover:text-gold">+971 52 395 2892</a>
                       </li>
                       <li class="flex items-center">
                             &nbsp;<span class="sr-only">Phone</span>
                            <a href="tel:+97143213030" class="ml-9 text-sm text-gray-300 hover:text-gold">+971 4 321 3030</a>
                       </li>
                       <li class="flex items-center">
                            <svg class="h-5 w-5 text-gold flex-shrink-0" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" fill="currentColor"><path d="M3 4a2 2 0 00-2 2v1.161l8.441 4.221a1.25 1.25 0 001.118 0L19 7.162V6a2 2 0 00-2-2H3z" /><path d="M19 8.839l-7.77 3.885a2.75 2.75 0 01-2.46 0L1 8.839V14a2 2 0 002 2h14a2 2 0 002-2V8.839z" /></svg>
                            <a href="mailto:info@bozorgigroup.com" class="ml-3 text-sm text-gray-300 hover:text-gold">info@bozorgigroup.com</a>
                       </li>
                   </ul>
                </div>
                <!-- Quick Links -->
                <div>
                   <h3 class="text-base font-semibold leading-6 text-gold">Quick Links</h3>
                   <ul role="list" class="mt-6 space-y-4">
                       <li><a href="#products" class="text-sm leading-6 text-gray-300 hover:text-gold">Products</a></li>
                       <li><a href="#about" class="text-sm leading-6 text-gray-300 hover:text-gold">About Us</a></li>
                       <li><a href="#history" class="text-sm leading-6 text-gray-300 hover:text-gold">Our History</a></li>
                       <li><a href="#humanity" class="text-sm leading-6 text-gray-300 hover:text-gold">Humanity First</a></li>
                   </ul>
                </div>
                <!-- Social Media -->
                <div>
                   <h3 class="text-base font-semibold leading-6 text-gold">Follow Us</h3>
                   <div class="flex space-x-6 mt-6">
                       <a href="https://www.facebook.com/AliBozorgiofficial/" target="_blank" rel="noopener noreferrer" class="text-gray-400 hover:text-gold">
                           <span class="sr-only">Facebook</span>
                           <svg class="h-6 w-6" fill="currentColor" viewBox="0 0 24 24" aria-hidden="true"><path fill-rule="evenodd" d="M22 12c0-5.523-4.477-10-10-10S2 6.477 2 12c0 4.991 3.657 9.128 8.438 9.878v-6.987h-2.54V12h2.54V9.797c0-2.506 1.492-3.89 3.777-3.89 1.094 0 2.238.195 2.238.195v2.46h-1.26c-1.243 0-1.63.771-1.63 1.562V12h2.773l-.443 2.89h-2.33v6.988C18.343 21.128 22 16.991 22 12z" clip-rule="evenodd" /></svg>
                       </a>
                       <a href="https://www.instagram.com/alibozorgi.uae" target="_blank" rel="noopener noreferrer" class="text-gray-400 hover:text-gold">
                           <span class="sr-only">Instagram</span>
                           <svg class="h-6 w-6" fill="currentColor" viewBox="0 0 24 24" aria-hidden="true"><path fill-rule="evenodd" d="M12.315 2c2.43 0 2.784.013 3.808.06 1.064.049 1.791.218 2.427.465a4.902 4.902 0 011.772 1.153 4.902 4.902 0 011.153 1.772c.247.636.416 1.363.465 2.427.048 1.024.06 1.378.06 3.808s-.012 2.784-.06 3.808c-.049 1.064-.218 1.791-.465 2.427a4.902 4.902 0 01-1.153 1.772 4.902 4.902 0 01-1.772 1.153c-.636.247-1.363.416-2.427.465-1.024.048-1.378.06-3.808.06s-2.784-.012-3.808-.06c-1.064-.049-1.791-.218-2.427-.465a4.902 4.902 0 01-1.772-1.153 4.902 4.902 0 01-1.153-1.772c-.247-.636-.416-1.363-.465-2.427-.048-1.024-.06-1.378-.06-3.808s.012-2.784.06-3.808c.049-1.064.218-1.791.465-2.427a4.902 4.902 0 011.153-1.772A4.902 4.902 0 016.345 2.525c.636-.247 1.363-.416 2.427-.465C9.794 2.013 10.148 2 12.315 2zM12 7.027a4.973 4.973 0 100 9.946 4.973 4.973 0 000-9.946zm0 8.05a3.077 3.077 0 110-6.155 3.077 3.077 0 010 6.155zM16.966 6.326a1.2 1.2 0 100 2.4 1.2 1.2 0 000-2.4z" clip-rule="evenodd" /></svg>
                       </a>
                       <a href="https://x.com/aliabozorgi" target="_blank" rel="noopener noreferrer" class="text-gray-400 hover:text-gold">
                           <span class="sr-only">Twitter</span>
                           <svg class="h-6 w-6" fill="currentColor" viewBox="0 0 24 24" aria-hidden="true"><path d="M13.682 10.682L20.236 3h-1.638L13.37 9.682 9.13 3H3l6.874 9.97L3 21h1.638l5.534-6.42L15.158 21H21l-7.318-10.318zm-2.146 2.34L11.1 12.49 5.38 4.22h2.524l4.94 5.75 0.44 0.51 5.952 7.28h-2.524l-5.28-6.07z" /></svg>
                       </a>
                   </div>
                </div>
            </div>
            <div class="mt-16 border-t border-white/10 pt-8 sm:mt-20 lg:mt-24">
                <p class="text-xs leading-5 text-gray-400">&copy; <span id="copyright-year"></span> Bozorgi Group. All rights reserved.</p>
            </div>
        </div>
    </footer>

    <!-- JavaScript -->
    <script>
        document.addEventListener('DOMContentLoaded', function() {
            // === Mobile Menu Functionality ===
            const mobileMenuButton = document.getElementById('mobile-menu-button');
            const mobileMenuCloseButton = document.getElementById('mobile-menu-close-button');
            const mobileMenu = document.getElementById('mobile-menu');
            const mobileNavItems = document.querySelectorAll('.mobile-nav-item');

            mobileMenuButton.addEventListener('click', () => {
                mobileMenu.classList.remove('hidden');
            });

            const closeMobileMenu = () => {
                mobileMenu.classList.add('hidden');
            }

            mobileMenuCloseButton.addEventListener('click', closeMobileMenu);
            mobileNavItems.forEach(item => {
                item.addEventListener('click', closeMobileMenu);
            });
            
            // === Header Shadow on Scroll ===
            const header = document.getElementById('header');
            window.addEventListener('scroll', () => {
                if (window.scrollY > 10) {
                    header.classList.add('shadow-md');
                } else {
                    header.classList.remove('shadow-md');
                }
            });

            // === Active Nav Link Highlighting on Scroll ===
            const sections = document.querySelectorAll('section[id]');
            const navLinks = document.querySelectorAll('.nav-item');

            const observerOptions = {
                root: null,
                rootMargin: '0px',
                threshold: 0.4
            };

            const observer = new IntersectionObserver((entries) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        const id = entry.target.getAttribute('id');
                        navLinks.forEach(link => {
                            link.classList.remove('text-gold');
                            if (link.getAttribute('href') === `#${id}`) {
                                link.classList.add('text-gold');
                            }
                        });
                    }
                });
            }, observerOptions);

            sections.forEach(section => {
                observer.observe(section);
            });

            // === Scroll-Reveal Animations ===
            const revealElements = document.querySelectorAll('.reveal');
            const revealObserver = new IntersectionObserver((entries) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.classList.add('reveal-visible');
                        revealObserver.unobserve(entry.target);
                    }
                });
            }, { threshold: 0.1 });

            revealElements.forEach(el => {
                revealObserver.observe(el);
            });

            // === Set Copyright Year ===
            document.getElementById('copyright-year').textContent = new Date().getFullYear();
        });
    </script>
</body>
</html>
```