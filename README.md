# Universebeautyskincare.github.io
Online skincare retail shop
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>UNIVERSE Skincare</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@100..900&display=swap" rel="stylesheet">
    
<script type="module" src="https://unpkg.com/lucide@latest"></script>
    <script src="https://unpkg.com/html5-qrcode@2.3.8/minified/html5-qrcode.min.js"></script>
    
    <style>
        /* Custom styles for the mobile app feel */
        body {
            font-family: 'Inter', sans-serif;
            background-color: #0c4a6e; /* Deep blue background */
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            margin: 0;
        }

        /* Simulating the device frame and dark app background */
        .app-container {
            width: 100%;
            max-width: 400px; /* Standard mobile width */
            height: 800px; /* Fixed height for mobile simulation */
            background: #0d0c1d; /* Very dark background */
            box-shadow: 0 20px 50px rgba(0, 0, 0, 0.5);
            border-radius: 30px;
            overflow: hidden;
            display: flex;
            flex-direction: column;
            position: relative;
        }

        /* Header gradient to match the template */
        .app-header {
            background: linear-gradient(135deg, #1c193f, #312e81, #4f46e5);
        }

        /* Content area that scrolls */
        .app-content {
            flex-grow: 1;
            overflow-y: auto;
            padding: 1rem;
            -ms-overflow-style: none; /* IE and Edge */
            scrollbar-width: none; /* Firefox */
        }
        .app-content::-webkit-scrollbar {
            display: none; /* Chrome, Safari and Opera */
        }

        /* Product image gradient borders/glow */
        .product-card {
            border: 2px solid transparent;
            border-radius: 12px;
            background-clip: padding-box, border-box;
            background-origin: padding-box, border-box;
            background-image: linear-gradient(#0d0c1d, #0d0c1d), linear-gradient(to right, #4f46e5, #312e81);
            transition: transform 0.2s, box-shadow 0.2s;
        }
        .product-card:hover {
             transform: translateY(-2px);
             box-shadow: 0 10px 15px -3px rgba(79, 70, 229, 0.2), 0 4px 6px -2px rgba(79, 70, 229, 0.05);
        }

        .active-nav {
            transform: scale(1.1);
            color: #818cf8;
        }

        /* Icon styling for social links */
        .social-icon {
            transition: all 0.2s;
            cursor: pointer;
        }
        .social-icon:hover {
            color: #a78bfa;
            transform: translateY(-2px);
        }

        /* Styling for the mobile shop filter bar */
        .mobile-shop-nav {
            background: #1c193f;
            box-shadow: 0 -5px 20px rgba(0, 0, 0, 0.5);
            border-top: 1px solid #4f46e550;
        }

        /* Custom badge styles for the dark theme */
        .product-badge {
            @apply absolute top-0 left-0 text-xs font-semibold px-2 py-0.5 rounded-br-lg;
        }
        .official-store-badge {
            @apply bg-indigo-600 text-white;
        }
        .pay-on-delivery-badge {
            @apply bg-green-500 text-white;
        }
        .discount-badge {
            @apply bg-pink-500 text-white;
        }

        /* Custom styling for quantity buttons */
        .qty-btn {
            @apply bg-indigo-700 text-white w-6 h-6 rounded-full text-lg leading-none flex items-center justify-center transition hover:bg-indigo-600 active:scale-95;
        }
        /* Style for the QR code scanner box */
        #reader video {
            border-radius: 8px;
            width: 100% !important; /* Ensure video fits the container */
            max-height: 250px;
        }

        /* Styling for Admin Form inputs */
        .admin-input {
            @apply w-full p-3 bg-gray-700/50 text-white rounded-lg border border-indigo-500/50 focus:ring-2 focus:ring-indigo-400 focus:outline-none transition;
        }
        
    </style>
</head>
<body class="selection:bg-indigo-300 selection:text-indigo-900">

<div id="app" class="app-container">

    
<header id="app-header" class="app-header p-4 text-white shadow-lg h-36 flex flex-col justify-between">
        <div class="flex justify-between items-center text-xs font-semibold">
            <span class="text-gray-400">HOME SHOP CART AUTH</span>
            <span class="text-gray-400">9:41 AM</span>
        </div>
        <div class="flex items-center mt-2 flex-grow">
            
<div class="w-20 h-20 flex-shrink-0">
                <a href="https://ibb.co/Z6djmTW9" class="block w-full h-full"><img src="https://i.ibb.co/zhsMJfGd/IMG-0365.jpg" alt="UNIVERSE Logo" class="w-full h-full object-contain border-0"></a>
            </div>
            <div class="ml-4 flex-grow">
                <h1 class="text-lg font-bold">UNIVERSE</h1>
                <p class="text-sm text-gray-300">cosmetics and beauty skincare</p>
            </div>
        </div>
    </header>

    
<main id="main-content" class="app-content">

        
<div id="home-view" class="page-view" data-page="home">
            <div class="w-full h-8 bg-indigo-600 rounded-lg flex items-center justify-center mb-6">
                <h2 class="text-white text-base font-semibold tracking-wider">HOME</h2>
            </div>
            
            <section class="mb-8 rounded-xl overflow-hidden shadow-2xl product-card border-none p-0">
                <div class="relative w-full h-[300px] overflow-hidden">
                    <img src="https://i.ibb.co/nMNNJ4TH/IMG-0481.jpg"
                         alt="UNIVERSE Radiance Skincare Banner" 
                         class="w-full h-full object-cover brightness-75"
                         onerror="this.onerror=null;this.src='https://placehold.co/400x600/1c193f/d1d5db?text=Image+Load+Error';"
                    >
                    
                    <div class="absolute inset-0 flex items-center justify-center p-4">
                        <h3 class="text-3xl font-extrabold text-white text-center tracking-wider leading-snug drop-shadow-lg">
                            Unveiling your radiance
                        </h3>
                    </div>
                </div>
            </section>
            <section class="mb-8">
                <h3 class="text-xl font-extrabold text-white mb-4 border-b border-indigo-400/50 pb-2">ABOUT</h3>
                <div class="grid grid-cols-1 md:grid-cols-2 gap-4 items-center">
                    <p class="text-gray-300 leading-relaxed text-sm">
                        This company strives in providing you products that helps unveil your radiance, shine with us today. We believe true beauty starts with healthy, nourished skin, and we're committed to sourcing only the best ingredients.
                    </p>
                    <div class="rounded-xl overflow-hidden shadow-2xl product-card">
                        <a href="https://ibb.co/KjsVX3VM" class="block w-full h-auto">
                            <img src="https://i.ibb.co/fYNr2Prh/IMG-0390.jpg" alt="Skincare products" class="w-full h-auto object-cover transition-transform duration-300 hover:scale-[1.03] border-0">
                        </a>
                    </div>
                </div>
            </section>

            <section class="mt-8 mb-8 pt-4 border-t border-indigo-400/50">
                <h3 class="text-xl font-extrabold text-white mb-4">NEW ARRIVALS</h3>
                <div class="grid grid-cols-2 gap-4 mb-6">
                    <div class="rounded-lg overflow-hidden shadow-xl product-card p-1">
                        <a href="https://ibb.co/HTN8Tq2C" class="block">
                            <img src="https://i.ibb.co/N21B2K3r/IMG-0391.jpg" alt="New Product 1" class="w-full h-auto object-cover rounded-lg">
                        </a>
                    </div>
                    <div class="rounded-lg overflow-hidden shadow-xl product-card p-1">
                        <a href="https://ibb.co/k64VFFWR" class="block">
                            <img src="https://i.ibb.co/fGkV77Ph/IMG-0389.jpg" alt="New Product 2" class="w-full h-auto object-cover rounded-lg">
                        </a>
                    </div>
                </div>

                <button onclick="navigateTo('shop')" class="w-full py-3 bg-indigo-600 text-white font-bold text-lg rounded-xl shadow-lg hover:bg-indigo-700 transition duration-200 transform hover:scale-[1.01] flex items-center justify-center">
                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-shopping-bag mr-3"><path d="M6 2L3 7v14a2 2 0 0 0 2 2h14a2 2 0 0 0 2-2V7l-3-5Z"/><path d="M3 7h18"/><path d="M16 10a4 4 0 0 1-8 0"/></svg>
                    SHOP NEW ARRIVALS
                </button>
            </section>
            <section class="mt-8 mb-8 pt-4 border-t border-indigo-400/50">
                <div class="p-6 bg-indigo-900/40 rounded-xl shadow-inner border border-indigo-700/50">
                    <h3 class="text-lg font-bold text-white mb-3">LOCATION & CONTACT</h3>
                    <p class="text-gray-300">
                        <strong class="text-indigo-400">Location:</strong> A09 Plateau Plaza International Trade Fair Lagos
                    </p>
                    <p class="text-gray-300 mt-1">
                        <strong class="text-indigo-400">Contact:</strong> 07044292747
                    </p>

                    <div class="flex flex-col space-y-4 mt-5 text-2xl text-white">
                        
                        <div class="flex items-center">
                            <a href="#" class="social-icon text-pink-400 flex-shrink-0">
                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-instagram"><rect width="20" height="20" x="2" y="2" rx="5" ry="5"/><path d="M16 11.37A4 4 0 1 1 12.63 8 4 4 0 0 1 16 11.37z"/><line x1="17.5" x2="17.51" y1="6.5" y2="6.5"/></svg>
                            </a>
                            <span class="text-xs text-indigo-400 ml-3">@universe_cosmetics_beauty_skin</span>
                        </div>

                        <div class="flex items-center">
                            <a href="#" class="social-icon flex-shrink-0">
                                
<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-music-3">
                                    <path d="M11 18v-5.172a2 2 0 1 0-4 0v5.172a2 2 0 1 0 4 0Z"/><path d="M17 18v-5.172a2 2 0 1 0-4 0v5.172a2 2 0 1 0 4 0Z"/><path d="M11 13h6"/>
                                </svg>
                            </a>
                            <span class="text-xs text-gray-500 ml-3">@TikTok_Handle</span>
                        </div>
                        
                        <div class="flex items-center">
                            <a href="#" class="social-icon text-green-400 flex-shrink-0">
                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-message-circle"><path d="m21 11.5c.34-1.34 0-2.61-1.3-4.7-1.32-2.1-3.65-2.68-4.88-2.68-2.3 0-3.68.74-5.26 2.32-1.58 1.57-2.32 2.96-2.32 5.26 0 1.23.58 3.56 2.68 4.88 2.1 1.3 3.37 1.64 4.7 1.3 1.34-.34 2.61 0 4.7 1.3 2.1 1.32 2.68 3.65 2.68 4.88 0 2.3-.74 3.68-2.32 5.26-1.57 1.58-2.96 2.32-5.26 2.32-1.23 0-3.56-.58-4.88-2.68-1.3-2.1-1.64-3.37-1.3-4.7"/></svg>
                            </a>
                            <span class="text-xs text-gray-500 ml-3">Chat on WhatsApp</span>
                        </div>
                    </div>
                </div>
            </section>
            <section class="mt-8 pt-4 border-t border-indigo-400/50">
                <h3 class="text-xl font-extrabold text-white mb-4">TESTIMONIALS</h3>
                <div class="space-y-4">
                    <div class="p-4 rounded-xl bg-indigo-900/40 text-sm">
                        <p class="text-gray-200 italic">"My skin has never felt better. The products are truly transformative!"</p>
                        <p class="text-right text-indigo-400 mt-2">— Sarah L.</p>
                    </div>
                    <div class="p-4 rounded-xl bg-indigo-900/40 text-sm">
                        <p class="text-gray-200 italic">"Fast shipping and amazing customer support. Highly recommend UNIVERSE!"</p>
                        <p class="text-right text-indigo-400 mt-2">— David B.</p>
                    </div>
                </div>
            </section>
        </div>

        
<div id="shop-view" class="page-view hidden" data-page="shop">
            <div class="w-full h-8 bg-indigo-600 rounded-lg flex items-center justify-center mb-6">
                <h2 class="text-white text-base font-semibold tracking-wider">SHOP NOW</h2>
            </div>
            
            <section class="pb-16">
                <div id="product-grid" class="grid grid-cols-2 gap-4">
                    <p id="shop-loading-message" class="col-span-2 text-center text-gray-400 py-12">Loading products...</p>
                </div>
            </section>
            <section class="mt-8 pt-4 border-t border-indigo-400/50">
                <h3 class="text-xl font-extrabold text-white mb-4">CUSTOMER REVIEWS</h3>
                <div class="space-y-4">
                    <div class="flex items-start p-4 rounded-xl bg-indigo-900/40 border border-indigo-700/50">
                        <img src="https://placehold.co/64x64/4c051e/ffffff?text=User" onerror="this.onerror=null;this.src='https://placehold.co/64x64/4c051e/ffffff?text=User';" alt="Portrait of a happy Black woman using UNIVERSE products" class="w-12 h-12 rounded-full object-cover mr-4 flex-shrink-0">
                        <div class="flex-grow">
                            <p class="text-gray-200 italic text-sm">"The Radiant Glow Serum is a game-changer! It's lightweight and gives my skin a flawless, non-oily finish. Absolutely essential for my routine."</p>
                            <p class="text-right text-indigo-400 font-semibold mt-2">— Jessica A.</p>
                        </div>
                    </div>
                    <div class="flex items-start p-4 rounded-xl bg-indigo-900/40 border border-indigo-700/50">
                        <img src="https://placehold.co/64x64/2d1740/ffffff?text=User" onerror="this.onerror=null;this.src='https://placehold.co/64x64/2d1740/ffffff?text=User';" alt="Portrait of a satisfied Black woman customer" class="w-12 h-12 rounded-full object-cover mr-4 flex-shrink-0">
                        <div class="flex-grow">
                            <p class="text-gray-200 italic text-sm">"I was skeptical, but the Moisturizing Cream completely cleared up my dry patches. It feels rich without being heavy—perfection!"</p>
                            <p class="text-right text-indigo-400 font-semibold mt-2">— Nala O.</p>
                        </div>
                    </div>
                </div>
            </section>
            </div>

        
<div id="cart-view" class="page-view hidden" data-page="cart">
            <div class="w-full h-8 bg-indigo-600 rounded-lg flex items-center justify-center mb-6">
                <h2 class="text-white text-base font-semibold tracking-wider">SHOPPING CART</h2>
            </div>

            <div id="cart-items-container" class="space-y-4 mb-8">
                <p class="text-gray-400 text-center py-12" id="cart-empty-message">
                    Your cart is empty. Time to find your radiance!
                </p>
            </div>
            
            <button onclick="clearCart()" id="clear-cart-btn" class="w-full py-2 mb-4 bg-red-600 text-white font-bold text-sm rounded-xl shadow-lg hover:bg-red-700 transition duration-200 transform hover:scale-[1.01] flex items-center justify-center hidden">
                <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-trash-2 mr-2"><path d="M3 6h18"/><path d="M19 6v14c0 1-1 2-2 2H7c-1 0-2-1-2-2V6"/><path d="M10 11v6"/><path d="M14 11v6"/><path d="M8 6V4c0-1 1-2 2-2h4c1 0 2 1 2 2v2"/></svg>
                CLEAR ENTIRE CART
            </button>


            <div id="cart-summary" class="sticky bottom-0 bg-gray-900/50 p-4 rounded-xl border border-indigo-700/50">
                <div class="flex justify-between items-center text-lg mb-3">
                    <span class="text-gray-300 font-semibold">Subtotal:</span>
                    <span id="cart-subtotal" class="text-white font-bold">$0.00</span>
                </div>
                <div class="flex justify-between items-center text-lg mb-4 border-b border-indigo-700/50 pb-3">
                    <span class="text-gray-300 font-semibold">Shipping:</span>
                    <span class="text-white font-bold">FREE</span>
                </div>
                <div class="flex justify-between items-center text-xl">
                    <span class="text-indigo-400 font-extrabold">Total:</span>
                    <span id="cart-total" class="text-pink-400 font-extrabold">$0.00</span>
                </div>
                
                <button onclick="alertMessage('Checkout Initiated')" class="w-full py-3 mt-4 bg-pink-600 text-white font-bold text-lg rounded-xl shadow-lg hover:bg-pink-700 transition duration-200 transform hover:scale-[1.01] flex items-center justify-center">
                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-credit-card mr-3"><rect width="20" height="14" x="2" y="5" rx="2"/><line x1="2" x2="22" y1="10" y2="10"/></svg>
                    PROCEED TO CHECKOUT
                </button>
                <p id="auth-status-display" class="text-xs text-center text-gray-500 mt-2">
                    Loading user status...
                </p>
            </div>
        </div>

        
<div id="auth-view" class="page-view hidden" data-page="auth">
            <div class="w-full h-8 bg-pink-600 rounded-lg flex items-center justify-center mb-6">
                <h2 class="text-white text-base font-semibold tracking-wider" id="auth-header-title">QR SCANNER / ADMIN</h2>
            </div>

            <div id="admin-panel" class="hidden">
                <h3 class="text-2xl font-bold text-white mb-4 text-center">Product Management</h3>
                <p class="text-xs text-gray-400 text-center mb-4">You are currently signed in as the Administrator.</p>
                
                <div class="p-4 bg-indigo-900/40 rounded-xl mb-6 border border-indigo-700/50">
                    <h4 class="text-lg font-semibold text-indigo-300 mb-4" id="form-title">Add New Product</h4>
                    <form id="product-form" onsubmit="handleProductFormSubmit(event)">
                        <input type="hidden" id="product-doc-id" value="">
                        <div class="space-y-3">
                            <input type="text" id="product-name" class="admin-input" placeholder="Product Name" required>
                            <input type="number" id="product-price" class="admin-input" placeholder="Price (e.g., 45.00)" step="0.01" required>
                            <input type="number" id="product-line-through-price" class="admin-input" placeholder="Old Price (Optional, e.g., 55.00)" step="0.01">
                            <input type="text" id="product-img" class="admin-input" placeholder="Image URL (e.g., https://i.ibb.co/...)" required>
                            <input type="text" id="product-badge" class="admin-input" placeholder="Badge Text (e.g., Best Seller)">
                            <button type="submit" id="product-form-button" class="w-full py-3 bg-indigo-600 text-white font-bold rounded-lg hover:bg-indigo-700 transition">Add Product</button>
                            <button type="button" onclick="resetForm()" class="w-full py-3 bg-gray-600 text-white font-bold rounded-lg hover:bg-gray-700 transition">Cancel / New</button>
                        </div>
                    </form>
                </div>

                <div class="p-4 bg-gray-900/50 rounded-xl border border-gray-700/50">
                    <h4 class="text-lg font-semibold text-indigo-300 mb-4">Existing Products</h4>
                    <ul id="admin-product-list" class="space-y-3">
                        <li class="text-gray-400">Loading products...</li>
                    </ul>
                </div>

            </div>

            <div id="qr-scanner-content">
                <section class="p-4 bg-indigo-900/40 rounded-xl">
                    <h3 class="text-lg font-bold text-white mb-4 text-center">Scan to Authenticate or Learn More</h3>
                    
                    <div id="reader" class="w-full mx-auto" style="max-width: 300px;">
                        </div>

                    <div id="auth-result" class="mt-4 p-4 rounded-lg text-white text-center border border-indigo-500/50 shadow-inner min-h-16">
                        Scan Result: Waiting for camera permission...
                    </div>
                    <p class="text-xs text-gray-400 mt-3 text-center">
                        Tap the Auth tab to start and stop the scanner. This feature can be used to scan product tags or login keys.
                    </p>
                </section>
            </div>
            
        </div>
        </main>

    <div id="mobile-shop-nav" class="fixed bottom-16 left-0 right-0 h-14 mobile-shop-nav flex justify-around items-center z-40 hidden">
        <button onclick="alertMessage('Sort Feature')" class="flex items-center text-white/90 hover:text-indigo-400 transition-colors duration-200">
            <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-arrow-down-up mr-2"><path d="m3 16 4 4 4-4"/><path d="M7 20V4"/><path d="m21 8-4-4-4 4"/><path d="M17 4v16"/></svg>
            <span class="font-bold text-sm">Sort by</span>
        </button>
        <div class="w-px h-8 bg-indigo-700"></div>
        <button onclick="alertMessage('Filter Feature')" class="flex items-center text-white/90 hover:text-indigo-400 transition-colors duration-200">
            <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-sliders-horizontal mr-2"><path d="M21 17H3"/><path d="M21 12H3"/><path d="M21 7H3"/><path d="M18 10v4"/><path d="M6 5v4"/><path d="M14 15v4"/></svg>
            <span class="font-bold text-sm">Filter</span>
        </button>
    </div>


    
<footer class="flex justify-around items-center h-16 bg-[#1c193f] border-t border-indigo-500/30 text-gray-400 shadow-[0_-5px_20px_rgba(0,0,0,0.3)]">
        <button onclick="navigateTo('home')" id="nav-home" class="nav-button flex flex-col items-center p-2 rounded-lg transition-all duration-300 active-nav">
            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-home"><path d="m3 9 9-7 9 7v11a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2z"/><polyline points="9 22 9 12 15 12 15 22"/></svg>
            <span class="text-xs mt-1">Home</span>
        </button>
        <button onclick="navigateTo('shop')" id="nav-shop" class="nav-button flex flex-col items-center p-2 rounded-lg transition-all duration-300">
            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-shopping-bag"><path d="M6 2L3 7v14a2 2 0 0 0 2 2h14a2 2 0 0 0 2-2V7l-3-5Z"/><path d="M3 7h18"/><path d="M16 10a4 4 0 0 1-8 0"/></svg>
            <span class="text-xs mt-1">Shop</span>
        </button>
        <button onclick="navigateTo('cart')" id="nav-cart" class="nav-button flex flex-col items-center p-2 rounded-lg transition-all duration-300">
            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-shopping-cart"><circle cx="8" cy="20" r="1"/><circle cx="19" cy="20" r="1"/><path d="M2.5 2.5h2l2.64 10.37a2 2 0 0 0 1.95 1.63h8.84a2 2 0 0 0 1.95-1.63L21.5 7.5h-13"/></svg>
            <span class="text-xs mt-1">Cart</span>
        </button>
        <button onclick="navigateTo('auth')" id="nav-auth" class="nav-button flex flex-col items-center p-2 rounded-lg transition-all duration-300">
            <svg xmlns="http://www.w3.org/2300/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-scan"><path d="M3 7V5a2 2 0 0 1 2-2h2"/><path d="M17 3h2a2 2 0 0 1 2 2v2"/><path d="M21 17v2a2 2 0 0 1-2 2h-2"/><path d="M7 21H5a2 2 0 0 1-2-2v-2"/></svg>
            <span class="text-xs mt-1">Auth</span>
        </button>
    </footer>

    
<div id="message-box" class="fixed inset-0 bg-black/60 z-50 hidden items-center justify-center">
        <div class="bg-gray-800 p-6 rounded-xl shadow-2xl max-w-xs w-full text-center border-t-4 border-indigo-500">
            <p id="message-text" class="text-white text-lg mb-4"></p>
            <button onclick="hideMessage()" class="w-full bg-indigo-600 text-white py-2 rounded-lg font-semibold hover:bg-indigo-700 transition">OK</button>
        </div>
    </div>

    <div id="confirmation-box" class="fixed inset-0 bg-black/60 z-50 hidden items-center justify-center">
        <div class="bg-gray-800 p-6 rounded-xl shadow-2xl max-w-xs w-full text-center border-t-4 border-red-500">
            <p id="confirmation-text" class="text-white text-lg mb-4"></p>
            <div class="flex justify-between space-x-4">
                <button id="confirm-yes-btn" class="flex-1 bg-red-600 text-white py-2 rounded-lg font-semibold hover:bg-red-700 transition">Confirm</button>
                <button id="confirm-no-btn" class="flex-1 bg-gray-600 text-white py-2 rounded-lg font-semibold hover:bg-gray-700 transition">Cancel</button>
            </div>
        </div>
    </div>
    </div>

<script type="module">
    // --- Firebase Imports ---
    import { initializeApp } from "https://www.gstatic.com/firebasejs/11.6.1/firebase-app.js";
    import { getAuth, signInAnonymously, signInWithCustomToken, onAuthStateChanged } from "https://www.gstatic.com/firebasejs/11.6.1/firebase-auth.js";
    // *** UPDATED FIREBASE IMPORTS: Added writeBatch for clearCart function ***
    import { getFirestore, doc, collection, query, addDoc, setDoc, updateDoc, deleteDoc, onSnapshot, writeBatch } from "https://www.gstatic.com/firebasejs/11.6.1/firebase-firestore.js";
    import { setLogLevel } from "https://www.gstatic.com/firebasejs/11.6.1/firebase-firestore.js";
    // setLogLevel('debug'); // Optional: Uncomment to see detailed Firestore logs

    // --- App Configuration and Globals ---
    const appId = typeof __app_id !== 'undefined' ? __app_id : 'default-app-id';
    // NOTE: You must replace the empty object with your Firebase Config keys!
    const firebaseConfig = JSON.parse(typeof __firebase_config !== 'undefined' ? __firebase_config : '{}'); 
    const initialAuthToken = typeof __initial_auth_token !== 'undefined' ? __initial_auth_token : null;

    let db;
    let auth;
    let userId = null;
    let isCurrentUserAdmin = false;
    let productsLoaded = false;
    let cartListenerUnsubscribe = null;
    let productsListenerUnsubscribe = null;

    // Stores products as an object for quick lookup: { docId: { docId, name, price, ... } }
    let currentProductsMap = {};
    // Stores cart items: { docId: { cartDocId, quantity: N, data: ProductData } }
    let currentCartItems = {}; 

    // --- QR Scanner Globals ---
    let html5QrcodeScanner = null;

    // --- DOM Elements (Alert/Confirmation) ---
    const messageBox = document.getElementById('message-box');
    const messageText = document.getElementById('message-text');

    const confirmationBox = document.getElementById('confirmation-box');
    const confirmationText = document.getElementById('confirmation-text');
    const confirmYesBtn = document.getElementById('confirm-yes-btn');
    const confirmNoBtn = document.getElementById('confirm-no-btn');
    let resolveConfirmation = null;

    // --- DOM Elements (Main App) ---
    const navButtons = document.querySelectorAll('.nav-button');
    const mobileShopNav = document.getElementById('mobile-shop-nav');
    const mainContent = document.getElementById('main-content');
    const cartItemsContainer = document.getElementById('cart-items-container');
    const cartEmptyMessage = document.getElementById('cart-empty-message');
    const cartSubtotal = document.getElementById('cart-subtotal');
    const cartTotal = document.getElementById('cart-total');
    const authStatusDisplay = document.getElementById('auth-status-display');
    const authHeaderTitle = document.getElementById('auth-header-title');
    // *** NEW: Clear Cart Button element ***
    const clearCartBtn = document.getElementById('clear-cart-btn');

    // Admin/Auth View Elements
    const adminPanel = document.getElementById('admin-panel');
    const qrScannerContent = document.getElementById('qr-scanner-content');
    const authResultDisplay = document.getElementById('auth-result');
    const adminProductList = document.getElementById('admin-product-list');
    const productForm = document.getElementById('product-form');
    const productDocIdInput = document.getElementById('product-doc-id');
    const productNameInput = document.getElementById('product-name');
    const productPriceInput = document.getElementById('product-price');
    const productLineThroughPriceInput = document.getElementById('product-line-through-price');
    const productImgInput = document.getElementById('product-img');
    const productBadgeInput = document.getElementById('product-badge');
    const formTitle = document.getElementById('form-title');
    const formButton = document.getElementById('product-form-button');
    const productGrid = document.getElementById('product-grid');
    const shopLoadingMessage = document.getElementById('shop-loading-message');


    let currentPage = 'home';

    // --- Firebase Collection/Document References ---

    /** Gets the Firestore collection reference for all public products. */
    function getProductsCollectionRef() {
        if (!db) return null;
        // Public data: /artifacts/{appId}/public/data/products
        return collection(db, `artifacts/${appId}/public/data/products`);
    }

    /** Gets the Firestore document reference for the admin configuration. */
    function getAdminConfigDocRef() {
        if (!db) return null;
        // Public setting: /artifacts/{appId}/public/data/settings/adminConfig
        return doc(db, `artifacts/${appId}/public/data/settings/adminConfig`);
    }

    /** Gets the Firestore collection reference for the user's private cart. */
    function getCartCollectionRef() {
        if (!db || !userId) return null;
        // Private data: /artifacts/{appId}/users/{userId}/cart
        return collection(db, `artifacts/${appId}/users/${userId}/cart`);
    }

    // --- Firebase Initialization and Auth ---

    /** Initializes Firebase and sets up the authentication listener. */
    async function initializeFirebase() {
        if (Object.keys(firebaseConfig).length === 0) {
            console.error("Firebase config is empty. Cannot initialize.");
            authStatusDisplay.textContent = "Error: Firebase config missing.";
            return;
        }

        const app = initializeApp(firebaseConfig);
        db = getFirestore(app);
        auth = getAuth(app);

        // Sign in using the provided custom token or anonymously
        try {
            if (initialAuthToken) {
                await signInWithCustomToken(auth, initialAuthToken);
            } else {
                await signInAnonymously(auth);
            }
        } catch (error) {
            console.error("Firebase authentication failed:", error);
            authStatusDisplay.textContent = `Auth failed: ${error.code}`;
            return;
        }

        // Listen for auth state changes to set the userId
        onAuthStateChanged(auth, (user) => {
            if (user) {
                userId = user.uid;
                authStatusDisplay.textContent = `User ID: ${userId.substring(0, 8)}...`;
                console.log("User signed in with ID:", userId);
                loadProductsListener(); // Start listening to products immediately
                loadAdminStatusListener(); // Check/set admin status
                startCartListener(); // Start listening to the cart
            } else {
                userId = null;
                authStatusDisplay.textContent = "Signed out.";
                console.log("User signed out.");
                // Clean up listeners on sign out
                if (cartListenerUnsubscribe) cartListenerUnsubscribe();
                if (productsListenerUnsubscribe) productsListenerUnsubscribe();
                currentProductsMap = {};
                renderShop();
            }
        });
    }

    // --- Admin Status and Conditional Rendering ---

    /** Sets up a listener for the Admin configuration document. */
    function loadAdminStatusListener() {
        const adminDocRef = getAdminConfigDocRef();
        if (!adminDocRef || !userId) return;

        onSnapshot(adminDocRef, async (docSnapshot) => {
            if (!docSnapshot.exists()) {
                // If config doesn't exist, make the current user the initial admin.
                try {
                    await setDoc(adminDocRef, { adminUserId: userId });
                    isCurrentUserAdmin = true;
                    console.log("Admin config initialized. Current user is Admin.");
                } catch (e) {
                    console.error("Failed to initialize admin config:", e);
                }
            } else {
                // Check if the current user ID matches the stored admin ID
                const adminData = docSnapshot.data();
                isCurrentUserAdmin = (adminData && adminData.adminUserId === userId);
                console.log("Admin status check:", isCurrentUserAdmin ? "Admin" : "Standard User");
            }
            // Update UI on state change
            updateAdminAuthView();
        }, (error) => {
            console.error("Error listening to admin status:", error);
        });
    }

    /** Toggles the visibility of the Admin Panel vs. QR Scanner. */
    function updateAdminAuthView() {
        if (currentPage !== 'auth') return;

        if (isCurrentUserAdmin) {
            adminPanel.classList.remove('hidden');
            qrScannerContent.classList.add('hidden');
            authHeaderTitle.textContent = 'ADMIN PRODUCT MANAGER';
        } else {
            adminPanel.classList.add('hidden');
            qrScannerContent.classList.remove('hidden');
            authHeaderTitle.textContent = 'QR SCANNER / AUTH';
            // Start scanner only if it's visible
            startScanner();
        }
    }


    // --- Product Management (Admin/Shop) Functions ---

    /** Renders the shop view using data from Firestore. */
    function renderShop() {
        productGrid.innerHTML = '';
        const items = Object.values(currentProductsMap);
        
        if (!productsLoaded || items.length === 0) {
            shopLoadingMessage.classList.remove('hidden');
            productGrid.innerHTML = '';
            productGrid.appendChild(shopLoadingMessage);
            if (productsLoaded && items.length === 0) {
                 shopLoadingMessage.textContent = 'No products available right now!';
            } else if (!productsLoaded) {
                 shopLoadingMessage.textContent = 'Loading products...';
            }
            return;
        }

        shopLoadingMessage.classList.add('hidden');
        
        items.forEach(product => {
            const lineThrough = product.lineThroughPrice ? `<p class="text-xs text-gray-400 line-through mb-2">$${Number(product.lineThroughPrice).toFixed(2)}</p>` : `<p class="text-xs text-gray-400 mb-2 invisible"></p>`;
            const productHtml = `
                <div class="product-card bg-gray-900/50 p-2 shadow-2xl flex flex-col">
                    <div class="relative mb-2 rounded-lg overflow-hidden h-36">
                        <img src="${product.img}" onerror="this.onerror=null;this.src='https://placehold.co/400x400/312e81/ffffff?text=Image+Error';" alt="${product.name}" class="w-full h-full object-cover">
                        <button class="absolute top-2 right-2 text-white/70 hover:text-pink-400 transition">
                            <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-heart"><path d="M19 14c1.49-1.46 3-3.23 3-5.5A5.5 5.5 0 0 0 16.5 3c-1.76 0-3 .5-4.5 2-1.5-1.5-2.74-2-4.5-2A5.5 5.5 0 0 0 2 8.5c0 2.27 1.51 4.04 3 5.5l7 7Z"/></svg>
                        </button>
                    </div>
                    <div class="flex flex-col flex-grow">
                        <p class="text-sm font-medium text-gray-200 leading-tight flex-grow">${product.name}</p>
                        <div class="flex items-center text-xs my-1">
                            <span class="text-pink-400">★★★★★</span>
                            <span class="text-gray-500 ml-1">(0)</span>
                        </div>
                        <p class="text-lg font-bold text-white mt-1">$${Number(product.price).toFixed(2)}</p>
                        ${lineThrough}
                        <button onclick="addToCart('${product.docId}')" class="w-full py-2 bg-indigo-600 text-white text-sm font-semibold rounded-lg hover:bg-indigo-700 transition duration-200">
                            Add to cart
                        </button>
                    </div>
                </div>
            `;
            productGrid.insertAdjacentHTML('beforeend', productHtml);
        });
    }

    /** Renders the admin product list using data from Firestore. */
    function renderAdminProductList() {
        adminProductList.innerHTML = '';
        const items = Object.values(currentProductsMap);

        if (items.length === 0) {
            adminProductList.innerHTML = '<li class="text-gray-400">No products in the database.</li>';
            return;
        }

        items.forEach(product => {
            const lineThroughInfo = product.lineThroughPrice ? ` (Old: $${Number(product.lineThroughPrice).toFixed(2)})` : '';
            const listItem = `
                <li class="flex justify-between items-center p-3 bg-gray-800/70 rounded-lg border-l-4 border-indigo-400/70">
                    <div class="flex-grow min-w-0 pr-2">
                        <p class="text-white font-semibold truncate">${product.name}</p>
                        <p class="text-xs text-indigo-300">$${Number(product.price).toFixed(2)}${lineThroughInfo}</p>
                    </div>
                    <div class="flex space-x-2 flex-shrink-0">
                        <button onclick="editProduct('${product.docId}')" class="bg-blue-600 hover:bg-blue-700 text-white p-2 rounded-lg text-xs font-bold transition">Edit</button>
                        <button onclick="deleteProduct('${product.docId}')" class="bg-red-600 hover:bg-red-700 text-white p-2 rounded-lg text-xs font-bold transition">Delete</button>
                    </div>
                </li>
            `;
            adminProductList.insertAdjacentHTML('beforeend', listItem);
        });
    }

    /** Starts the real-time listener for public products. */
    function loadProductsListener() {
        if (productsListenerUnsubscribe) productsListenerUnsubscribe(); // Stop existing listener

        const productsRef = getProductsCollectionRef();
        if (!productsRef) return;

        productsListenerUnsubscribe = onSnapshot(productsRef, (snapshot) => {
            currentProductsMap = {};
            snapshot.forEach((doc) => {
                const product = doc.data();
                // Store product data using its Firestore document ID
                currentProductsMap[doc.id] = { docId: doc.id, ...product };
            });

            productsLoaded = true;
            renderShop();
            if (isCurrentUserAdmin) {
                renderAdminProductList();
            }

            // Also re-render the cart in case prices changed
            renderCart();

        }, (error) => {
            console.error("Error listening to products: ", error);
            shopLoadingMessage.textContent = 'Error loading products.';
        });
    }

    // --- Admin CRUD Functions ---
    // ... (handleProductFormSubmit, editProduct, resetForm, deleteProduct functions remain the same) ...

    /**
     * Handles product form submission (Add or Edit).
     * @param {Event} event - The form submission event.
     */
    async function handleProductFormSubmit(event) {
        event.preventDefault();

        if (!isCurrentUserAdmin) {
            alertMessage("Authorization failed. You are not the admin.");
            return;
        }

        const docId = productDocIdInput.value.trim();
        const name = productNameInput.value.trim();
        const price = parseFloat(productPriceInput.value);
        const img = productImgInput.value.trim();
        const badge = productBadgeInput.value.trim();
        const lineThroughPriceValue = productLineThroughPriceInput.value.trim();
        const lineThroughPrice = lineThroughPriceValue ? parseFloat(lineThroughPriceValue) : null;
        
        if (!name || isNaN(price) || price <= 0 || !img) {
            alertMessage("Please fill out all required fields (Name, Price, Image URL) correctly.");
            return;
        }

        const productData = {
            name: name,
            price: price,
            img: img,
            badge: badge || 'New',
            lineThroughPrice: lineThroughPrice
        };

        const productsRef = getProductsCollectionRef();
        if (!productsRef) return;

        try {
            if (docId) {
                // EDIT mode
                const docRef = doc(productsRef, docId);
                await updateDoc(docRef, productData);
                alertMessage(`Product "${name}" updated successfully!`);
            } else {
                // ADD mode
                await addDoc(productsRef, productData);
                alertMessage(`New product "${name}" added successfully!`);
            }
            resetForm();
        } catch (e) {
            console.error("Error saving product: ", e);
            alertMessage("Error: Could not save product. Check console for details.");
        }
    }

    /**
     * Pre-fills the form to edit an existing product.
     * @param {string} docId - The Firestore document ID of the product.
     */
    function editProduct(docId) {
        const product = currentProductsMap[docId];
        if (!product) {
            alertMessage("Product not found for editing.");
            return;
        }

        productDocIdInput.value = docId;
        productNameInput.value = product.name;
        productPriceInput.value = product.price;
        productImgInput.value = product.img;
        productBadgeInput.value = product.badge || '';
        productLineThroughPriceInput.value = product.lineThroughPrice || '';

        formTitle.textContent = `Edit Product: ${product.name}`;
        formButton.textContent = 'Update Product';

        // Scroll to the top of the content area to show the form
        mainContent.scrollTop = 0;
    }

    /** Resets the admin form to 'Add New Product' state. */
    function resetForm() {
        productForm.reset();
        productDocIdInput.value = '';
        formTitle.textContent = 'Add New Product';
        formButton.textContent = 'Add Product';
    }

    /**
     * Deletes a product from Firestore.
     * @param {string} docId - The Firestore document ID of the product.
     */
    async function deleteProduct(docId) {
        if (!isCurrentUserAdmin) {
            alertMessage("Authorization failed. You are not the admin.");
            return;
        }

        const product = currentProductsMap[docId];
        
        // --- Custom confirmation instead of window.confirm ---
        const confirmation = await confirmAction(`Are you sure you want to delete "${product ? product.name : 'this product'}"?`);
        
        if (!confirmation) return;
        // --- End custom confirmation ---

        const productsRef = getProductsCollectionRef();
        if (!productsRef) return;

        try {
            const docRef = doc(productsRef, docId);
            await deleteDoc(docRef);
            alertMessage(`Product deleted successfully.`);
            // Automatically re-renders via the onSnapshot listener
            resetForm(); 
        } catch (e) {
            console.error("Error deleting product: ", e);
            alertMessage("Error: Could not delete product.");
        }
    }

    // --- Cart Persistence Functions ---
    
    /**
     * Adds an item to the cart or increments its quantity.
     * @param {string} docId - The Firestore document ID of the product to add (from the products collection).
     */
    async function addToCart(docId) {
        const productData = currentProductsMap[docId];
        if (!productData) {
            alertMessage("Product data not found. Please try again later.");
            return;
        }

        const cartRef = getCartCollectionRef();
        if (!cartRef) return;

        // Find the cart item using the product docId
        const existingItem = Object.values(currentCartItems).find(item => item.data.docId === docId);

        try {
            if (existingItem) {
                // Item exists, update quantity
                const cartDocRef = doc(cartRef, existingItem.cartDocId);
                const newQuantity = existingItem.quantity + 1;
                await updateDoc(cartDocRef, {
                    quantity: newQuantity
                });
                alertMessage(`Added another ${productData.name}! Total: ${newQuantity}`);
            } else {
                // Item doesn't exist, add new document
                await addDoc(cartRef, {
                    productDocId: docId, // Store the reference to the product doc
                    quantity: 1,
                    timestamp: Date.now()
                });
                alertMessage(`${productData.name} added to cart!`);
            }
        } catch (e) {
            console.error("Error adding/updating document: ", e);
            alertMessage("Error: Could not update cart. Check console for details.");
        }
    }

    /**
     * Updates the quantity of an item or removes it if quantity is zero.
     * @param {string} cartDocId - The Firestore document ID of the cart item (from the user's cart collection).
     * @param {number} change - The amount to change the quantity by (+1 or -1).
     */
    async function updateCartItemQuantity(cartDocId, change) {
        const cartRef = getCartCollectionRef();
        if (!cartRef) return;

        const cartItem = currentCartItems[cartDocId];
        if (!cartItem) {
            console.error("Cart item not found:", cartDocId);
            return;
        }

        const newQuantity = cartItem.quantity + change;
        const docRef = doc(cartRef, cartDocId);

        try {
            if (newQuantity <= 0) {
                // Remove item if quantity is zero or less
                await deleteDoc(docRef);
                alertMessage(`${cartItem.data.name} removed from cart.`);
            } else {
                // Update quantity
                await updateDoc(docRef, {
                    quantity: newQuantity
                });
            }
        } catch (e) {
            console.error("Error updating/deleting document: ", e);
            alertMessage("Error: Could not update cart item quantity.");
        }
    }

    // *** NEW FUNCTION: Clear Cart ***
    /** Clears all items from the user's cart using a Firestore batch write. */
    async function clearCart() {
        if (Object.keys(currentCartItems).length === 0) {
            alertMessage("Your cart is already empty.");
            return;
        }

        const confirmation = await confirmAction("Are you sure you want to remove ALL items from your cart?");
        if (!confirmation) return;

        const cartRef = getCartCollectionRef();
        if (!cartRef) return;

        const batch = writeBatch(db);
        const itemIds = Object.keys(currentCartItems);

        try {
            // Add a delete operation for every item in the cart
            itemIds.forEach(cartDocId => {
                const docRef = doc(cartRef, cartDocId);
                batch.delete(docRef);
            });

            // Commit the batch of deletions
            await batch.commit();
            alertMessage(`Successfully cleared ${itemIds.length} items from your cart!`);

        } catch (e) {
            console.error("Error clearing cart with batch: ", e);
            alertMessage("Error: Could not clear cart. Please try again.");
        }
    }

    /**
     * Starts the real-time listener for the user's cart.
     */
    function startCartListener() {
        if (cartListenerUnsubscribe) {
            cartListenerUnsubscribe(); // Stop previous listener
        }

        const cartRef = getCartCollectionRef();
        if (!cartRef) return;

        const q = query(cartRef);

        cartListenerUnsubscribe = onSnapshot(q, (snapshot) => {
            currentCartItems = {};
            let total = 0;

            snapshot.forEach((doc) => {
                const item = doc.data();
                // Get product details from the local currentProductsMap using productDocId
                const productData = currentProductsMap[item.productDocId]; 

                if (productData) {
                    currentCartItems[doc.id] = {
                        cartDocId: doc.id,
                        quantity: item.quantity,
                        data: productData // Use the full product object
                    };
                    total += item.quantity * productData.price;
                } else {
                    console.warn(`Product reference ID ${item.productDocId} not found in product catalog.`);
                    // Optionally: delete orphaned cart item here
                }
            });

            renderCart(total);

        }, (error) => {
            console.error("Error listening to cart changes: ", error);
            alertMessage("Error loading cart data in real-time.");
        });
    }

    /**
     * Renders the cart items and updates the total/subtotal.
     * @param {number} total - The calculated total price of all items. (Optional, calculates if not provided)
     */
    function renderCart(total = null) {
        const items = Object.values(currentCartItems);
        cartItemsContainer.innerHTML = '';
        
        let calculatedTotal = 0;

        if (items.length === 0) {
            cartEmptyMessage.classList.remove('hidden');
            // *** UPDATED: Hide the clear cart button when empty ***
            clearCartBtn.classList.add('hidden');
        } else {
            cartEmptyMessage.classList.add('hidden');
            // *** UPDATED: Show the clear cart button when not empty ***
            clearCartBtn.classList.remove('hidden');
            items.forEach(item => {
                const subtotal = (item.quantity * item.data.price).toFixed(2);
                calculatedTotal += parseFloat(subtotal);

                const itemHtml = `
                    <div class="flex items-center bg-indigo-900/40 p-3 rounded-xl shadow-lg border border-indigo-700/50">
                        <img src="${item.data.img}" onerror="this.onerror=null;this.src='https://placehold.co/100x100/1e072b/ffffff?text=Product';" alt="${item.data.name}" class="w-16 h-16 rounded-lg object-cover mr-3 flex-shrink-0">
                        <div class="flex-grow">
                            <p class="text-white font-semibold leading-tight">${item.data.name}</p>
                            <p class="text-indigo-300 text-sm">$${Number(item.data.price).toFixed(2)} / item</p>
                        </div>
                        <div class="flex flex-col items-end flex-shrink-0">
                            <div class="flex items-center space-x-2 mb-2">
                                <button onclick="updateCartItemQuantity('${item.cartDocId}', -1)" class="qty-btn">-</button>
                                <span class="text-white font-bold text-lg">${item.quantity}</span>
                                <button onclick="updateCartItemQuantity('${item.cartDocId}', 1)" class="qty-btn">+</button>
                            </div>
                            <p class="text-pink-400 font-extrabold text-lg">$${subtotal}</p>
                        </div>
                    </div>
                `;
                cartItemsContainer.insertAdjacentHTML('beforeend', itemHtml);
            });
        }

        const finalTotal = (total !== null ? total : calculatedTotal).toFixed(2);
        cartSubtotal.textContent = `$${finalTotal}`;
        cartTotal.textContent = `$${finalTotal}`;
    }


    // --- QR Scanner Functions (unchanged logic) ---

    /** Callback for successful QR code scan. */
    function onScanSuccess(decodedText, decodedResult) {
        if (authResultDisplay) {
            authResultDisplay.innerHTML = `<p class="text-green-400 font-bold">SCAN SUCCESSFUL!</p><p class="text-sm break-all">Data: ${decodedText}</p>`;
        }
        stopScanner(); 
    }

    /** Callback for failed QR code scan (or continuous errors). */
    function onScanFailure(error) {
        // Log errors but avoid showing them to the user constantly
        // console.warn(`Code scan error = ${error}`);
    }

    /** Initializes and starts the QR scanner. */
    function startScanner() {
        if (isCurrentUserAdmin) return; // Do not start scanner if admin panel is showing

        if (typeof Html5QrcodeScanner === 'undefined') {
             authResultDisplay.textContent = "QR Scanner library not loaded. Cannot start scanner.";
             return;
        }

        authResultDisplay.textContent = "Scan Result: Waiting for QR Code...";

        if (!html5QrcodeScanner) {
            html5QrcodeScanner = new Html5QrcodeScanner(
                "reader",
                { fps: 10, qrbox: { width: 200, height: 200 } },
                /* verbose= */ false
            );
        }

        const readerElement = document.getElementById('reader');
        if (readerElement && readerElement.childElementCount === 0) {
             html5QrcodeScanner.render(onScanSuccess, onScanFailure);
        }
    }

    /** Stops the QR scanner and cleans up the DOM. */
    function stopScanner() {
        if (html5QrcodeScanner) {
            const readerElement = document.getElementById('reader');
            if (readerElement && readerElement.querySelector('video')) {
                 html5QrcodeScanner.stop().then(() => {
                    console.log("Scanner stopped gracefully.");
                    readerElement.innerHTML = ""; 
                 }).catch(err => {
                    console.warn("Scanner stop failed (camera might not have been active):", err);
                    readerElement.innerHTML = "";
                 });
            } else if (readerElement) {
                 readerElement.innerHTML = "";
            }
        }
    }


    // --- Utility Functions (Alert/Confirmation) ---

    /** Shows a custom message box instead of using alert() */
    function alertMessage(message) {
        messageText.textContent = message;
        messageBox.classList.add('flex');
        messageBox.classList.remove('hidden');
    }

    /** Hides the custom message box. */
    function hideMessage() {
        messageBox.classList.remove('flex');
        messageBox.classList.add('hidden');
    }

    /** Shows a custom confirmation dialog and returns a Promise that resolves to true/false. */
    function confirmAction(message) {
        return new Promise((resolve) => {
            confirmationText.textContent = message;
            confirmationBox.classList.add('flex');
            confirmationBox.classList.remove('hidden');
            
            resolveConfirmation = resolve;
        });
    }

    /** Event listeners for confirmation buttons */
    confirmYesBtn.onclick = () => {
        confirmationBox.classList.remove('flex');
        confirmationBox.classList.add('hidden');
        // Change text back to "Delete" for admin form
        if (confirmationText.textContent.includes("delete")) {
             confirmYesBtn.textContent = "Delete";
        } else {
             confirmYesBtn.textContent = "Confirm";
        }
        if (resolveConfirmation) resolveConfirmation(true);
    };

    confirmNoBtn.onclick = () => {
        confirmationBox.classList.remove('flex');
        confirmationBox.classList.add('hidden');
        // Change text back to "Delete" for admin form
        if (confirmationText.textContent.includes("delete")) {
             confirmYesBtn.textContent = "Delete";
        } else {
             confirmYesBtn.textContent = "Confirm";
        }
        if (resolveConfirmation) resolveConfirmation(false);
    };

    // --- Utility Functions (Navigation) ---

    /**
     * Handles navigation between the main views.
     * @param {string} targetPage - The ID suffix of the page to navigate to ('home', 'shop', 'cart', or 'auth').
     */
    function navigateTo(targetPage) {
        // Stop QR scanner if leaving the Auth page
        if (currentPage === 'auth' && targetPage !== 'auth') {
            stopScanner();
        }
        
        if (currentPage === targetPage) return;
        
        currentPage = targetPage;

        // Hide all views
        document.querySelectorAll('.page-view').forEach(view => {
            view.classList.add('hidden');
        });

        // Show the target view
        document.getElementById(`${targetPage}-view`).classList.remove('hidden');

        // Toggle the sticky mobile shop navigation
        const isShop = targetPage === 'shop';
        if (isShop && window.innerWidth <= 400) {
            mobileShopNav.classList.remove('hidden');
        } else {
            mobileShopNav.classList.add('hidden');
        }

        // Update active navigation button style
        navButtons.forEach(button => {
            button.classList.remove('active-nav', 'text-indigo-400');
            button.classList.add('text-gray-400');
        });

        const activeNavButton = document.getElementById(`nav-${targetPage}`);
        if (activeNavButton) {
            activeNavButton.classList.add('active-nav', 'text-indigo-400');
            activeNavButton.classList.remove('text-gray-400');
        }

        // Handle Auth/Admin view logic
        if (targetPage === 'auth') {
            updateAdminAuthView();
        }

        // Scroll to top when changing views
        mainContent.scrollTop = 0;
    }

    // --- Global Export (Allows HTML buttons to call these functions) ---
    window.alertMessage = alertMessage;
    window.hideMessage = hideMessage;
    window.navigateTo = navigateTo;
    window.addToCart = addToCart;
    window.updateCartItemQuantity = updateCartItemQuantity;
    // *** NEW: Export clearCart ***
    window.clearCart = clearCart;
    window.handleProductFormSubmit = handleProductFormSubmit;
    window.editProduct = editProduct;
    window.deleteProduct = deleteProduct;
    window.resetForm = resetForm;
    // Exporting confirmation functions for general use, though internal calls should use the promise
    window.confirmAction = confirmAction; 

    // --- Initial load setup ---
    window.onload = function() {
        initializeFirebase();
        navigateTo('home');
    };

    window.addEventListener('resize', () => {
        if (currentPage === 'shop' && window.innerWidth <= 400) {
            mobileShopNav.classList.remove('hidden');
        } else {
            mobileShopNav.classList.add('hidden');
        }
    });

</script>
</body>
</html>
