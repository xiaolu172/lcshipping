<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SwiftShip - Reliable Shipping Solutions</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        .gradient-bg {
            background: linear-gradient(135deg, #3b82f6 0%, #1d4ed8 100%);
        }
        .card-hover:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1);
        }
        .tracking-input:focus {
            outline: none;
            box-shadow: 0 0 0 3px rgba(59, 130, 246, 0.5);
        }
        .service-card:hover .service-icon {
            transform: scale(1.1);
        }
        #mobile-menu {
            transition: all 0.3s ease;
        }
    </style>
</head>
<body class="font-sans antialiased text-gray-800">
    <!-- Navigation -->
    <nav class="bg-white shadow-lg sticky top-0 z-50">
        <div class="max-w-7xl mx-auto px-4">
            <div class="flex justify-between">
                <div class="flex space-x-7">
                    <div>
                        <a href="#" class="flex items-center py-4 px-2">
                            <span class="font-bold text-blue-600 text-2xl">Swift<span class="text-blue-800">Ship</span></span>
                        </a>
                    </div>
                    <div class="hidden md:flex items-center space-x-1">
                        <a href="#" class="py-4 px-2 text-blue-600 border-b-4 border-blue-600 font-semibold">Home</a>
                        <a href="#services" class="py-4 px-2 text-gray-500 font-semibold hover:text-blue-600 transition duration-300">Services</a>
                        <a href="#tracking" class="py-4 px-2 text-gray-500 font-semibold hover:text-blue-600 transition duration-300">Tracking</a>
                        <a href="#pricing" class="py-4 px-2 text-gray-500 font-semibold hover:text-blue-600 transition duration-300">Pricing</a>
                        <a href="#contact" class="py-4 px-2 text-gray-500 font-semibold hover:text-blue-600 transition duration-300">Contact</a>
                    </div>
                </div>
                <div class="hidden md:flex items-center space-x-3">
                    <a href="#" class="py-2 px-4 font-medium text-gray-600 rounded hover:bg-blue-100 transition duration-300">
                        <i class="fas fa-user mr-1"></i> Login
                    </a>
                    <a href="#" class="py-2 px-4 font-medium text-white bg-blue-600 rounded hover:bg-blue-700 transition duration-300">
                        <i class="fas fa-box mr-1"></i> Ship Now
                    </a>
                </div>
                <div class="md:hidden flex items-center">
                    <button id="menu-btn" class="outline-none mobile-menu-button">
                        <svg class="w-6 h-6 text-gray-500 hover:text-blue-600"
                            fill="none"
                            stroke-linecap="round"
                            stroke-linejoin="round"
                            stroke-width="2"
                            viewBox="0 0 24 24"
                            stroke="currentColor">
                            <path d="M4 6h16M4 12h16M4 18h16"></path>
                        </svg>
                    </button>
                </div>
            </div>
        </div>
        <div id="mobile-menu" class="hidden md:hidden bg-white">
            <a href="#" class="block py-2 px-4 text-sm hover:bg-gray-100 text-blue-600 font-semibold">Home</a>
            <a href="#services" class="block py-2 px-4 text-sm hover:bg-gray-100">Services</a>
            <a href="#tracking" class="block py-2 px-4 text-sm hover:bg-gray-100">Tracking</a>
            <a href="#pricing" class="block py-2 px-4 text-sm hover:bg-gray-100">Pricing</a>
            <a href="#contact" class="block py-2 px-4 text-sm hover:bg-gray-100">Contact</a>
            <div class="py-2 px-4">
                <a href="#" class="block text-center py-2 px-4 font-medium text-gray-600 rounded hover:bg-blue-100 mb-2">
                    <i class="fas fa-user mr-1"></i> Login
                </a>
                <a href="#" class="block text-center py-2 px-4 font-medium text-white bg-blue-600 rounded hover:bg-blue-700">
                    <i class="fas fa-box mr-1"></i> Ship Now
                </a>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="gradient-bg text-white">
        <div class="container mx-auto px-6 py-20">
            <div class="flex flex-col md:flex-row items-center">
                <div class="md:w-1/2 flex flex-col items-start mb-10 md:mb-0">
                    <h1 class="text-4xl md:text-5xl font-bold leading-tight mb-4">Fast, Reliable Shipping Solutions</h1>
                    <p class="text-xl mb-8">Delivering your packages with care and precision, anywhere in the world.</p>
                    
                    <!-- Tracking Form -->
                    <div class="w-full max-w-md bg-white rounded-lg shadow-lg p-6 mb-8">
                        <h3 class="text-xl font-bold text-gray-800 mb-4">Track Your Shipment</h3>
                        <div class="flex">
                            <input type="text" placeholder="Enter tracking number" class="flex-grow px-4 py-3 rounded-l-lg border border-gray-300 tracking-input text-gray-800 focus:border-blue-500">
                            <button class="bg-blue-600 hover:bg-blue-700 text-white font-bold py-3 px-6 rounded-r-lg transition duration-300">
                                Track
                            </button>
                        </div>
                        <p class="text-sm text-gray-600 mt-2">Don't have a tracking number? <a href="#" class="text-blue-600 hover:underline">Contact us</a></p>
                    </div>
                    
                    <div class="flex flex-col sm:flex-row gap-4">
                        <button class="bg-white text-blue-600 hover:bg-gray-100 font-bold py-3 px-6 rounded-full text-lg transition duration-300 transform hover:scale-105">
                            <i class="fas fa-box mr-2"></i> Ship Now
                        </button>
                        <button class="border-2 border-white text-white hover:bg-white hover:text-blue-600 font-bold py-3 px-6 rounded-full text-lg transition duration-300 transform hover:scale-105">
                            <i class="fas fa-phone-alt mr-2"></i> Call Us
                        </button>
                    </div>
                </div>
                <div class="md:w-1/2">
                    <img src="https://images.unsplash.com/photo-1556740738-b6a63e27c4df?ixlib=rb-1.2.1&auto=format&fit=crop&w=750&q=80" alt="Delivery truck" class="rounded-lg shadow-2xl">
                </div>
            </div>
        </div>
    </section>

    <!-- Stats Section -->
    <section class="bg-gray-50 py-12">
        <div class="container mx-auto px-6">
            <div class="grid grid-cols-2 md:grid-cols-4 gap-8 text-center">
                <div class="bg-white p-6 rounded-lg shadow-sm">
                    <div class="text-blue-600 text-4xl font-bold mb-2">10M+</div>
                    <div class="text-gray-600">Packages Delivered</div>
                </div>
                <div class="bg-white p-6 rounded-lg shadow-sm">
                    <div class="text-blue-600 text-4xl font-bold mb-2">150+</div>
                    <div class="text-gray-600">Countries Served</div>
                </div>
                <div class="bg-white p-6 rounded-lg shadow-sm">
                    <div class="text-blue-600 text-4xl font-bold mb-2">99%</div>
                    <div class="text-gray-600">On-Time Delivery</div>
                </div>
                <div class="bg-white p-6 rounded-lg shadow-sm">
                    <div class="text-blue-600 text-4xl font-bold mb-2">24/7</div>
                    <div class="text-gray-600">Customer Support</div>
                </div>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section id="services" class="py-20 bg-white">
        <div class="container mx-auto px-6">
            <h2 class="text-3xl font-bold text-center text-gray-800 mb-4">Our Shipping Services</h2>
            <p class="text-xl text-center text-gray-600 mb-16 max-w-3xl mx-auto">We offer a comprehensive range of shipping solutions tailored to meet your specific needs.</p>
            
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Service 1 -->
                <div class="bg-gray-50 p-8 rounded-lg shadow-sm service-card transition duration-300">
                    <div class="text-blue-600 mb-4">
                        <i class="fas fa-shipping-fast service-icon text-5xl transition duration-300"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3">Express Shipping</h3>
                    <p class="text-gray-600 mb-4">Get your packages delivered in 1-3 business days with our premium express service.</p>
                    <a href="#" class="text-blue-600 font-semibold hover:underline">Learn more <i class="fas fa-arrow-right ml-1"></i></a>
                </div>
                
                <!-- Service 2 -->
                <div class="bg-gray-50 p-8 rounded-lg shadow-sm service-card transition duration-300">
                    <div class="text-blue-600 mb-4">
                        <i class="fas fa-globe-americas service-icon text-5xl transition duration-300"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3">International Shipping</h3>
                    <p class="text-gray-600 mb-4">Reliable global delivery with customs clearance handled by our experts.</p>
                    <a href="#" class="text-blue-600 font-semibold hover:underline">Learn more <i class="fas fa-arrow-right ml-1"></i></a>
                </div>
                
                <!-- Service 3 -->
                <div class="bg-gray-50 p-8 rounded-lg shadow-sm service-card transition duration-300">
                    <div class="text-blue-600 mb-4">
                        <i class="fas fa-pallet service-icon text-5xl transition duration-300"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3">Freight Services</h3>
                    <p class="text-gray-600 mb-4">Cost-effective solutions for large shipments and palletized goods.</p>
                    <a href="#" class="text-blue-600 font-semibold hover:underline">Learn more <i class="fas fa-arrow-right ml-1"></i></a>
                </div>
                
                <!-- Service 4 -->
                <div class="bg-gray-50 p-8 rounded-lg shadow-sm service-card transition duration-300">
                    <div class="text-blue-600 mb-4">
                        <i class="fas fa-warehouse service-icon text-5xl transition duration-300"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3">Warehousing</h3>
                    <p class="text-gray-600 mb-4">Secure storage solutions with inventory management and fulfillment services.</p>
                    <a href="#" class="text-blue-600 font-semibold hover:underline">Learn more <i class="fas fa-arrow-right ml-1"></i></a>
                </div>
                
                <!-- Service 5 -->
                <div class="bg-gray-50 p-8 rounded-lg shadow-sm service-card transition duration-300">
                    <div class="text-blue-600 mb-4">
                        <i class="fas fa-temperature-low service-icon text-5xl transition duration-300"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3">Cold Chain Logistics</h3>
                    <p class="text-gray-600 mb-4">Temperature-controlled shipping for pharmaceuticals, food, and other sensitive goods.</p>
                    <a href="#" class="text-blue-600 font-semibold hover:underline">Learn more <i class="fas fa-arrow-right ml-1"></i></a>
                </div>
                
                <!-- Service 6 -->
                <div class="bg-gray-50 p-8 rounded-lg shadow-sm service-card transition duration-300">
                    <div class="text-blue-600 mb-4">
                        <i class="fas fa-undo service-icon text-5xl transition duration-300"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3">Returns Management</h3>
                    <p class="text-gray-600 mb-4">Streamlined returns process to enhance your customer experience.</p>
                    <a href="#" class="text-blue-600 font-semibold hover:underline">Learn more <i class="fas fa-arrow-right ml-1"></i></a>
                </div>
            </div>
        </div>
    </section>

    <!-- Tracking Section -->
    <section id="tracking" class="py-20 bg-gray-50">
        <div class="container mx-auto px-6">
            <div class="flex flex-col lg:flex-row items-center">
                <div class="lg:w-1/2 mb-12 lg:mb-0 lg:pr-12">
                    <h2 class="text-3xl font-bold text-gray-800 mb-6">Real-Time Package Tracking</h2>
                    <p class="text-gray-600 mb-8">Track your shipments in real-time with our advanced tracking system. Get instant updates on your package's location and estimated delivery time.</p>
                    
                    <div class="space-y-6">
                        <div class="flex items-start">
                            <div class="bg-blue-100 p-3 rounded-full mr-4 mt-1">
                                <i class="fas fa-map-marker-alt text-blue-600"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-gray-800 mb-2">Live Location Tracking</h4>
                                <p class="text-gray-600">See exactly where your package is at any moment during transit.</p>
                            </div>
                        </div>
                        
                        <div class="flex items-start">
                            <div class="bg-blue-100 p-3 rounded-full mr-4 mt-1">
                                <i class="fas fa-bell text-blue-600"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-gray-800 mb-2">Instant Notifications</h4>
                                <p class="text-gray-600">Get alerts via email or SMS for all important delivery milestones.</p>
                            </div>
                        </div>
                        
                        <div class="flex items-start">
                            <div class="bg-blue-100 p-3 rounded-full mr-4 mt-1">
                                <i class="fas fa-history text-blue-600"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-gray-800 mb-2">Delivery History</h4>
                                <p class="text-gray-600">Access complete delivery history for all your shipments.</p>
                            </div>
                        </div>
                    </div>
                    
                    <a href="tracking.html" class="inline-block mt-8 bg-blue-600 hover:bg-blue-700 text-white font-bold py-3 px-6 rounded-lg transition duration-300">
                        <i class="fas fa-search mr-2"></i> Track Your Package
                    </a>
                </div>
                
                <div class="lg:w-1/2">
                    <div class="bg-white p-6 rounded-lg shadow-lg">
                        <div class="border-l-4 border-blue-600 pl-4 mb-6">
                            <h3 class="text-xl font-bold text-gray-800">Sample Tracking Information</h3>
                            <p class="text-gray-600">Tracking #: SW123456789</p>
                        </div>
                        
                        <div class="space-y-6">
                            <!-- Tracking Step 1 -->
                            <div class="flex">
                                <div class="flex flex-col items-center mr-4">
                                    <div class="w-8 h-8 bg-blue-600 rounded-full flex items-center justify-center text-white">
                                        <i class="fas fa-check"></i>
                                    </div>
                                    <div class="w-px h-full bg-blue-300"></div>
                                </div>
                                <div class="pb-6">
                                    <p class="font-semibold text-gray-800">Package Delivered</p>
                                    <p class="text-sm text-gray-600">June 15, 2023 - 10:30 AM</p>
                                    <p class="text-gray-600 mt-1">Delivered to front door. Signed by John Smith.</p>
                                </div>
                            </div>
                            
                            <!-- Tracking Step 2 -->
                            <div class="flex">
                                <div class="flex flex-col items-center mr-4">
                                    <div class="w-8 h-8 bg-blue-600 rounded-full flex items-center justify-center text-white">
                                        <i class="fas fa-check"></i>
                                    </div>
                                    <div class="w-px h-full bg-blue-300"></div>
                                </div>
                                <div class="pb-6">
                                    <p class="font-semibold text-gray-800">Out for Delivery</p>
                                    <p class="text-sm text-gray-600">June 15, 2023 - 8:15 AM</p>
                                    <p class="text-gray-600 mt-1">Your package is on the delivery vehicle.</p>
                                </div>
                            </div>
                            
                            <!-- Tracking Step 3 -->
                            <div class="flex">
                                <div class="flex flex-col items-center mr-4">
                                    <div class="w-8 h-8 bg-blue-600 rounded-full flex items-center justify-center text-white">
                                        <i class="fas fa-check"></i>
                                    </div>
                                    <div class="w-px h-full bg-blue-300"></div>
                                </div>
                                <div class="pb-6">
                                    <p class="font-semibold text-gray-800">Arrived at Local Facility</p>
                                    <p class="text-sm text-gray-600">June 14, 2023 - 11:45 PM</p>
                                    <p class="text-gray-600 mt-1">Package processed at New York distribution center.</p>
                                </div>
                            </div>
                            
                            <!-- Tracking Step 4 -->
                            <div class="flex">
                                <div class="flex flex-col items-center mr-4">
                                    <div class="w-8 h-8 bg-blue-600 rounded-full flex items-center justify-center text-white">
                                        <i class="fas fa-check"></i>
                                    </div>
                                </div>
                                <div>
                                    <p class="font-semibold text-gray-800">Shipped</p>
                                    <p class="text-sm text-gray-600">June 12, 2023 - 3:20 PM</p>
                                    <p class="text-gray-600 mt-1">Package left origin facility in Los Angeles.</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Pricing Section -->
    <section id="pricing" class="py-20 bg-white">
        <div class="container mx-auto px-6">
            <h2 class="text-3xl font-bold text-center text-gray-800 mb-4">Simple, Transparent Pricing</h2>
            <p class="text-xl text-center text-gray-600 mb-16">Pay only for what you need with our flexible pricing options.</p>
            
            <div class="flex flex-col md:flex-row justify-center items-center md:items-stretch gap-8">
                <!-- Domestic Shipping -->
                <div class="w-full md:w-1/3 bg-gray-50 border border-gray-200 rounded-lg py-8 px-6 text-center hover:shadow-lg transition duration-300">
                    <h3 class="text-2xl font-bold mb-4">Domestic Shipping</h3>
                    <div class="text-4xl font-bold mb-6">$7.99<span class="text-lg text-gray-600">/package</span></div>
                    <ul class="mb-8 text-gray-600 space-y-3">
                        <li class="flex items-center justify-center">
                            <i class="fas fa-check text-green-500 mr-2"></i> 2-5 business days
                        </li>
                        <li class="flex items-center justify-center">
                            <i class="fas fa-check text-green-500 mr-2"></i> Up to 5 lbs
                        </li>
                        <li class="flex items-center justify-center">
                            <i class="fas fa-check text-green-500 mr-2"></i> Tracking included
                        </li>
                        <li class="flex items-center justify-center">
                            <i class="fas fa-check text-green-500 mr-2"></i> $100 insurance
                        </li>
                    </ul>
                    <button class="w-full bg-blue-600 hover:bg-blue-700 text-white font-bold py-3 px-4 rounded-lg transition duration-300">
                        Choose Plan
                    </button>
                </div>
                
                <!-- International Shipping -->
                <div class="w-full md:w-1/3 border-2 border-blue-600 rounded-lg py-8 px-6 text-center transform hover:shadow-lg transition duration-300 relative">
                    <div class="absolute top-0 right-0 bg-blue-600 text-white text-xs font-bold px-3 py-1 rounded-bl rounded-tr">POPULAR</div>
                    <h3 class="text-2xl font-bold mb-4">International Shipping</h3>
                    <div class="text-4xl font-bold mb-6">$24.99<span class="text-lg text-gray-600">/package</span></div>
                    <ul class="mb-8 text-gray-600 space-y-3">
                        <li class="flex items-center justify-center">
                            <i class="fas fa-check text-green-500 mr-2"></i> 5-10 business days
                        </li>
                        <li class="flex items-center justify-center">
                            <i class="fas fa-check text-green-500 mr-2"></i> Up to 10 lbs
                        </li>
                        <li class="flex items-center justify-center">
                            <i class="fas fa-check text-green-500 mr-2"></i> Customs clearance
                        </li>
                        <li class="flex items-center justify-center">
                            <i class="fas fa-check text-green-500 mr-2"></i> $500 insurance
                        </li>
                    </ul>
                    <button class="w-full bg-blue-600 hover:bg-blue-700 text-white font-bold py-3 px-4 rounded-lg transition duration-300">
                        Choose Plan
                    </button>
                </div>
                
                <!-- Enterprise Solutions -->
                <div class="w-full md:w-1/3 bg-gray-50 border border-gray-200 rounded-lg py-8 px-6 text-center hover:shadow-lg transition duration-300">
                    <h3 class="text-2xl font-bold mb-4">Enterprise Solutions</h3>
                    <div class="text-4xl font-bold mb-6">Custom</div>
                    <ul class="mb-8 text-gray-600 space-y-3">
                        <li class="flex items-center justify-center">
                            <i class="fas fa-check text-green-500 mr-2"></i> Volume discounts
                        </li>
                        <li class="flex items-center justify-center">
                            <i class="fas fa-check text-green-500 mr-2"></i> Dedicated account manager
                        </li>
                        <li class="flex items-center justify-center">
                            <i class="fas fa-check text-green-500 mr-2"></i> API integration
                        </li>
                        <li class="flex items-center justify-center">
                            <i class="fas fa-check text-green-500 mr-2"></i> Custom solutions
                        </li>
                    </ul>
                    <button class="w-full bg-blue-600 hover:bg-blue-700 text-white font-bold py-3 px-4 rounded-lg transition duration-300">
                        Contact Sales
                    </button>
                </div>
            </div>
            
            <div class="mt-16 bg-blue-50 border border-blue-200 rounded-lg p-6">
                <h3 class="text-xl font-bold text-gray-800 mb-4">Need help choosing?</h3>
                <p class="text-gray-600 mb-4">Our shipping experts can help you select the right service for your needs.</p>
                <div class="flex flex-col sm:flex-row gap-4">
                    <button class="bg-blue-600 hover:bg-blue-700 text-white font-bold py-3 px-6 rounded-lg transition duration-300">
                        <i class="fas fa-phone-alt mr-2"></i> Call Us: (800) 123-4567
                    </button>
                    <button class="bg-white hover:bg-gray-100 text-blue-600 font-bold py-3 px-6 rounded-lg border border-blue-600 transition duration-300">
                        <i class="fas fa-comment-alt mr-2"></i> Live Chat
                    </button>
                </div>
            </div>
        </div>
    </section>

    <!-- Testimonials Section -->
    <section class="py-20 bg-gray-50">
        <div class="container mx-auto px-6">
            <h2 class="text-3xl font-bold text-center text-gray-800 mb-4">Trusted by Businesses Worldwide</h2>
            <p class="text-xl text-center text-gray-600 mb-16">See what our customers say about our shipping services.</p>
            
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <!-- Testimonial 1 -->
                <div class="bg-white p-8 rounded-lg shadow-sm">
                    <div class="flex items-center mb-4">
                        <div class="text-yellow-400 mr-2">
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                        </div>
                    </div>
                    <p class="text-gray-600 italic mb-6">"SwiftShip has transformed our e-commerce operations. Their reliable service and real-time tracking give us peace of mind when shipping to customers worldwide."</p>
                    <div class="flex items-center">
                        <img class="w-12 h-12 rounded-full mr-4" src="https://randomuser.me/api/portraits/women/32.jpg" alt="Sarah Johnson">
                        <div>
                            <h4 class="font-bold">Sarah Johnson</h4>
                            <p class="text-gray-600 text-sm">CEO, TrendyBoutique</p>
                        </div>
                    </div>
                </div>
                
                <!-- Testimonial 2 -->
                <div class="bg-white p-8 rounded-lg shadow-sm">
                    <div class="flex items-center mb-4">
                        <div class="text-yellow-400 mr-2">
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                        </div>
                    </div>
                    <p class="text-gray-600 italic mb-6">"The customer support is exceptional. When we had a time-sensitive shipment, their team went above and beyond to ensure it arrived on time."</p>
                    <div class="flex items-center">
                        <img class="w-12 h-12 rounded-full mr-4" src="https://randomuser.me/api/portraits/men/54.jpg" alt="Michael Chen">
                        <div>
                            <h4 class="font-bold">Michael Chen</h4>
                            <p class="text-gray-600 text-sm">Operations Manager, TechGadgets</p>
                        </div>
                    </div>
                </div>
                
                <!-- Testimonial 3 -->
                <div class="bg-white p-8 rounded-lg shadow-sm">
                    <div class="flex items-center mb-4">
                        <div class="text-yellow-400 mr-2">
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star"></i>
                            <i class="fas fa-star-half-alt"></i>
                        </div>
                    </div>
                    <p class="text-gray-600 italic mb-6">"We switched to SwiftShip last year and have saved over 30% on shipping costs while improving delivery times. Their enterprise solutions are perfect for our growing business."</p>
                    <div class="flex items-center">
                        <img class="w-12 h-12 rounded-full mr-4" src="https://randomuser.me/api/portraits/women/68.jpg" alt="Emma Rodriguez">
                        <div>
                            <h4 class="font-bold">Emma Rodriguez</h4>
                            <p class="text-gray-600 text-sm">Director, Global Imports</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- CTA Section -->
    <section class="gradient-bg text-white py-16">
        <div class="container mx-auto px-6 text-center">
            <h2 class="text-3xl font-bold mb-6">Ready to Ship With Us?</h2>
            <p class="text-xl mb-8 max-w-2xl mx-auto">Join thousands of businesses that trust SwiftShip for their shipping needs.</p>
            <div class="flex flex-col sm:flex-row justify-center gap-4">
                <button class="bg-white text-blue-600 hover:bg-gray-100 font-bold py-3 px-8 rounded-full text-lg transition duration-300">
                    <i class="fas fa-box mr-2"></i> Get Started
                </button>
                <button class="border-2 border-white text-white hover:bg-white hover:text-blue-600 font-bold py-3 px-8 rounded-full text-lg transition duration-300">
                    <i class="fas fa-phone-alt mr-2"></i> Contact Sales
                </button>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-20 bg-white">
        <div class="container mx-auto px-6">
            <div class="flex flex-col lg:flex-row">
                <div class="lg:w-1/2 mb-12 lg:mb-0 lg:pr-12">
                    <h2 class="text-3xl font-bold text-gray-800 mb-6">Contact Our Team</h2>
                    <p class="text-gray-600 mb-8">Have questions or need assistance? Our customer service team is available 24/7 to help with your shipping needs.</p>
                    
                    <div class="space-y-6">
                        <div class="flex items-start">
                            <div class="bg-blue-100 p-3 rounded-full mr-4 mt-1">
                                <i class="fas fa-phone-alt text-blue-600"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-gray-800 mb-2">Phone Support</h4>
                                <p class="text-gray-600">(800) 123-4567</p>
                                <p class="text-sm text-gray-500">Available 24/7</p>
                            </div>
                        </div>
                        
                        <div class="flex items-start">
                            <div class="bg-blue-100 p-3 rounded-full mr-4 mt-1">
                                <i class="fas fa-envelope text-blue-600"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-gray-800 mb-2">Email Support</h4>
                                <p class="text-gray-600">support@swiftship.com</p>
                                <p class="text-sm text-gray-500">Typically responds within 1 hour</p>
                            </div>
                        </div>
                        
                        <div class="flex items-start">
                            <div class="bg-blue-100 p-3 rounded-full mr-4 mt-1">
                                <i class="fas fa-comment-alt text-blue-600"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-gray-800 mb-2">Live Chat</h4>
                                <p class="text-gray-600">Available on our website</p>
                                <p class="text-sm text-gray-500">Mon-Fri: 8AM-8PM EST</p>
                            </div>
                        </div>
                        
                        <div class="flex items-start">
                            <div class="bg-blue-100 p-3 rounded-full mr-4 mt-1">
                                <i class="fas fa-map-marker-alt text-blue-600"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-gray-800 mb-2">Corporate Office</h4>
                                <p class="text-gray-600">123 Shipping Lane<br>New York, NY 10001<br>United States</p>
                            </div>
                        </div>
                    </div>
                </div>
                
                <div class="lg:w-1/2">
                    <form class="bg-gray-50 p-8 rounded-lg shadow-md">
                        <h3 class="text-xl font-bold text-gray-800 mb-6">Send Us a Message</h3>
                        
                        <div class="grid grid-cols-1 md:grid-cols-2 gap-6 mb-6">
                            <div>
                                <label for="first-name" class="block text-gray-700 font-medium mb-2">First Name</label>
                                <input type="text" id="first-name" class="w-full px-4 py-3 rounded-lg border border-gray-300 focus:outline-none focus:border-blue-500">
                            </div>
                            <div>
                                <label for="last-name" class="block text-gray-700 font-medium mb-2">Last Name</label>
                                <input type="text" id="last-name" class="w-full px-4 py-3 rounded-lg border border-gray-300 focus:outline-none focus:border-blue-500">
                            </div>
                        </div>
                        
                        <div class="mb-6">
                            <label for="email" class="block text-gray-700 font-medium mb-2">Email Address</label>
                            <input type="email" id="email" class="w-full px-4 py-3 rounded-lg border border-gray-300 focus:outline-none focus:border-blue-500">
                        </div>
                        
                        <div class="mb-6">
                            <label for="subject" class="block text-gray-700 font-medium mb-2">Subject</label>
                            <select id="subject" class="w-full px-4 py-3 rounded-lg border border-gray-300 focus:outline-none focus:border-blue-500">
                                <option>General Inquiry</option>
                                <option>Tracking Assistance</option>
                                <option>Billing Question</option>
                                <option>Shipping Rates</option>
                                <option>Other</option>
                            </select>
                        </div>
                        
                        <div class="mb-6">
                            <label for="message" class="block text-gray-700 font-medium mb-2">Message</label>
                            <textarea id="message" rows="5" class="w-full px-4 py-3 rounded-lg border border-gray-300 focus:outline-none focus:border-blue-500"></textarea>
                        </div>
                        
                        <button type="submit" class="w-full bg-blue-600 hover:bg-blue-700 text-white font-bold py-3 px-4 rounded-lg transition duration-300">
                            Send Message
                        </button>
                    </form>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-900 text-white pt-16 pb-8">
        <div class="container mx-auto px-6">
            <div class="flex flex-col md:flex-row justify-between mb-12">
                <div class="mb-8 md:mb-0">
                    <h3 class="text-2xl font-bold mb-4">Swift<span class="text-blue-400">Ship</span></h3>
                    <p class="text-gray-400 mb-4 max-w-xs">Delivering excellence in logistics and shipping solutions worldwide.</p>
                    <div class="flex space-x-4">
                        <a href="#" class="text-gray-400 hover:text-white transition duration-300">
                            <i class="fab fa-facebook-f"></i>
                        </a>
                        <a href="#" class="text-gray-400 hover:text-white transition duration-300">
                            <i class="fab fa-twitter"></i>
                        </a>
                        <a href="#" class="text-gray-400 hover:text-white transition duration-300">
                            <i class="fab fa-instagram"></i>
                        </a>
                        <a href="#" class="text-gray-400 hover:text-white transition duration-300">
                            <i class="fab fa-linkedin-in"></i>
                        </a>
                    </div>
                </div>
                
                <div class="grid grid-cols-2 md:grid-cols-4 gap-8">
                    <div>
                        <h4 class="text-lg font-semibold mb-4">Services</h4>
                        <ul class="space-y-2">
                            <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Express Shipping</a></li>
                            <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">International</a></li>
                            <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Freight</a></li>
                            <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Warehousing</a></li>
                        </ul>
                    </div>
                    
                    <div>
                        <h4 class="text-lg font-semibold mb-4">Company</h4>
                        <ul class="space-y-2">
                            <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">About Us</a></li>
                            <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Careers</a></li>
                            <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">News</a></li>
                            <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Partners</a></li>
                        </ul>
                    </div>
                    
                    <div>
                        <h4 class="text-lg font-semibold mb-4">Resources</h4>
                        <ul class="space-y-2">
                            <li><a href="tracking.html" class="text-gray-400 hover:text-white transition duration-300">Tracking</a></li>
                            <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Shipping Rates</a></li>
                            <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Support Center</a></li>
                            <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">API Documentation</a></li>
                        </ul>
                    </div>
                    
                    <div>
                        <h4 class="text-lg font-semibold mb-4">Legal</h4>
                        <ul class="space-y-2">
                            <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Terms of Service</a></li>
                            <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Privacy Policy</a></li>
                            <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Cookie Policy</a></li>
                            <li><a href="#" class="text-gray-400 hover:text-white transition duration-300">Shipping Policy</a></li>
                        </ul>
                    </div>
                </div>
            </div>
            
            <div class="border-t border-gray-800 pt-8 flex flex-col md:flex-row justify-between items-center">
                <p class="text-gray-400 mb-4 md:mb-0">© 2023 SwiftShip. All rights reserved.</p>
                <div class="flex flex-col sm:flex-row sm:space-x-6 space-y-2 sm:space-y-0 text-center">
                    <a href="#" class="text-gray-400 hover:text-white transition duration-300">Privacy Policy</a>
                    <a href="#" class="text-gray-400 hover:text-white transition duration-300">Terms of Service</a>
                    <a href="#" class="text-gray-400 hover:text-white transition duration-300">Sitemap</a>
                </div>
            </div>
        </div>
    </footer>

    <!-- Back to Top Button -->
    <button id="back-to-top" class="fixed bottom-8 right-8 bg-blue-600 text-white p-4 rounded-full shadow-lg hidden hover:bg-blue-700 transition duration-300">
        <i class="fas fa-arrow-up"></i>
    </button>

    <script>
        // Mobile menu toggle
        const mobileMenuButton = document.getElementById('menu-btn');
        const mobileMenu = document.getElementById('mobile-menu');
        
        mobileMenuButton.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });
        
        // Smooth scrolling for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                
                const targetId = this.getAttribute('href');
                if (targetId === '#') return;
                
                const targetElement = document.querySelector(targetId);
                if (targetElement) {
                    targetElement.scrollIntoView({
                        behavior: 'smooth'
                    });
                    
                    // Close mobile menu if open
                    if (!mobileMenu.classList.contains('hidden')) {
                        mobileMenu.classList.add('hidden');
                    }
                }
            });
        });
        
        // Back to top button
        const backToTopButton = document.getElementById('back-to-top');
        
        window.addEventListener('scroll', () => {
            if (window.pageYOffset > 300) {
                backToTopButton.classList.remove('hidden');
            } else {
                backToTopButton.classList.add('hidden');
            }
        });
        
        backToTopButton.addEventListener('click', () => {
            window.scrollTo({
                top: 0,
                behavior: 'smooth'
            });
        });
        
        // Form submission
        const contactForm = document.querySelector('form');
        if (contactForm) {
            contactForm.addEventListener('submit', (e) => {
                e.preventDefault();
                alert('Thank you for your message! Our team will get back to you soon.');
                contactForm.reset();
            });
        }
        
        // Tracking form submission
        const trackingForm = document.querySelector('.tracking-input')?.parentElement;
        if (trackingForm) {
            trackingForm.addEventListener('submit', (e) => {
                e.preventDefault();
                // In a real implementation, this would redirect to the tracking page with the tracking number
                window.location.href = 'tracking.html?tracking=' + document.querySelector('.tracking-input').value;
            });
        }
    </script>
</body>
</html>
