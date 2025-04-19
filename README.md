<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SMM Panel Services</title>
    <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.2.19/dist/tailwind.min.css" rel="stylesheet">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@fortawesome/fontawesome-free@6.0.0/css/all.min.css">
    <style>
        body {
            font-family: 'Poppins', sans-serif;
            color: #333;
            background-color: #f8f9fa;
        }
        .gradient-bg {
            background: linear-gradient(90deg, #4f46e5 0%, #7c3aed 100%);
        }
        .card {
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0,0,0,0.1);
        }
        .testimonial {
            background-color: #fff;
            border-radius: 10px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
        }
        .step-card {
            background-color: white;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
            transition: all 0.3s ease;
        }
        .step-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 15px rgba(0,0,0,0.1);
        }
        .modal {
            transition: opacity 0.3s ease;
        }
    </style>
</head>
<body class="overflow-x-hidden">
    <!-- Header -->
    <header class="bg-white shadow-sm sticky top-0 z-50">
        <nav class="container mx-auto px-6 py-3 flex justify-between items-center">
            <div class="flex items-center">
                <h1 class="text-2xl font-bold text-indigo-600">SMM Panel</h1>
            </div>
            <div class="hidden md:flex items-center space-x-8">
                <a href="#services" class="text-gray-700 hover:text-indigo-600 transition">Services</a>
                <a href="#how-it-works" class="text-gray-700 hover:text-indigo-600 transition">How it Works</a>
                <a href="#testimonials" class="text-gray-700 hover:text-indigo-600 transition">Testimonials</a>
                <a href="#faq" class="text-gray-700 hover:text-indigo-600 transition">FAQ</a>
            </div>
            <div class="flex items-center space-x-4">
                <button onclick="openModal('loginModal')" class="px-4 py-2 rounded text-indigo-600 font-medium hover:bg-indigo-50 transition">Login</button>
                <button onclick="openModal('registerModal')" class="px-4 py-2 rounded bg-indigo-600 text-white font-medium hover:bg-indigo-700 transition">Register</button>
            </div>
        </nav>
    </header>

    <!-- Hero Section -->
    <section class="gradient-bg text-white py-20">
        <div class="container mx-auto px-6 text-center">
            <h1 class="text-4xl md:text-5xl font-bold mb-6">Best SMM Panel Service Provider</h1>
            <p class="text-xl mb-10 max-w-3xl mx-auto">Enjoy excellent social media marketing services at amazing prices! Boost your online presence with our premium SMM services.</p>
            <div class="flex flex-col md:flex-row justify-center gap-4">
                <button onclick="openModal('registerModal')" class="px-8 py-3 bg-white text-indigo-600 font-semibold rounded-lg hover:bg-gray-100 transition">Get Started</button>
                <a href="#services" class="px-8 py-3 bg-indigo-700 text-white font-semibold rounded-lg hover:bg-indigo-800 transition">View Services</a>
            </div>
        </div>
    </section>

    <!-- Features Section -->
    <section class="py-16 bg-white">
        <div class="container mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="text-3xl font-bold text-gray-800 mb-4">Why Choose Our SMM Panel?</h2>
                <p class="text-gray-600 max-w-2xl mx-auto">We provide high-quality social media services to help you grow your online presence efficiently.</p>
            </div>
            
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <div class="card p-6 bg-gray-50 rounded-lg shadow-sm">
                    <div class="text-indigo-500 mb-4">
                        <i class="fas fa-money-bill-wave text-3xl"></i>
                    </div>
                    <h3 class="text-xl font-semibold mb-2">Affordable Pricing</h3>
                    <p class="text-gray-600">We always make sure that our services are affordable for everyone.</p>
                </div>
                
                <div class="card p-6 bg-gray-50 rounded-lg shadow-sm">
                    <div class="text-indigo-500 mb-4">
                        <i class="fas fa-bolt text-3xl"></i>
                    </div>
                    <h3 class="text-xl font-semibold mb-2">Fast Delivery</h3>
                    <p class="text-gray-600">You can rest assured that your orders will be delivered quickly and efficiently.</p>
                </div>
                
                <div class="card p-6 bg-gray-50 rounded-lg shadow-sm">
                    <div class="text-indigo-500 mb-4">
                        <i class="fas fa-credit-card text-3xl"></i>
                    </div>
                    <h3 class="text-xl font-semibold mb-2">Multiple Payment Options</h3>
                    <p class="text-gray-600">Add funds via any payment option we provide for your convenience.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- How It Works Section -->
    <section id="how-it-works" class="py-16 bg-gray-50">
        <div class="container mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="text-3xl font-bold text-gray-800 mb-4">How It Works</h2>
                <p class="text-gray-600 max-w-2xl mx-auto">Four simple steps to start growing your social media presence</p>
            </div>
            
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8">
                <div class="step-card p-6 text-center">
                    <div class="w-16 h-16 bg-indigo-100 rounded-full flex items-center justify-center mx-auto mb-4">
                        <span class="text-2xl font-bold text-indigo-600">1</span>
                    </div>
                    <h3 class="text-xl font-semibold mb-2">Register & Log In</h3>
                    <p class="text-gray-600">Begin with signing up and then log in to your account.</p>
                </div>
                
                <div class="step-card p-6 text-center">
                    <div class="w-16 h-16 bg-indigo-100 rounded-full flex items-center justify-center mx-auto mb-4">
                        <span class="text-2xl font-bold text-indigo-600">2</span>
                    </div>
                    <h3 class="text-xl font-semibold mb-2">Add Funds</h3>
                    <p class="text-gray-600">Add funds to your account using your preferred payment method.</p>
                </div>
                
                <div class="step-card p-6 text-center">
                    <div class="w-16 h-16 bg-indigo-100 rounded-full flex items-center justify-center mx-auto mb-4">
                        <span class="text-2xl font-bold text-indigo-600">3</span>
                    </div>
                    <h3 class="text-xl font-semibold mb-2">Place Your Orders</h3>
                    <p class="text-gray-600">Select the services you need to help your business grow online.</p>
                </div>
                
                <div class="step-card p-6 text-center">
                    <div class="w-16 h-16 bg-indigo-100 rounded-full flex items-center justify-center mx-auto mb-4">
                        <span class="text-2xl font-bold text-indigo-600">4</span>
                    </div>
                    <h3 class="text-xl font-semibold mb-2">Amazing Results</h3>
                    <p class="text-gray-600">We'll notify you once your order is ready. Enjoy fantastic results!</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section id="services" class="py-16 bg-white">
        <div class="container mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="text-3xl font-bold text-gray-800 mb-4">Our Services</h2>
                <p class="text-gray-600 max-w-2xl mx-auto">We offer a wide range of social media marketing services to help you grow your online presence</p>
            </div>
            
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <div class="card p-6 rounded-lg shadow-sm border border-gray-200">
                    <div class="text-indigo-500 mb-4">
                        <i class="fab fa-instagram text-3xl"></i>
                    </div>
                    <h3 class="text-xl font-semibold mb-2">Instagram Services</h3>
                    <ul class="text-gray-600 space-y-2">
                        <li>• Instagram Followers</li>
                        <li>• Instagram Likes</li>
                        <li>• Instagram Views</li>
                        <li>• Instagram Comments</li>
                        <li>• Instagram Story Views</li>
                    </ul>
                    <button class="mt-6 w-full py-2 bg-indigo-600 text-white rounded hover:bg-indigo-700 transition">Order Now</button>
                </div>
                
                <div class="card p-6 rounded-lg shadow-sm border border-gray-200">
                    <div class="text-indigo-500 mb-4">
                        <i class="fab fa-facebook text-3xl"></i>
                    </div>
                    <h3 class="text-xl font-semibold mb-2">Facebook Services</h3>
                    <ul class="text-gray-600 space-y-2">
                        <li>• Facebook Page Likes</li>
                        <li>• Facebook Post Likes</li>
                        <li>• Facebook Followers</li>
                        <li>• Facebook Comments</li>
                        <li>• Facebook Group Members</li>
                    </ul>
                    <button class="mt-6 w-full py-2 bg-indigo-600 text-white rounded hover:bg-indigo-700 transition">Order Now</button>
                </div>
                
                <div class="card p-6 rounded-lg shadow-sm border border-gray-200">
                    <div class="text-indigo-500 mb-4">
                        <i class="fab fa-youtube text-3xl"></i>
                    </div>
                    <h3 class="text-xl font-semibold mb-2">YouTube Services</h3>
                    <ul class="text-gray-600 space-y-2">
                        <li>• YouTube Subscribers</li>
                        <li>• YouTube Views</li>
                        <li>• YouTube Likes</li>
                        <li>• YouTube Comments</li>
                        <li>• YouTube Watch Time Hours</li>
                    </ul>
                    <button class="mt-6 w-full py-2 bg-indigo-600 text-white rounded hover:bg-indigo-700 transition">Order Now</button>
                </div>
                
                <div class="card p-6 rounded-lg shadow-sm border border-gray-200">
                    <div class="text-indigo-500 mb-4">
                        <i class="fab fa-twitter text-3xl"></i>
                    </div>
                    <h3 class="text-xl font-semibold mb-2">Twitter Services</h3>
                    <ul class="text-gray-600 space-y-2">
                        <li>• Twitter Followers</li>
                        <li>• Twitter Likes</li>
                        <li>• Twitter Retweets</li>
                        <li>• Twitter Comments</li>
                        <li>• Twitter Poll Votes</li>
                    </ul>
                    <button class="mt-6 w-full py-2 bg-indigo-600 text-white rounded hover:bg-indigo-700 transition">Order Now</button>
                </div>
                
                <div class="card p-6 rounded-lg shadow-sm border border-gray-200">
                    <div class="text-indigo-500 mb-4">
                        <i class="fab fa-tiktok text-3xl"></i>
                    </div>
                    <h3 class="text-xl font-semibold mb-2">TikTok Services</h3>
                    <ul class="text-gray-600 space-y-2">
                        <li>• TikTok Followers</li>
                        <li>• TikTok Likes</li>
                        <li>• TikTok Views</li>
                        <li>• TikTok Comments</li>
                        <li>• TikTok Shares</li>
                    </ul>
                    <button class="mt-6 w-full py-2 bg-indigo-600 text-white rounded hover:bg-indigo-700 transition">Order Now</button>
                </div>
                
                <div class="card p-6 rounded-lg shadow-sm border border-gray-200">
                    <div class="text-indigo-500 mb-4">
                        <i class="fas fa-globe text-3xl"></i>
                    </div>
                    <h3 class="text-xl font-semibold mb-2">Other Services</h3>
                    <ul class="text-gray-600 space-y-2">
                        <li>• Spotify Plays & Followers</li>
                        <li>• SoundCloud Plays & Likes</li>
                        <li>• Telegram Members</li>
                        <li>• Website Traffic</li>
                        <li>• Discord Members</li>
                    </ul>
                    <button class="mt-6 w-full py-2 bg-indigo-600 text-white rounded hover:bg-indigo-700 transition">Order Now</button>
                </div>
            </div>
        </div>
    </section>

    <!-- Testimonials Section -->
    <section id="testimonials" class="py-16 bg-gray-50">
        <div class="container mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="text-3xl font-bold text-gray-800 mb-4">What Our Customers Say</h2>
                <p class="text-gray-600 max-w-2xl mx-auto">Read what our customers have to say about our services</p>
            </div>
            
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <div class="testimonial p-6">
                    <div class="flex items-center mb-4">
                        <div class="w-12 h-12 bg-indigo-100 rounded-full flex items-center justify-center mr-4">
                            <i class="fas fa-user text-indigo-600"></i>
                        </div>
                        <div>
                            <h4 class="font-semibold">Brad Garcia</h4>
                            <div class="flex text-yellow-400">
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                            </div>
                        </div>
                    </div>
                    <p class="text-gray-600">Keep up the great work, guys! If you aren't sure where to order SMM services to promote your business, go with this SMM panel you won't regret it.</p>
                </div>
                
                <div class="testimonial p-6">
                    <div class="flex items-center mb-4">
                        <div class="w-12 h-12 bg-indigo-100 rounded-full flex items-center justify-center mr-4">
                            <i class="fas fa-user text-indigo-600"></i>
                        </div>
                        <div>
                            <h4 class="font-semibold">Mike Wong</h4>
                            <div class="flex text-yellow-400">
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                            </div>
                        </div>
                    </div>
                    <p class="text-gray-600">Finding this SMM panel helped me save SO much time and money on building social media accounts for my company! I've never had a problem with these guys which is why I highly recommend their services.</p>
                </div>
                
                <div class="testimonial p-6">
                    <div class="flex items-center mb-4">
                        <div class="w-12 h-12 bg-indigo-100 rounded-full flex items-center justify-center mr-4">
                            <i class="fas fa-user text-indigo-600"></i>
                        </div>
                        <div>
                            <h4 class="font-semibold">Asil Kocak</h4>
                            <div class="flex text-yellow-400">
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                            </div>
                        </div>
                    </div>
                    <p class="text-gray-600">I do SMM promotions for different businesses and this panel has been such a great discovery for me! I used to spend lots of time doing some tasks that can be done super quickly now because SMM services here are delivered so fast. Thank you guys!</p>
                </div>
            </div>
        </div>
    </section>

    <!-- FAQ Section -->
    <section id="faq" class="py-16 bg-white">
        <div class="container mx-auto px-6">
            <div class="text-center mb-16">
                <h2 class="text-3xl font-bold text-gray-800 mb-4">Frequently Asked Questions</h2>
                <p class="text-gray-600 max-w-2xl mx-auto">Find answers to the most common questions about our services</p>
            </div>
            
            <div class="max-w-3xl mx-auto">
                <div class="mb-6 border-b border-gray-200 pb-6">
                    <h3 class="text-xl font-semibold mb-2">What is an SMM panel?</h3>
                    <p class="text-gray-600">SMM panels are online stores that offer SMM services of different kinds, including likes, followers, views, and more for various social media platforms.</p>
                </div>
                
                <div class="mb-6 border-b border-gray-200 pb-6">
                    <h3 class="text-xl font-semibold mb-2">What services do you offer?</h3>
                    <p class="text-gray-600">Our panel provides different types of SMM services, such as likes, views, followers, and more for platforms like Instagram, Facebook, YouTube, Twitter, TikTok, and others.</p>
                </div>
                
                <div class="mb-6 border-b border-gray-200 pb-6">
                    <h3 class="text-xl font-semibold mb-2">Is using your SMM services safe?</h3>
                    <p class="text-gray-600">Using our SMM services is definitely safe, and you won't lose your accounts. We use methods that comply with social media platforms' terms of service.</p>
                </div>
                
                <div class="mb-6 border-b border-gray-200 pb-6">
                    <h3 class="text-xl font-semibold mb-2">What is a mass order?</h3>
                    <p class="text-gray-600">The mass order feature allows you to place multiple orders at once, saving you time when you need to order services for multiple links.</p>
                </div>
                
                <div class="mb-6">
                    <h3 class="text-xl font-semibold mb-2">What is drip-feed?</h3>
                    <p class="text-gray-600">Drip-feed allows you to build engagement on your account at the speed that you want. For example, instead of getting 10
