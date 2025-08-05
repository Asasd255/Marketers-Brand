# Marketers-Brand
Expert digital marketer
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Asadullah - Digital Marketing Expert</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        /* Custom CSS */
        html {
            scroll-behavior: smooth;
        }
        .nav-link {
            position: relative;
        }
        .nav-link::after {
            content: '';
            position: absolute;
            width: 0;
            height: 2px;
            bottom: 0;
            left: 0;
            background-color: #3b82f6;
            transition: width 0.3s ease;
        }
        .nav-link:hover::after {
            width: 100%;
        }
        .page {
            display: none;
        }
        .page.active {
            display: block;
            animation: fadeIn 0.5s ease;
        }
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        .service-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1), 0 10px 10px -5px rgba(0, 0, 0, 0.04);
        }
        .portfolio-item:hover .portfolio-overlay {
            opacity: 1;
        }
    </style>
</head>
<body class="font-sans bg-gray-50 text-gray-800">
    <!-- Navigation -->
    <nav class="fixed w-full bg-white shadow-md z-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between h-16 items-center">
                <div class="flex-shrink-0 flex items-center">
                    <a href="#" onclick="showPage('home')" class="text-2xl font-bold text-blue-600">Asadullah Digital</a>
                </div>
                <div class="hidden md:block">
                    <div class="ml-10 flex items-baseline space-x-4">
                        <a href="#" onclick="showPage('home')" class="nav-link px-3 py-2 text-sm font-medium text-gray-900 hover:text-blue-600 transition duration-300">Home</a>
                        <a href="#" onclick="showPage('services')" class="nav-link px-3 py-2 text-sm font-medium text-gray-900 hover:text-blue-600 transition duration-300">Services</a>
                        <a href="#" onclick="showPage('portfolio')" class="nav-link px-3 py-2 text-sm font-medium text-gray-900 hover:text-blue-600 transition duration-300">Portfolio</a>
                        <a href="#" onclick="showPage('about')" class="nav-link px-3 py-2 text-sm font-medium text-gray-900 hover:text-blue-600 transition duration-300">About</a>
                        <a href="#" onclick="showPage('contact')" class="nav-link px-3 py-2 text-sm font-medium text-gray-900 hover:text-blue-600 transition duration-300">Contact</a>
                    </div>
                </div>
                <div class="md:hidden">
                    <button type="button" onclick="toggleMobileMenu()" class="inline-flex items-center justify-center p-2 rounded-md text-gray-700 hover:text-blue-600 focus:outline-none">
                        <svg class="h-6 w-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
                        </svg>
                    </button>
                </div>
            </div>
        </div>
        <!-- Mobile menu -->
        <div id="mobile-menu" class="hidden md:hidden bg-white shadow-lg">
            <div class="px-2 pt-2 pb-3 space-y-1 sm:px-3">
                <a href="#" onclick="showPage('home')" class="block px-3 py-2 rounded-md text-base font-medium text-gray-900 hover:text-blue-600">Home</a>
                <a href="#" onclick="showPage('services')" class="block px-3 py-2 rounded-md text-base font-medium text-gray-900 hover:text-blue-600">Services</a>
                <a href="#" onclick="showPage('portfolio')" class="block px-3 py-2 rounded-md text-base font-medium text-gray-900 hover:text-blue-600">Portfolio</a>
                <a href="#" onclick="showPage('about')" class="block px-3 py-2 rounded-md text-base font-medium text-gray-900 hover:text-blue-600">About</a>
                <a href="#" onclick="showPage('contact')" class="block px-3 py-2 rounded-md text-base font-medium text-gray-900 hover:text-blue-600">Contact</a>
            </div>
        </div>
    </nav>

    <!-- Home Page -->
    <section id="home" class="page active min-h-screen pt-20">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-12 md:py-24">
            <div class="md:flex items-center justify-between">
                <div class="md:w-1/2 mb-10 md:mb-0">
                    <h1 class="text-4xl md:text-6xl font-bold text-gray-900 leading-tight mb-6">
                        Digital Marketing <span class="text-blue-600">Solutions</span> That Drive Results
                    </h1>
                    <p class="text-lg text-gray-600 mb-8 max-w-lg">
                        Helping businesses grow through strategic digital marketing campaigns that deliver measurable results and ROI.
                    </p>
                    <div class="flex space-x-4">
                        <a href="#" onclick="showPage('contact')" class="bg-blue-600 hover:bg-blue-700 text-white px-6 py-3 rounded-lg font-medium transition duration-300">
                            Get Started
                        </a>
                        <a href="#" onclick="showPage('services')" class="border border-blue-600 text-blue-600 hover:bg-blue-50 px-6 py-3 rounded-lg font-medium transition duration-300">
                            Our Services
                        </a>
                    </div>
                </div>
                <div class="md:w-1/2 flex justify-center">
                    <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/eda5402f-081b-44f4-99f6-6c9751493a6f.png" alt="Digital marketing concept with abstract social media icons, graph growth charts, and web analytics dashboard on a clean white background" class="rounded-lg shadow-xl">
                </div>
            </div>
        </div>
    </section>

    <!-- Services Page -->
    <section id="services" class="page min-h-screen py-20 bg-gray-100">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="text-3xl font-bold text-gray-900 mb-4">Our Digital Marketing Services</h2>
                <p class="text-gray-600 max-w-2xl mx-auto">Comprehensive digital marketing solutions tailored to your business needs</p>
            </div>
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Service 1 -->
                <div class="service-card bg-white rounded-xl shadow-md overflow-hidden p-6 transition duration-300">
                    <div class="text-blue-600 text-4xl mb-4">
                        <i class="fas fa-search"></i>
                    </div>
                    <h3 class="text-xl font-semibold text-gray-900 mb-3">SEO Optimization</h3>
                    <p class="text-gray-600 mb-4">
                        Improve your website's visibility on search engines with our comprehensive SEO strategies that include keyword research, on-page and technical optimization.
                    </p>
                    <ul class="space-y-2 text-gray-600 mb-4">
                        <li class="flex items-start">
                            <i class="fas fa-check text-green-500 mr-2 mt-1"></i>
                            <span>Keyword research & strategy</span>
                        </li>
                        <li class="flex items-start">
                            <i class="fas fa-check text-green-500 mr-2 mt-1"></i>
                            <span>On-page optimization</span>
                        </li>
                        <li class="flex items-start">
                            <i class="fas fa-check text-green-500 mr-2 mt-1"></i>
                            <span>Technical SEO audit</span>
                        </li>
                    </ul>
                </div>

                <!-- Service 2 -->
                <div class="service-card bg-white rounded-xl shadow-md overflow-hidden p-6 transition duration-300">
                    <div class="text-blue-600 text-4xl mb-4">
                        <i class="fas fa-ad"></i>
                    </div>
                    <h3 class="text-xl font-semibold text-gray-900 mb-3">Paid Advertising</h3>
                    <p class="text-gray-600 mb-4">
                        Maximize your ROI with targeted Facebook, Instagram, and Google Ads campaigns that reach your ideal customers at the right moment.
                    </p>
                    <ul class="space-y-2 text-gray-600 mb-4">
                        <li class="flex items-start">
                            <i class="fas fa-check text-green-500 mr-2 mt-1"></i>
                            <span>Facebook & Instagram Ads</span>
                        </li>
                        <li class="flex items-start">
                            <i class="fas fa-check text-green-500 mr-2 mt-1"></i>
                            <span>Google Ads (Search & Display)</span>
                        </li>
                        <li class="flex items-start">
                            <i class="fas fa-check text-green-500 mr-2 mt-1"></i>
                            <span>Conversion tracking & optimization</span>
                        </li>
                    </ul>
                </div>

                <!-- Service 3 -->
                <div class="service-card bg-white rounded-xl shadow-md overflow-hidden p-6 transition duration-300">
                    <div class="text-blue-600 text-4xl mb-4">
                        <i class="fas fa-users"></i>
                    </div>
                    <h3 class="text-xl font-semibold text-gray-900 mb-3">Social Media Marketing</h3>
                    <p class="text-gray-600 mb-4">
                        Build brand awareness and engage with your audience through strategic social media content and community management.
                    </p>
                    <ul class="space-y-2 text-gray-600 mb-4">
                        <li class="flex items-start">
                            <i class="fas fa-check text-green-500 mr-2 mt-1"></i>
                            <span>Content strategy & calendar</span>
                        </li>
                        <li class="flex items-start">
                            <i class="fas fa-check text-green-500 mr-2 mt-1"></i>
                            <span>Community management</span>
                        </li>
                        <li class="flex items-start">
                            <i class="fas fa-check text-green-500 mr-2 mt-1"></i>
                            <span>Influencer collaborations</span>
                        </li>
                    </ul>
                </div>

                <!-- Service 4 -->
                <div class="service-card bg-white rounded-xl shadow-md overflow-hidden p-6 transition duration-300">
                    <div class="text-blue-600 text-4xl mb-4">
                        <i class="fas fa-envelope-open-text"></i>
                    </div>
                    <h3 class="text-xl font-semibold text-gray-900 mb-3">Email Marketing</h3>
                    <p class="text-gray-600 mb-4">
                        Nurture leads and build customer loyalty through personalized email campaigns that drive engagement and conversions.
                    </p>
                    <ul class="space-y-2 text-gray-600 mb-4">
                        <li class="flex items-start">
                            <i class="fas fa-check text-green-500 mr-2 mt-1"></i>
                            <span>Email campaign design</span>
                        </li>
                        <li class="flex items-start">
                            <i class="fas fa-check text-green-500 mr-2 mt-1"></i>
                            <span>Automation workflows</span>
                        </li>
                        <li class="flex items-start">
                            <i class="fas fa-check text-green-500 mr-2 mt-1"></i>
                            <span>List segmentation & personalization</span>
                        </li>
                    </ul>
                </div>

                <!-- Service 5 -->
                <div class="service-card bg-white rounded-xl shadow-md overflow-hidden p-6 transition duration-300">
                    <div class="text-blue-600 text-4xl mb-4">
                        <i class="fas fa-chart-line"></i>
                    </div>
                    <h3 class="text-xl font-semibold text-gray-900 mb-3">Content Marketing</h3>
                    <p class="text-gray-600 mb-4">
                        Attract and retain customers through valuable, relevant content that establishes your brand as an industry authority.
                    </p>
                    <ul class="space-y-2 text-gray-600 mb-4">
                        <li class="flex items-start">
                            <i class="fas fa-check text-green-500 mr-2 mt-1"></i>
                            <span>Blog content creation</span>
                        </li>
                        <li class="flex items-start">
                            <i class="fas fa-check text-green-500 mr-2 mt-1"></i>
                            <span>Video production</span>
                        </li>
                        <li class="flex items-start">
                            <i class="fas fa-check text-green-500 mr-2 mt-1"></i>
                            <span>Content distribution strategy</span>
                        </li>
                    </ul>
                </div>

                <!-- Service 6 -->
                <div class="service-card bg-white rounded-xl shadow-md overflow-hidden p-6 transition duration-300">
                    <div class="text-blue-600 text-4xl mb-4">
                        <i class="fas fa-mobile-alt"></i>
                    </div>
                    <h3 class="text-xl font-semibold text-gray-900 mb-3">Web Development</h3>
                    <p class="text-gray-600 mb-4">
                        Get a high-performance website that converts visitors into customers with our custom web development solutions.
                    </p>
                    <ul class="space-y-2 text-gray-600 mb-4">
                        <li class="flex items-start">
                            <i class="fas fa-check text-green-500 mr-2 mt-1"></i>
                            <span>Responsive website design</span>
                        </li>
                        <li class="flex items-start">
                            <i class="fas fa-check text-green-500 mr-2 mt-1"></i>
                            <span>Landing page creation</span>
                        </li>
                        <li class="flex items-start">
                            <i class="fas fa-check text-green-500 mr-2 mt-1"></i>
                            <span>Conversion rate optimization</span>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- Portfolio Page -->
    <section id="portfolio" class="page min-h-screen py-20 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="text-3xl font-bold text-gray-900 mb-4">Our Portfolio</h2>
                <p class="text-gray-600 max-w-2xl mx-auto">See examples of our successful digital marketing campaigns</p>
            </div>
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-6">
                <!-- Portfolio Item 1 -->
                <div class="portfolio-item relative rounded-xl overflow-hidden shadow-lg">
                    <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/31231c70-46a5-4b35-9239-485a8798ab2a.png" alt="E-commerce website dashboard showing increased sales after digital marketing campaign implementation" class="w-full h-64 object-cover">
                    <div class="portfolio-overlay absolute inset-0 bg-blue-600 bg-opacity-90 flex items-center justify-center flex-col text-white opacity-0 transition-opacity duration-300 p-6">
                        <h3 class="text-xl font-bold mb-2">E-Commerce Growth</h3>
                        <p class="text-center mb-4">Increased online sales by 320% within 6 months for a fashion retail client through comprehensive digital marketing strategy.</p>
                        <span class="px-4 py-2 bg-white text-blue-600 rounded-full text-sm font-medium">View Case Study</span>
                    </div>
                </div>

                <!-- Portfolio Item 2 -->
                <div class="portfolio-item relative rounded-xl overflow-hidden shadow-lg">
                    <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/dd57d3fd-fc61-4339-a0b9-f7479549f439.png" alt="Social media analytics showing increased engagement and follower growth after campaign implementation" class="w-full h-64 object-cover">
                    <div class="portfolio-overlay absolute inset-0 bg-blue-600 bg-opacity-90 flex items-center justify-center flex-col text-white opacity-0 transition-opacity duration-300 p-6">
                        <h3 class="text-xl font-bold mb-2">Social Media Engagement</h3>
                        <p class="text-center mb-4">Grew a restaurant's Instagram following from 500 to 15k+ followers with engaging content strategy.</p>
                        <span class="px-4 py-2 bg-white text-blue-600 rounded-full text-sm font-medium">View Case Study</span>
                    </div>
                </div>

                <!-- Portfolio Item 3 -->
                <div class="portfolio-item relative rounded-xl overflow-hidden shadow-lg">
                    <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/d6e00cf0-f7df-4124-8c83-3cfec1c816c6.png" alt="Google Analytics dashboard showing organic traffic growth after SEO optimization campaign" class="w-full h-64 object-cover">
                    <div class="portfolio-overlay absolute inset-0 bg-blue-600 bg-opacity-90 flex items-center justify-center flex-col text-white opacity-0 transition-opacity duration-300 p-6">
                        <h3 class="text-xl font-bold mb-2">SEO Success</h3>
                        <p class="text-center mb-4">Improved organic traffic by 450% for a B2B software company through comprehensive SEO strategy.</p>
                        <span class="px-4 py-2 bg-white text-blue-600 rounded-full text-sm font-medium">View Case Study</span>
                    </div>
                </div>

                <!-- Portfolio Item 4 -->
                <div class="portfolio-item relative rounded-xl overflow-hidden shadow-lg">
                    <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/edbf4713-04da-4d02-9663-cbb6e2cc2632.png" alt="Email marketing dashboard showing high open and click-through rates for a campaign" class="w-full h-64 object-cover">
                    <div class="portfolio-overlay absolute inset-0 bg-blue-600 bg-opacity-90 flex items-center justify-center flex-col text-white opacity-0 transition-opacity duration-300 p-6">
                        <h3 class="text-xl font-bold mb-2">Email Marketing</h3>
                        <p class="text-center mb-4">Achieved 45% open rates for a financial services company through personalized email marketing automation.</p>
                        <span class="px-4 py-2 bg-white text-blue-600 rounded-full text-sm font-medium">View Case Study</span>
                    </div>
                </div>

                <!-- Portfolio Item 5 -->
                <div class="portfolio-item relative rounded-xl overflow-hidden shadow-lg">
                    <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/96eb0ddc-7d5e-427b-88da-eccaf0ccf449.png" alt="Google Ads dashboard showing effective PPC campaign with high conversion rates and low cost per acquisition" class="w-full h-64 object-cover">
                    <div class="portfolio-overlay absolute inset-0 bg-blue-600 bg-opacity-90 flex items-center justify-center flex-col text-white opacity-0 transition-opacity duration-300 p-6">
                        <h3 class="text-xl font-bold mb-2">PPC Campaign</h3>
                        <p class="text-center mb-4">Decreased cost per acquisition by 65% for a home services business through Google Ads optimization.</p>
                        <span class="px-4 py-2 bg-white text-blue-600 rounded-full text-sm font-medium">View Case Study</span>
                    </div>
                </div>

                <!-- Portfolio Item 6 -->
                <div class="portfolio-item relative rounded-xl overflow-hidden shadow-lg">
                    <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/ec4d8fe8-1c31-4832-b2ca-f86964be05de.png" alt="Website design showcase for a luxury real estate client with modern aesthetics and high conversion elements" class="w-full h-64 object-cover">
                    <div class="portfolio-overlay absolute inset-0 bg-blue-600 bg-opacity-90 flex items-center justify-center flex-col text-white opacity-0 transition-opacity duration-300 p-6">
                        <h3 class="text-xl font-bold mb-2">Web Design</h3>
                        <p class="text-center mb-4">Created a high-converting website for a luxury real estate client that increased lead generation by 200%.</p>
                        <span class="px-4 py-2 bg-white text-blue-600 rounded-full text-sm font-medium">View Case Study</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- About Page -->
    <section id="about" class="page min-h-screen py-20 bg-gray-100">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="md:flex items-center">
                <div class="md:w-1/2 mb-10 md:mb-0">
                    <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/6d18fd39-4e00-4f06-8ff9-d2fcdd9a00a7.png" alt="Professional portrait of Asadullah, a digital marketing expert from Pakistan, wearing business casual attire and smiling confidently" class="rounded-lg shadow-xl">
                </div>
                <div class="md:w-1/2 md:pl-12">
                    <h2 class="text-3xl font-bold text-gray-900 mb-6">About Me</h2>
                    <p class="text-gray-600 mb-4">
                        Hi, I'm Asadullah, a passionate digital marketing expert with 5+ years of experience helping businesses grow their online presence and reach their target audiences effectively.
                    </p>
                    <p class="text-gray-600 mb-4">
                        My journey in digital marketing began when I recognized the power of online platforms to transform businesses. Since then, I've dedicated myself to mastering the latest digital marketing strategies, tools, and trends to deliver measurable results for my clients.
                    </p>
                    <p class="text-gray-600 mb-6">
                        I believe in data-driven marketing approaches combined with creative strategies that resonate with your audience. Every campaign I create is tailored to your specific business needs and goals.
                    </p>
                    <div class="mb-8">
                        <h4 class="text-lg font-semibold text-gray-900 mb-3">My Approach</h4>
                        <ul class="space-y-3">
                            <li class="flex items-start">
                                <div class="flex-shrink-0 h-5 w-5 text-blue-600 mt-1 mr-2">
                                    <i class="fas fa-check-circle"></i>
                                </div>
                                <p class="text-gray-600"><strong>Strategic:</strong> Every campaign starts with in-depth research and planning</p>
                            </li>
                            <li class="flex items-start">
                                <div class="flex-shrink-0 h-5 w-5 text-blue-600 mt-1 mr-2">
                                    <i class="fas fa-check-circle"></i>
                                </div>
                                <p class="text-gray-600"><strong>Transparent:</strong> Clear reporting and communication at every stage</p>
                            </li>
                            <li class="flex items-start">
                                <div class="flex-shrink-0 h-5 w-5 text-blue-600 mt-1 mr-2">
                                    <i class="fas fa-check-circle"></i>
                                </div>
                                <p class="text-gray-600"><strong>Results-Driven:</strong> Focused on delivering measurable ROI</p>
                            </li>
                        </ul>
                    </div>
                    <a href="#" onclick="showPage('contact')" class="inline-flex items-center px-6 py-3 border border-transparent text-base font-medium rounded-md shadow-sm text-white bg-blue-600 hover:bg-blue-700 transition duration-300">
                        Get in Touch
                    </a>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Page -->
    <section id="contact" class="page min-h-screen py-20 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="text-3xl font-bold text-gray-900 mb-4">Get In Touch</h2>
                <p class="text-gray-600 max-w-2xl mx-auto">Ready to grow your business? Contact me today to discuss your digital marketing needs.</p>
            </div>
            <div class="md:flex">
                <div class="md:w-1/2 mb-10 md:mb-0 md:pr-8">
                    <div class="bg-gray-50 p-8 rounded-xl shadow-sm">
                        <h3 class="text-xl font-semibold text-gray-900 mb-6">Contact Information</h3>
                        <div class="space-y-4">
                            <div class="flex items-start">
                                <div class="flex-shrink-0 h-6 w-6 text-blue-600 mt-1">
                                    <i class="fas fa-map-marker-alt"></i>
                                </div>
                                <div class="ml-3">
                                    <p class="text-base font-medium text-gray-900">Address</p>
                                    <p class="text-gray-600">Basti Zahoorabad, Khanewal, Pakistan</p>
                                </div>
                            </div>
                            <div class="flex items-start">
                                <div class="flex-shrink-0 h-6 w-6 text-blue-600 mt-1">
                                    <i class="fas fa-phone-alt"></i>
                                </div>
                                <div class="ml-3">
                                    <p class="text-base font-medium text-gray-900">Phone</p>
                                    <p class="text-gray-600">+92 304 1020106</p>
                                </div>
                            </div>
                            <div class="flex items-start">
                                <div class="flex-shrink-0 h-6 w-6 text-blue-600 mt-1">
                                    <i class="fas fa-envelope"></i>
                                </div>
                                <div class="ml-3">
                                    <p class="text-base font-medium text-gray-900">Email</p>
                                    <p class="text-gray-600">marketerdigital554@gmail.com</p>
                                </div>
                            </div>
                        </div>
                        <div class="mt-8">
                            <h4 class="text-lg font-semibold text-gray-900 mb-4">Connect With Me</h4>
                            <div class="flex space-x-4">
                                <a href="#" class="h-10 w-10 rounded-full bg-blue-600 text-white flex items-center justify-center hover:bg-blue-700 transition duration-300">
                                    <i class="fab fa-facebook-f"></i>
                                </a>
                                <a href="#" class="h-10 w-10 rounded-full bg-blue-400 text-white flex items-center justify-center hover:bg-blue-500 transition duration-300">
                                    <i class="fab fa-twitter"></i>
                                </a>
                                <a href="#" class="h-10 w-10 rounded-full bg-pink-600 text-white flex items-center justify-center hover:bg-pink-700 transition duration-300">
                                    <i class="fab fa-instagram"></i>
                                </a>
                                <a href="#" class="h-10 w-10
