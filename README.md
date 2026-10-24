<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Pawan Mart - Aapka Apna Supermarket | 10-Min Delivery in Ranchi</title>
  
  <!-- Tailwind CSS CDN -->
  <script src="https://cdn.tailwindcss.com"></script>
  
  <!-- FontAwesome Icons -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
  
  <!-- Google Fonts: Plus Jakarta Sans & Outfit -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@400;500;600;700;800;900&family=Plus+Jakarta+Sans:wght@400;500;600;700;800&display=swap" rel="stylesheet">
  
  <script>
    tailwind.config = {
      theme: {
        extend: {
          colors: {
            brand: {
              yellow: '#FBBF24',
              orange: '#F97316',
              amber: '#D97706',
              green: '#059669',
              darkGreen: '#064E3B',
              navy: '#0F172A',
              lightGray: '#F8FAFC'
            }
          },
          fontFamily: {
            sans: ['"Plus Jakarta Sans"', 'sans-serif'],
            display: ['"Outfit"', 'sans-serif']
          }
        }
      }
    }
  </script>

  <style>
    .no-scrollbar::-webkit-scrollbar { display: none; }
    .no-scrollbar { -ms-overflow-style: none; scrollbar-width: none; }
    .badge-pulse { animation: pulseGlow 2s cubic-bezier(0.4, 0, 0.6, 1) infinite; }
    @keyframes pulseGlow {
      0%, 100% { opacity: 1; transform: scale(1); }
      50% { opacity: .88; transform: scale(1.05); }
    }
    .transition-drawer { transition: transform 0.3s cubic-bezier(0.16, 1, 0.3, 1); }
    input[type=number]::-webkit-inner-spin-button, 
    input[type=number]::-webkit-outer-spin-button { 
      -webkit-appearance: none; 
      margin: 0; 
    }
    input[type=number] {
      appearance: textfield;
      -moz-appearance: textfield;
    }
  </style>
</head>
<body class="bg-[#F9FAFB] text-slate-800 font-sans antialiased overflow-x-hidden selection:bg-amber-400 selection:text-slate-900">

  <!-- ================= TOP ANNOUNCEMENT BAR ================= -->
  <div class="bg-gradient-to-r from-amber-500 via-orange-500 to-amber-600 text-slate-950 font-medium text-xs sm:text-sm py-2 px-4 shadow-sm">
    <div class="max-w-7xl mx-auto flex items-center justify-between">
      <div class="flex items-center space-x-2 mx-auto sm:mx-0">
        <span class="bg-white text-orange-600 text-[10px] font-black px-2 py-0.5 rounded-full uppercase tracking-wider shadow-sm flex items-center gap-1">
          <i class="fa-solid fa-bolt text-amber-500"></i>
          10-Min Fast
        </span>
        <span class="text-white font-semibold">Fresh farm vegetables & daily groceries in Ranchi! Free delivery above ₹199.</span>
      </div>
      <div class="hidden sm:flex items-center space-x-5 text-white/95 text-xs font-semibold">
        <span class="flex items-center gap-1 text-white">
          <i class="fa-solid fa-location-dot text-amber-200"></i> Ranchi Only
        </span>
        <span class="text-white/40">|</span>
        <a href="mailto:p01hariprajapati@gmail.com" class="hover:text-white transition">
          <i class="fa-solid fa-envelope"></i> p01hariprajapati@gmail.com
        </a>
      </div>
    </div>
  </div>

  <!-- ================= MAIN HEADER / NAVBAR ================= -->
  <header class="sticky top-0 z-40 bg-white/95 backdrop-blur-md border-b border-slate-200/80 shadow-sm">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex items-center justify-between h-20 gap-3 md:gap-6">
        
        <!-- Logo & Location Badge -->
        <div class="flex items-center space-x-3 md:space-x-6 shrink-0">
          <a href="#" class="flex items-center gap-2 group">
            <div class="w-11 h-11 rounded-2xl bg-gradient-to-tr from-amber-500 via-orange-500 to-amber-400 flex items-center justify-center text-white shadow-md shadow-orange-500/20 group-hover:scale-105 transition font-display font-black text-2xl">
              P
            </div>
            <div class="flex flex-col">
              <span class="font-display font-extrabold text-2xl tracking-tight text-slate-900 leading-none">
                Pawan<span class="text-amber-500">Mart</span>
              </span>
              <span class="text-[10px] uppercase font-bold tracking-widest text-emerald-600 mt-0.5">Fresh Vegetables & Kirana • Ranchi</span>
            </div>
          </a>

          <div class="hidden lg:flex items-center gap-2 bg-emerald-50 border border-emerald-200 px-3.5 py-1.5 rounded-xl">
            <div class="w-7 h-7 rounded-lg bg-emerald-100 text-emerald-700 flex items-center justify-center shrink-0">
              <i class="fa-solid fa-location-dot text-xs"></i>
            </div>
            <div class="text-left">
              <div class="text-[9px] text-emerald-700 font-bold uppercase tracking-wider">Service Hub</div>
              <div class="text-xs font-bold text-slate-900">Ranchi, Jharkhand</div>
            </div>
          </div>
        </div>

        <!-- Center: Interactive Search Bar -->
        <div class="flex-1 max-w-xl mx-2 md:mx-4 relative">
          <div class="relative">
            <input 
              type="text" 
              id="searchInput" 
              oninput="handleSearch(this.value)" 
              placeholder='Search: "Potato", "Tomato", "Atta", "Rice", "Onion", "Milk", "Maggi", "Oil"...' 
              class="w-full pl-11 pr-10 py-3 rounded-2xl bg-slate-100/90 border border-transparent focus:border-amber-400 focus:bg-white focus:outline-none focus:ring-4 focus:ring-amber-400/20 text-sm transition-all text-slate-800 placeholder-slate-400 font-medium"
            >
            <div class="absolute inset-y-0 left-0 pl-4 flex items-center pointer-events-none text-slate-400">
              <i class="fa-solid fa-magnifying-glass text-sm"></i>
            </div>
            <button id="clearSearchBtn" onclick="clearSearch()" class="hidden absolute inset-y-0 right-0 pr-3.5 flex items-center text-slate-400 hover:text-slate-600">
              <i class="fa-solid fa-xmark"></i>
            </button>
          </div>
        </div>

        <!-- Right: Cart Action -->
        <div class="flex items-center space-x-2 sm:space-x-3 shrink-0">
          <button 
            onclick="toggleCart(true)" 
            class="relative flex items-center gap-2.5 px-4 py-2.5 bg-emerald-600 hover:bg-emerald-700 active:scale-95 text-white font-bold text-xs sm:text-sm rounded-2xl shadow-lg shadow-emerald-600/25 transition duration-150"
          >
            <div class="relative">
              <i class="fa-solid fa-cart-shopping text-base"></i>
              <span id="cartCountBadge" class="absolute -top-2.5 -right-3 bg-amber-400 text-slate-900 font-black text-[10px] w-5 h-5 rounded-full flex items-center justify-center border-2 border-white shadow">
                0
              </span>
            </div>
            <div class="hidden sm:flex flex-col text-left leading-tight">
              <span class="text-[10px] text-emerald-100 font-medium">My Cart</span>
              <span id="headerCartTotal" class="font-extrabold">₹0</span>
            </div>
          </button>
        </div>
      </div>
    </div>
  </header>

  <!-- ================= HERO SECTION ================= -->
  <section class="relative bg-gradient-to-b from-amber-50 via-white to-slate-50 pt-8 pb-14 border-b border-slate-200/60 overflow-hidden">
    <div class="absolute -top-24 -right-24 w-96 h-96 bg-amber-200/40 rounded-full blur-3xl pointer-events-none"></div>
    <div class="absolute bottom-0 -left-20 w-80 h-80 bg-emerald-200/30 rounded-full blur-3xl pointer-events-none"></div>

    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10">
      <div class="grid grid-cols-1 lg:grid-cols-12 gap-8 items-center">
        
        <div class="lg:col-span-7 space-y-6 text-center lg:text-left">
          <div class="inline-flex items-center gap-2 bg-white px-4 py-2 rounded-full shadow-sm border border-amber-200 text-xs font-bold text-slate-700">
            <span class="flex h-2.5 w-2.5 rounded-full bg-emerald-500 animate-pulse"></span>
            <span>All placed orders arrive at <strong>Pawan Mart</strong></span>
          </div>

          <h1 class="font-display text-4xl sm:text-5xl lg:text-6xl font-extrabold text-slate-900 tracking-tight leading-[1.15]">
            Fresh Vegetables & Groceries <br class="hidden sm:inline">
            <span class="text-transparent bg-clip-text bg-gradient-to-r from-amber-500 via-orange-500 to-amber-600">Pawan Mart Ranchi</span>
          </h1>

          <p class="text-slate-600 text-base sm:text-lg max-w-2xl mx-auto lg:mx-0 font-normal leading-relaxed">
            Order fresh green vegetables, Atta, Basmati Rice, Dals, Pure Desi Ghee, Spices, Dairy, and Snacks delivered in <strong>10 to 15 minutes</strong> across all neighborhoods in <strong>Ranchi</strong>.
          </p>

          <div class="flex flex-col sm:flex-row items-center justify-center lg:justify-start gap-3 sm:gap-4 pt-2">
            <a href="#products-section" class="w-full sm:w-auto px-8 py-4 bg-gradient-to-r from-amber-500 to-orange-500 hover:from-amber-600 hover:to-orange-600 text-slate-950 font-bold rounded-2xl shadow-lg shadow-orange-500/25 flex items-center justify-center gap-2 transition transform active:scale-98">
              <span>Shop Vegetables & Items</span>
              <i class="fa-solid fa-arrow-right"></i>
            </a>
            <div class="inline-flex items-center gap-2 px-5 py-4 bg-emerald-100 text-emerald-900 font-bold text-xs rounded-2xl border border-emerald-300">
              <i class="fa-solid fa-carrot text-emerald-700 text-base"></i>
              <span>Farm Fresh Everyday</span>
            </div>
          </div>
        </div>

        <div class="lg:col-span-5">
          <div class="relative bg-white rounded-3xl p-6 shadow-2xl border border-slate-100 overflow-hidden group">
            <div class="flex items-center justify-between mb-4">
              <span class="bg-emerald-600 text-white font-extrabold text-xs px-3 py-1 rounded-full uppercase tracking-wider flex items-center gap-1">
                <i class="fa-solid fa-leaf"></i> Fresh Farm Basket
              </span>
              <span class="text-xs font-semibold text-slate-400">Morning Pluck</span>
            </div>

            <div class="relative rounded-2xl overflow-hidden aspect-[4/3] mb-4 bg-slate-100">
              <img 
                src="https://images.unsplash.com/photo-1610348725531-843dff563e2c?auto=format&fit=crop&w=800&q=80" 
                alt="Fresh Farm Vegetables" 
                class="w-full h-full object-cover group-hover:scale-105 transition duration-500"
              />
              <div class="absolute bottom-3 left-3 bg-white/95 backdrop-blur-md px-3 py-1.5 rounded-xl shadow-md flex items-center gap-2">
                <span class="text-emerald-600 font-bold text-xs"><i class="fa-solid fa-bolt"></i> 10-15 mins dispatch</span>
                <span class="text-slate-300">•</span>
                <span class="text-xs text-slate-600 font-medium">Ranchi Sabzi Mandi</span>
              </div>
            </div>

            <div class="space-y-3">
              <div class="flex items-baseline justify-between">
                <div>
                  <h3 class="font-display font-bold text-lg text-slate-900">Ranchi Daily Sabzi Combo</h3>
                  <p class="text-xs text-slate-500">Fresh Potatoes (2kg), Onions (1kg) & Tomatoes (1kg)</p>
                </div>
                <div class="text-right">
                  <span class="text-slate-400 text-xs line-through block">₹185</span>
                  <span class="font-bold text-xl text-emerald-700">₹139</span>
                </div>
              </div>
              <button onclick="addVegComboToCart()" class="w-full py-3 bg-slate-900 hover:bg-slate-800 text-white font-bold text-sm rounded-xl transition flex items-center justify-center gap-2">
                <i class="fa-solid fa-plus text-amber-400"></i>
                <span>Add Sabzi Combo to Cart</span>
              </button>
            </div>
          </div>
        </div>

      </div>
    </div>
  </section>

  <!-- ================= CATEGORY QUICK NAV ================= -->
  <section class="py-6 bg-white border-b border-slate-100 sticky top-20 z-30 shadow-sm">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex items-center justify-between mb-3">
        <h2 class="font-display font-bold text-base sm:text-lg text-slate-900 flex items-center gap-2">
          <span>Categories</span>
          <span id="activeFilterBadge" class="text-xs font-semibold px-2.5 py-0.5 rounded-full bg-amber-100 text-amber-800 hidden"></span>
        </h2>
        <button onclick="filterCategory('All')" class="text-xs text-amber-600 font-bold hover:underline">Show All Products</button>
      </div>

      <div class="flex items-center space-x-3 overflow-x-auto pb-2 no-scrollbar" id="categoryContainer"></div>
    </div>
  </section>

  <!-- ================= PRODUCTS SECTION ================= -->
  <section id="products-section" class="py-12 bg-slate-50 min-h-[500px]">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      
      <div class="flex flex-col sm:flex-row sm:items-center justify-between gap-4 mb-8">
        <div>
          <h2 class="font-display font-extrabold text-2xl sm:text-3xl text-slate-900 tracking-tight" id="productGridTitle">
            Fresh Vegetables & Daily Groceries
          </h2>
          <p class="text-slate-500 text-sm mt-1" id="productCountSubtitle">
            Select desired quantity for each item and add to your Ranchi basket.
          </p>
        </div>
        
        <div class="flex items-center gap-2 self-start sm:self-auto">
          <span class="text-xs font-semibold text-slate-500">Sort:</span>
          <select id="sortSelect" onchange="applySorting(this.value)" class="text-xs font-bold bg-white border border-slate-200 rounded-xl px-3 py-2 text-slate-700 focus:outline-none focus:ring-2 focus:ring-amber-400">
            <option value="popular">Popularity</option>
            <option value="price-low">Price: Low to High</option>
            <option value="price-high">Price: High to Low</option>
            <option value="discount">Biggest Discount</option>
          </select>
        </div>
      </div>

      <!-- Products Grid -->
      <div id="productsGrid" class="grid grid-cols-2 sm:grid-cols-3 md:grid-cols-4 lg:grid-cols-5 gap-4 sm:gap-6"></div>

      <div id="noResults" class="hidden py-16 text-center">
        <div class="w-20 h-20 mx-auto bg-amber-50 rounded-full flex items-center justify-center text-3xl text-amber-500 mb-4">
          <i class="fa-solid fa-magnifying-glass"></i>
        </div>
        <h3 class="font-bold text-lg text-slate-800">No products found</h3>
        <p class="text-slate-500 text-sm max-w-sm mx-auto mt-1 mb-4">We couldn't find items matching your search. Try searching "Potato", "Tomato", "Atta", "Rice", or click below.</p>
        <button onclick="resetFilters()" class="px-5 py-2.5 bg-amber-500 hover:bg-amber-600 text-slate-900 font-bold text-xs rounded-xl transition">
          Reset Filter & Show All Items
        </button>
      </div>

    </div>
  </section>

  <!-- ================= RANCHI COVERAGE BANNER ================= -->
  <section class="py-12 bg-amber-500 text-slate-950">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center space-y-3">
      <span class="bg-slate-900 text-amber-400 font-black text-xs px-3 py-1 rounded-full uppercase tracking-wider">Local Hub Network</span>
      <h2 class="font-display font-black text-2xl sm:text-3xl text-slate-950">Exclusively Active In Ranchi</h2>
      <p class="text-sm font-semibold max-w-2xl mx-auto text-slate-900">
        Doorstep delivery in Tupudana, Hatia, Harmu, Argora, Lalpur, Doranda, Kanke, Bariatu, Ratu Road, and Hinoo.
      </p>
    </div>
  </section>

  <!-- ================= FOOTER ================= -->
  <footer class="bg-slate-900 text-slate-400 text-xs pt-16 pb-12 border-t border-slate-800">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="grid grid-cols-1 md:grid-cols-3 gap-8 mb-12">
        <div class="space-y-4">
          <div class="flex items-center gap-2">
            <div class="w-9 h-9 rounded-xl bg-amber-500 flex items-center justify-center text-slate-950 font-black font-display text-lg">P</div>
            <span class="font-display font-extrabold text-2xl text-white">Pawan<span class="text-amber-500">mart</span></span>
          </div>
          <p class="text-slate-400 max-w-sm leading-relaxed">
            Fast, reliable, hyper-convenient grocery and vegetable delivery service built exclusively for the city of Ranchi.
          </p>
        </div>

        <div>
          <h4 class="font-display font-bold text-white text-sm mb-4">Contact & Support</h4>
          <div class="space-y-2 text-xs text-slate-300">
            <p class="flex items-center gap-2">
              <i class="fa-solid fa-location-dot text-amber-400 w-4"></i>
              <span>Ranchi, Jharkhand, India</span>
            </p>
            <p class="flex items-center gap-2">
              <i class="fa-solid fa-envelope text-amber-400 w-4"></i>
              <a href="mailto:p01hariprajapati@gmail.com" class="hover:text-amber-400 font-mono">p01hariprajapati@gmail.com</a>
            </p>
          </div>
        </div>

        <div>
          <h4 class="font-display font-bold text-white text-sm mb-4">Ranchi Neighborhoods Served</h4>
          <p class="text-slate-400 leading-relaxed text-xs">
            Tupudana • Hatia • Harmu • Argora • Lalpur • Doranda • Kanke Road • Bariatu • Ratu Road • Hinoo
          </p>
        </div>
      </div>

      <div class="border-t border-slate-800 pt-8 flex flex-col sm:flex-row items-center justify-between text-slate-500 gap-4">
        <div>© <span id="currentYear"></span> Pawan Mart Ranchi. All rights reserved.</div>
        <div class="flex items-center space-x-6 text-xs">
          <span>Direct Orders Forwarded To: <strong class="text-amber-400 font-mono">PAWAN MART</strong></span>
        </div>
      </div>
    </div>
  </footer>

  <!-- ================= CART SLIDE-OVER DRAWER ================= -->
  <div id="cartDrawerBackdrop" class="fixed inset-0 bg-slate-900/60 backdrop-blur-sm z-50 hidden opacity-0 transition-opacity duration-300" onclick="toggleCart(false)"></div>
  
  <aside id="cartDrawer" class="fixed top-0 right-0 h-full w-full max-w-md bg-white shadow-2xl z-50 transform translate-x-full transition-drawer flex flex-col">
    <div class="p-5 border-b border-slate-100 flex items-center justify-between bg-slate-50">
      <div class="flex items-center gap-2.5">
        <div class="w-8 h-8 rounded-lg bg-emerald-100 text-emerald-700 flex items-center justify-center">
          <i class="fa-solid fa-cart-shopping text-sm"></i>
        </div>
        <div>
          <h3 class="font-display font-bold text-slate-900 text-base">Your Cart</h3>
          <p class="text-[11px] text-slate-500">Delivering in 10 mins across Ranchi</p>
        </div>
      </div>
      <button onclick="toggleCart(false)" class="p-2 text-slate-400 hover:text-slate-700 rounded-xl hover:bg-slate-200/60 transition">
        <i class="fa-solid fa-xmark text-lg"></i>
      </button>
    </div>

    <!-- Free Delivery Progress Bar -->
    <div class="bg-amber-50 px-5 py-3 border-b border-amber-100">
      <div class="flex justify-between text-xs font-semibold text-slate-800 mb-1">
        <span id="freeDeliveryStatus">Add ₹199 for Free Delivery</span>
        <span id="freeDeliveryBadge" class="text-amber-700 font-bold">Standard ₹25</span>
      </div>
      <div class="w-full bg-amber-200/60 rounded-full h-2 overflow-hidden">
        <div id="freeDeliveryProgress" class="bg-gradient-to-r from-amber-500 to-emerald-500 h-2 rounded-full transition-all duration-300" style="width: 0%"></div>
      </div>
    </div>

    <!-- Cart Item List -->
    <div id="cartItemList" class="flex-1 overflow-y-auto p-5 space-y-4"></div>

    <!-- Empty Cart Screen -->
    <div id="emptyCartView" class="hidden flex-1 flex flex-col items-center justify-center p-8 text-center">
      <div class="w-20 h-20 rounded-full bg-slate-100 flex items-center justify-center text-3xl text-slate-400 mb-3">
        <i class="fa-solid fa-basket-shopping"></i>
      </div>
      <h4 class="font-display font-bold text-lg text-slate-800">Your basket is empty</h4>
      <p class="text-xs text-slate-500 max-w-xs mt-1 mb-6">Explore our fresh farm vegetables, staples and daily essentials at lowest rates.</p>
      <button onclick="toggleCart(false)" class="px-6 py-2.5 bg-amber-500 hover:bg-amber-600 font-bold text-xs rounded-xl text-slate-900 transition">
        Start Shopping
      </button>
    </div>

    <!-- Cart Footer & Bill Summary -->
    <div id="cartFooterSummary" class="border-t border-slate-100 p-5 bg-slate-50 space-y-4">
      <div class="flex gap-2">
        <input 
          type="text" 
          id="couponInput" 
          placeholder="Coupon (Try: PAWAN100)" 
          class="flex-1 px-3 py-2 bg-white border border-slate-200 rounded-xl text-xs uppercase font-bold tracking-wider text-slate-700 focus:outline-none focus:ring-2 focus:ring-amber-400"
        >
        <button onclick="applyCoupon()" class="px-4 py-2 bg-slate-900 hover:bg-slate-800 text-white font-bold text-xs rounded-xl transition">
          Apply
        </button>
      </div>
      <div id="couponFeedback" class="text-[11px] font-semibold hidden"></div>

      <div class="space-y-1.5 text-xs text-slate-600">
        <div class="flex justify-between">
          <span>Items Total</span>
          <span id="billSubtotal" class="font-semibold text-slate-800">₹0</span>
        </div>
        <div class="flex justify-between">
          <span>Handling & Delivery Fee</span>
          <span id="billDeliveryFee" class="font-semibold text-slate-800">₹25</span>
        </div>
        <div id="discountRow" class="flex justify-between text-emerald-600 hidden font-semibold">
          <span>Coupon Discount</span>
          <span id="billDiscount">- ₹0</span>
        </div>
        <div class="border-t border-slate-200 pt-2 flex justify-between text-sm font-bold text-slate-900">
          <span>To Pay</span>
          <span id="billGrandTotal" class="text-base text-emerald-700">₹0</span>
        </div>
      </div>

      <button onclick="openCheckoutModal()" class="w-full py-3.5 bg-gradient-to-r from-emerald-600 to-emerald-700 hover:from-emerald-700 hover:to-emerald-800 active:scale-[0.99] text-white font-bold text-sm rounded-2xl shadow-lg shadow-emerald-600/30 flex items-center justify-between px-5 transition">
        <span>Proceed to Checkout</span>
        <span id="checkoutBtnTotal" class="font-extrabold bg-emerald-800/60 px-2.5 py-1 rounded-lg text-xs">₹0</span>
      </button>

      <p class="text-[10px] text-center text-slate-400">
        <i class="fa-solid fa-shield-halved text-emerald-600 mr-1"></i> Cash on Delivery & UPI at Doorstep in Ranchi
      </p>
    </div>
  </aside>

  <!-- ================= CHECKOUT MODAL ================= -->
  <div id="checkoutModal" class="fixed inset-0 z-50 hidden flex items-center justify-center p-4">
    <div class="fixed inset-0 bg-slate-900/60 backdrop-blur-sm" onclick="closeModal('checkoutModal')"></div>
    <div class="relative bg-white rounded-3xl max-w-md w-full p-6 sm:p-7 shadow-2xl z-10 border border-slate-100 max-h-[92vh] overflow-y-auto">
      
      <div class="flex justify-between items-start mb-4">
        <div>
          <span class="text-[10px] font-bold uppercase tracking-wider text-emerald-700 bg-emerald-100 px-2 py-0.5 rounded-full flex items-center gap-1 w-fit">
            <i class="fa-solid fa-bolt"></i> 10-Min Ranchi Delivery
          </span>
          <h3 class="font-display font-extrabold text-xl text-slate-900 mt-1">Delivery Address & Details</h3>
          <p class="text-xs text-slate-500">Order will be dispatched directly to your location.</p>
        </div>
        <button onclick="closeModal('checkoutModal')" class="p-1.5 text-slate-400 hover:text-slate-700 rounded-lg">
          <i class="fa-solid fa-xmark text-lg"></i>
        </button>
      </div>

      <form id="orderCheckoutForm" onsubmit="handlePlaceOrder(event)" class="space-y-3.5">
        <div>
          <label class="block text-xs font-bold text-slate-700 mb-1">Customer Full Name *</label>
          <div class="relative">
            <input required type="text" id="custName" placeholder="e.g. Rahul Kumar" class="w-full pl-9 pr-3.5 py-2.5 bg-slate-50 border border-slate-200 rounded-xl text-xs font-medium focus:ring-2 focus:ring-emerald-500 focus:outline-none">
            <div class="absolute inset-y-0 left-0 pl-3 flex items-center pointer-events-none text-slate-400">
              <i class="fa-solid fa-user text-xs"></i>
            </div>
          </div>
        </div>

        <div>
          <label class="block text-xs font-bold text-slate-700 mb-1">Mobile Number (For Delivery Call) *</label>
          <div class="relative">
            <input required type="tel" id="custPhone" pattern="[0-9]{10}" placeholder="10-digit mobile number" class="w-full pl-9 pr-3.5 py-2.5 bg-slate-50 border border-slate-200 rounded-xl text-xs font-medium focus:ring-2 focus:ring-emerald-500 focus:outline-none">
            <div class="absolute inset-y-0 left-0 pl-3 flex items-center pointer-events-none text-slate-400">
              <i class="fa-solid fa-phone text-xs"></i>
            </div>
          </div>
        </div>

        <div class="grid grid-cols-2 gap-3">
          <div>
            <label class="block text-xs font-bold text-slate-700 mb-1">Delivery City</label>
            <input readonly type="text" id="custCity" value="Ranchi, Jharkhand" class="w-full px-3 py-2.5 bg-gray-100 border border-slate-200 rounded-xl text-xs font-bold text-emerald-800 outline-none">
          </div>
          <div>
            <label class="block text-xs font-bold text-slate-700 mb-1">Ranchi Area / Colony *</label>
            <select id="custArea" required class="w-full px-3 py-2.5 bg-slate-50 border border-slate-200 rounded-xl text-xs font-medium focus:ring-2 focus:ring-emerald-500 focus:outline-none">
              <option value="Tupudana">Tupudana</option>
              <option value="Harmu">Harmu</option>
              <option value="Hatia">Hatia</option>
              <option value="Lalpur">Lalpur</option>
              <option value="Doranda">Doranda</option>
              <option value="Argora">Argora</option>
              <option value="Ratu Road">Ratu Road</option>
              <option value="Kanke Road">Kanke Road</option>
              <option value="Bariatu">Bariatu</option>
              <option value="Hinoo">Hinoo</option>
              <option value="Other Ranchi Area">Other Ranchi Area</option>
            </select>
          </div>
        </div>

        <div>
          <label class="block text-xs font-bold text-slate-700 mb-1">Complete House / Flat & Landmark Address *</label>
          <textarea required id="custAddress" rows="2" placeholder="e.g. Flat 204, Shanti Niwas, Near Harmu Chowk, Ranchi" class="w-full px-3.5 py-2 bg-slate-50 border border-slate-200 rounded-xl text-xs font-medium focus:ring-2 focus:ring-emerald-500 focus:outline-none"></textarea>
        </div>

        <div>
          <label class="block text-xs font-bold text-slate-700 mb-1">Select Payment Method</label>
          <div class="space-y-2 text-xs">
            <label class="flex items-center gap-3 p-3 border border-slate-200 rounded-xl cursor-pointer hover:bg-slate-50 transition">
              <input type="radio" name="paymentMethod" value="Cash on Delivery (COD)" checked class="text-emerald-600">
              <div>
                <span class="font-bold text-slate-800 block">Cash on Delivery (COD)</span>
                <span class="text-[11px] text-slate-500">Pay cash directly to the delivery rider in Ranchi</span>
              </div>
            </label>
            <label class="flex items-center gap-3 p-3 border border-slate-200 rounded-xl cursor-pointer hover:bg-slate-50 transition">
              <input type="radio" name="paymentMethod" value="UPI / QR on Delivery" class="text-emerald-600">
              <div>
                <span class="font-bold text-slate-800 block">UPI / QR on Delivery</span>
                <span class="text-[11px] text-slate-500">Scan rider's GPay / PhonePe QR code</span>
              </div>
            </label>
          </div>
        </div>

        <div class="bg-emerald-50 p-3 rounded-xl border border-emerald-100 flex items-center justify-between text-xs">
          <div>
            <div class="font-bold text-emerald-950">Grand Total Payable:</div>
            <div class="text-[10px] text-emerald-700">10-min packing & delivery included</div>
          </div>
          <div id="checkoutFinalAmount" class="font-black text-lg text-emerald-800">₹0</div>
        </div>

        <button type="submit" id="submitOrderBtn" class="w-full py-3.5 bg-emerald-600 hover:bg-emerald-700 text-white font-bold text-sm rounded-xl transition shadow-lg shadow-emerald-600/30 flex items-center justify-center gap-2">
          <i class="fa-solid fa-check"></i>
          <span>Confirm & Place Order</span>
        </button>

        <p class="text-[10px] text-center text-slate-400">Order details will land in <strong>p01hariprajapati@gmail.com</strong></p>
      </form>
    </div>
  </div>

  <!-- ================= SUCCESS ORDER MODAL ================= -->
  <div id="orderSuccessModal" class="fixed inset-0 z-50 hidden flex items-center justify-center p-4">
    <div class="fixed inset-0 bg-slate-900/60 backdrop-blur-sm"></div>
    <div class="relative bg-white rounded-3xl max-w-sm w-full p-7 shadow-2xl z-10 text-center space-y-4">
      <div class="w-16 h-16 bg-emerald-100 text-emerald-600 rounded-full flex items-center justify-center text-3xl mx-auto badge-pulse">
        <i class="fa-solid fa-check"></i>
      </div>
      <h3 class="font-display font-extrabold text-2xl text-slate-900">Order Confirmed!</h3>
      <p class="text-xs text-slate-600 leading-relaxed">
        Your order has been placed and forwarded to <strong>p01hariprajapati@gmail.com</strong>. The nearest Pawan Mart hub is preparing your order.
      </p>
      
      <div class="bg-amber-50 p-3.5 rounded-2xl border border-amber-200 text-left text-xs space-y-1.5">
        <div class="flex justify-between">
          <span class="text-slate-500">Order ID:</span>
          <span class="font-mono font-bold text-slate-900" id="confirmedOrderId">#PM-94821</span>
        </div>
        <div class="flex justify-between">
          <span class="text-slate-500">City:</span>
          <span class="font-bold text-slate-800">Ranchi, Jharkhand</span>
        </div>
        <div class="flex justify-between">
          <span class="text-slate-500">Estimated Delivery:</span>
          <span class="font-bold text-emerald-700">10-15 Minutes</span>
        </div>
        <div class="flex justify-between border-t border-amber-200/60 pt-1">
          <span class="text-slate-500">Customer:</span>
          <span class="font-semibold text-slate-800" id="confirmedCustName">-</span>
        </div>
      </div>

      <button onclick="closeModal('orderSuccessModal')" class="w-full py-3 bg-slate-900 hover:bg-slate-800 text-white font-bold text-xs rounded-xl transition">
        Continue Shopping
      </button>
    </div>
  </div>

  <!-- ================= TOAST CONTAINER ================= -->
  <div id="toastContainer" class="fixed bottom-6 left-1/2 transform -translate-x-1/2 z-50 flex flex-col items-center space-y-2 pointer-events-none"></div>

  <!-- ================= LOGIC & SCRIPT ================= -->
  <script>
    /* ==========================================================================
       FORM & STORE CONFIGURATION
       ========================================================================== */
    const FORMSUBMIT_TOKEN = "7d105d48f17b60d3af0326484b294e45";
    const STORE_OWNER_EMAIL = "p01hariprajapati@gmail.com";

    /* ==========================================================================
       EXPANDED CATALOG: VEGETABLES & POPULAR GROCERIES
       ========================================================================== */
    const CATEGORIES = [
      { id: 'All', name: 'All Products', icon: 'fa-basket-shopping' },
      { id: 'Fresh Vegetables', name: 'Fresh Vegetables', icon: 'fa-carrot' },
      { id: 'Atta & Flours', name: 'Atta & Flours', icon: 'fa-wheat-awn' },
      { id: 'Rice & Grains', name: 'Rice & Grains', icon: 'fa-bowl-rice' },
      { id: 'Dals & Pulses', name: 'Dals & Pulses', icon: 'fa-seedling' },
      { id: 'Edible Oils & Ghee', name: 'Oils & Ghee', icon: 'fa-bottle-droplet' },
      { id: 'Dairy & Bread', name: 'Dairy & Bread', icon: 'fa-cheese' },
      { id: 'Spices & Sugar', name: 'Spices & Sugar', icon: 'fa-pepper-hot' },
      { id: 'Snacks & Biscuits', name: 'Snacks & Biscuits', icon: 'fa-cookie-bite' },
      { id: 'Beverages & Tea', name: 'Beverages & Tea', icon: 'fa-mug-hot' },
      { id: 'Cleaning & Needs', name: 'Cleaning & Needs', icon: 'fa-broom' },
      { id: 'Personal Care', name: 'Personal Care', icon: 'fa-pump-soap' }
    ];

    const PRODUCTS = [
      // ================= FRESH FARM VEGETABLES =================
      { id: 101, title: 'Fresh Desi Potato (Aloo)', category: 'Fresh Vegetables', weight: '1 kg', mrp: 35, price: 26, image: 'https://images.unsplash.com/photo-1518977676601-b53f82aba655?auto=format&fit=crop&w=600&q=80', rating: 4.9 },
      { id: 102, title: 'Fresh Nashik Red Onion (Pyaz)', category: 'Fresh Vegetables', weight: '1 kg', mrp: 45, price: 34, image: 'https://images.unsplash.com/photo-1618512496248-a07fe83aa8cb?auto=format&fit=crop&w=600&q=80', rating: 4.8 },
      { id: 103, title: 'Fresh Hybrid Juicy Red Tomatoes (Tamatar)', category: 'Fresh Vegetables', weight: '1 kg', mrp: 40, price: 28, image: 'https://images.unsplash.com/photo-1592924357228-91a4daadcfea?auto=format&fit=crop&w=600&q=80', rating: 4.9 },
      { id: 104, title: 'Fresh Cauliflower (Phool Gobi)', category: 'Fresh Vegetables', weight: '1 pc (500-700g)', mrp: 45, price: 32, image: 'https://images.unsplash.com/photo-1568584711075-3d021a7c3ca3?auto=format&fit=crop&w=600&q=80', rating: 4.8 },
      { id: 105, title: 'Fresh Green Capsicum (Shimla Mirch)', category: 'Fresh Vegetables', weight: '500 g', mrp: 50, price: 38, image: 'https://images.unsplash.com/photo-1563565375-f3fdfdbefa83?auto=format&fit=crop&w=600&q=80', rating: 4.7 },
      { id: 106, title: 'Fresh Tender Lady Finger (Bhindi)', category: 'Fresh Vegetables', weight: '500 g', mrp: 40, price: 30, image: 'https://images.unsplash.com/photo-1629853488219-c6e3b0e35560?auto=format&fit=crop&w=600&q=80', rating: 4.8 },
      { id: 107, title: 'Fresh Ginger Root (Adrak)', category: 'Fresh Vegetables', weight: '250 g', mrp: 40, price: 28, image: 'https://images.unsplash.com/photo-1615485290382-441e4d049cb5?auto=format&fit=crop&w=600&q=80', rating: 4.9 },
      { id: 108, title: 'Fresh Spicy Green Chillies (Hari Mirch)', category: 'Fresh Vegetables', weight: '200 g', mrp: 25, price: 16, image: 'https://images.unsplash.com/photo-1588252303782-cb80119abd6d?auto=format&fit=crop&w=600&q=80', rating: 4.9 },
      { id: 109, title: 'Fresh Garlic Bulbs (Lahsun)', category: 'Fresh Vegetables', weight: '250 g', mrp: 65, price: 48, image: 'https://images.unsplash.com/photo-1540148426945-6cf22a6b2383?auto=format&fit=crop&w=600&q=80', rating: 4.8 },
      { id: 110, title: 'Fresh Crunchy Orange Carrots (Gajar)', category: 'Fresh Vegetables', weight: '500 g', mrp: 35, price: 24, image: 'https://images.unsplash.com/photo-1598170845058-32b9d6a5da37?auto=format&fit=crop&w=600&q=80', rating: 4.7 },
      { id: 111, title: 'Fresh Green Spinach Bunch (Palak)', category: 'Fresh Vegetables', weight: '250 g Bunch', mrp: 25, price: 18, image: 'https://images.unsplash.com/photo-1576045057995-568f588f82fb?auto=format&fit=crop&w=600&q=80', rating: 4.9 },
      { id: 112, title: 'Fresh Sweet Green Peas (Hari Matar)', category: 'Fresh Vegetables', weight: '500 g', mrp: 60, price: 42, image: 'https://images.unsplash.com/photo-1587735243615-c03f25aaff15?auto=format&fit=crop&w=600&q=80', rating: 4.8 },
      { id: 113, title: 'Fresh Lemon / Nimbu (Pack of 4)', category: 'Fresh Vegetables', weight: '4 pcs', mrp: 25, price: 18, image: 'https://images.unsplash.com/photo-1533089860892-a7c6f0a88666?auto=format&fit=crop&w=600&q=80', rating: 4.8 },

      // ================= ATTA & FLOURS =================
      { id: 1, title: 'Aashirvaad Superior MP Sharbati Atta', category: 'Atta & Flours', weight: '5 kg', mrp: 295, price: 245, image: 'https://images.unsplash.com/photo-1509440159596-0249088772ff?auto=format&fit=crop&w=600&q=80', rating: 4.9 },
      { id: 2, title: 'Fortune Chakki Fresh Pure Wheat Atta', category: 'Atta & Flours', weight: '10 kg', mrp: 480, price: 420, image: 'https://images.unsplash.com/photo-1574323347407-f5e1ad6d020b?auto=format&fit=crop&w=600&q=80', rating: 4.8 },
      { id: 3, title: 'Rajdhani Fine Besan (Gram Flour)', category: 'Atta & Flours', weight: '500 g', mrp: 65, price: 54, image: 'https://images.unsplash.com/photo-1627485937980-221c88ac04f9?auto=format&fit=crop&w=600&q=80', rating: 4.7 },
      { id: 4, title: 'Pilsbury Refined Maida Flour', category: 'Atta & Flours', weight: '1 kg', mrp: 55, price: 46, image: 'https://images.unsplash.com/photo-1586201375761-83865001e31c?auto=format&fit=crop&w=600&q=80', rating: 4.6 },
      { id: 5, title: 'Rajdhani Sooji / Rawa', category: 'Atta & Flours', weight: '500 g', mrp: 42, price: 35, image: 'https://images.unsplash.com/photo-1607623814075-e51df1bdc82f?auto=format&fit=crop&w=600&q=80', rating: 4.8 },

      // ================= RICE & GRAINS =================
      { id: 6, title: 'India Gate Basmati Rice Feast Rozzana', category: 'Rice & Grains', weight: '5 kg', mrp: 499, price: 399, image: 'https://images.unsplash.com/photo-1586201375761-83865001e31c?auto=format&fit=crop&w=600&q=80', rating: 4.9 },
      { id: 7, title: 'Daawat Super Long Grain Basmati Rice', category: 'Rice & Grains', weight: '1 kg', mrp: 165, price: 135, image: 'https://images.unsplash.com/photo-1536304993881-ff6e9eefa2a6?auto=format&fit=crop&w=600&q=80', rating: 4.8 },
      { id: 8, title: 'Premium Sona Masoori Raw Rice', category: 'Rice & Grains', weight: '5 kg', mrp: 350, price: 295, image: 'https://images.unsplash.com/photo-1516684732162-798a0062be99?auto=format&fit=crop&w=600&q=80', rating: 4.7 },
      { id: 9, title: 'Quaker Rolled Oats 100% Wholegrain', category: 'Rice & Grains', weight: '1 kg', mrp: 215, price: 180, image: 'https://images.unsplash.com/photo-1584776296944-ab6fb57b0bdd?auto=format&fit=crop&w=600&q=80', rating: 4.8 },
      { id: 10, title: 'Kelloggs Corn Flakes Real Almond Honey', category: 'Rice & Grains', weight: '300 g', mrp: 190, price: 165, image: 'https://images.unsplash.com/photo-1521483451569-e33803c0330c?auto=format&fit=crop&w=600&q=80', rating: 4.7 },

      // ================= DALS & PULSES =================
      { id: 11, title: 'Tata Sampann Unpolished Toor / Arhar Dal', category: 'Dals & Pulses', weight: '1 kg', mrp: 185, price: 158, image: 'https://images.unsplash.com/photo-1585994192701-f1a505c817ea?auto=format&fit=crop&w=600&q=80', rating: 4.9 },
      { id: 12, title: 'Tata Sampann Yellow Moong Dal Dhuli', category: 'Dals & Pulses', weight: '1 kg', mrp: 160, price: 138, image: 'https://images.unsplash.com/photo-1546833999-b9f581a1996d?auto=format&fit=crop&w=600&q=80', rating: 4.8 },
      { id: 13, title: 'Tata Sampann Red Masoor Dal (Split)', category: 'Dals & Pulses', weight: '1 kg', mrp: 130, price: 110, image: 'https://images.unsplash.com/photo-1515543237350-b3eea1ec8082?auto=format&fit=crop&w=600&q=80', rating: 4.7 },
      { id: 14, title: 'Tata Sampann Chana Dal High Protein', category: 'Dals & Pulses', weight: '1 kg', mrp: 125, price: 105, image: 'https://images.unsplash.com/photo-1596040033229-a9821ebd058d?auto=format&fit=crop&w=600&q=80', rating: 4.8 },
      { id: 15, title: 'Premium Kabuli Chana (Big White Chickpeas)', category: 'Dals & Pulses', weight: '1 kg', mrp: 180, price: 152, image: 'https://images.unsplash.com/photo-1515543237350-b3eea1ec8082?auto=format&fit=crop&w=600&q=80', rating: 4.7 },
      { id: 16, title: 'Rajma Chitra (Himalayan Kidney Beans)', category: 'Dals & Pulses', weight: '1 kg', mrp: 175, price: 148, image: 'https://images.unsplash.com/photo-1546833999-b9f581a1996d?auto=format&fit=crop&w=600&q=80', rating: 4.8 },

      // ================= EDIBLE OILS & GHEE =================
      { id: 17, title: 'Fortune Sunlite Refined Sunflower Oil', category: 'Edible Oils & Ghee', weight: '1 L Pouch', mrp: 165, price: 132, image: 'https://images.unsplash.com/photo-1474979266404-7eaacbcd87c5?auto=format&fit=crop&w=600&q=80', rating: 4.8 },
      { id: 18, title: 'Fortune Kachi Ghani Mustard Oil (Sarson)', category: 'Edible Oils & Ghee', weight: '1 L Bottle', mrp: 180, price: 150, image: 'https://images.unsplash.com/photo-1620916566398-39f1143ab7be?auto=format&fit=crop&w=600&q=80', rating: 4.9 },
      { id: 19, title: 'Amul Pure Desi Ghee Tin Pack', category: 'Edible Oils & Ghee', weight: '1 Litre', mrp: 650, price: 585, image: 'https://images.unsplash.com/photo-1589985270826-4b7bb135bc9d?auto=format&fit=crop&w=600&q=80', rating: 4.9 },
      { id: 20, title: 'Saffola Gold Pro Healthy Heart Edible Oil', category: 'Edible Oils & Ghee', weight: '1 L Pouch', mrp: 195, price: 168, image: 'https://images.unsplash.com/photo-1474979266404-7eaacbcd87c5?auto=format&fit=crop&w=600&q=80', rating: 4.8 },

      // ================= DAIRY & BREAD =================
      { id: 21, title: 'Amul Taaza Fresh Toned Milk', category: 'Dairy & Bread', weight: '500 ml', mrp: 28, price: 27, image: 'https://images.unsplash.com/photo-1550583724-b2692b85b150?auto=format&fit=crop&w=600&q=80', rating: 4.9 },
      { id: 22, title: 'Amul Salted Table Butter', category: 'Dairy & Bread', weight: '500 g', mrp: 275, price: 260, image: 'https://images.unsplash.com/photo-1589985270826-4b7bb135bc9d?auto=format&fit=crop&w=600&q=80', rating: 4.9 },
      { id: 23, title: 'Amul Malai Fresh Paneer Cube Pack', category: 'Dairy & Bread', weight: '200 g', mrp: 95, price: 88, image: 'https://images.unsplash.com/photo-1631452180519-c014fe946bc7?auto=format&fit=crop&w=600&q=80', rating: 4.9 },
      { id: 24, title: 'Amul Masti Dahi Fresh Curd Pouch', category: 'Dairy & Bread', weight: '400 g', mrp: 35, price: 32, image: 'https://images.unsplash.com/photo-1571212515416-fef01fc43637?auto=format&fit=crop&w=600&q=80', rating: 4.8 },
      { id: 25, title: 'Britannia 100% Whole Wheat Brown Bread', category: 'Dairy & Bread', weight: '400 g', mrp: 50, price: 45, image: 'https://images.unsplash.com/photo-1509440159596-0249088772ff?auto=format&fit=crop&w=600&q=80', rating: 4.7 },

      // ================= SPICES, SALT & SUGAR =================
      { id: 26, title: 'Tata Salt Vacuum Evaporated Iodised Salt', category: 'Spices & Sugar', weight: '1 kg', mrp: 28, price: 25, image: 'https://images.unsplash.com/photo-1518110925495-5fe2fda0442c?auto=format&fit=crop&w=600&q=80', rating: 4.8 },
      { id: 27, title: 'Madhur Pure Refined Crystal Sugar', category: 'Spices & Sugar', weight: '1 kg', mrp: 55, price: 48, image: 'https://images.unsplash.com/photo-1622484216801-6b2a47738bc3?auto=format&fit=crop&w=600&q=80', rating: 4.8 },
      { id: 28, title: 'Catch Turmeric / Haldi Powder', category: 'Spices & Sugar', weight: '200 g', mrp: 65, price: 52, image: 'https://images.unsplash.com/photo-1615485290382-441e4d049cb5?auto=format&fit=crop&w=600&q=80', rating: 4.8 },
      { id: 29, title: 'MDH Deggi Mirch Red Chilli Powder', category: 'Spices & Sugar', weight: '100 g', mrp: 88, price: 78, image: 'https://images.unsplash.com/photo-1596040033229-a9821ebd058d?auto=format&fit=crop&w=600&q=80', rating: 4.9 },
      { id: 30, title: 'Catch Coriander / Dhaniya Powder', category: 'Spices & Sugar', weight: '200 g', mrp: 70, price: 58, image: 'https://images.unsplash.com/photo-1596040033229-a9821ebd058d?auto=format&fit=crop&w=600&q=80', rating: 4.7 },
      { id: 31, title: 'Everest Royal Garam Masala Blend', category: 'Spices & Sugar', weight: '100 g', mrp: 92, price: 82, image: 'https://images.unsplash.com/photo-1596040033229-a9821ebd058d?auto=format&fit=crop&w=600&q=80', rating: 4.8 },
      { id: 32, title: 'Whole Jeera / Cumin Seeds Fresh', category: 'Spices & Sugar', weight: '100 g', mrp: 75, price: 59, image: 'https://images.unsplash.com/photo-1596040033229-a9821ebd058d?auto=format&fit=crop&w=600&q=80', rating: 4.8 },

      // ================= SNACKS & BISCUITS =================
      { id: 33, title: 'Maggi 2-Minute Masala Instant Noodles', category: 'Snacks & Biscuits', weight: '280 g (Pack of 4)', mrp: 60, price: 52, image: 'https://images.unsplash.com/photo-1612927601601-6638404737ce?auto=format&fit=crop&w=600&q=80', rating: 4.9 },
      { id: 34, title: 'Parle-G Gold Glucose Biscuits Mega Pack', category: 'Snacks & Biscuits', weight: '1 kg', mrp: 120, price: 105, image: 'https://images.unsplash.com/photo-1558961363-fa8fdf82db35?auto=format&fit=crop&w=600&q=80', rating: 4.8 },
      { id: 35, title: 'Britannia Good Day Cashew Cookies', category: 'Snacks & Biscuits', weight: '600 g', mrp: 150, price: 125, image: 'https://images.unsplash.com/photo-1499636136210-6f4ee915583e?auto=format&fit=crop&w=600&q=80', rating: 4.7 },
      { id: 36, title: 'Lays India Magic Masala Chips Party Pack', category: 'Snacks & Biscuits', weight: '115 g', mrp: 50, price: 44, image: 'https://images.unsplash.com/photo-1566478989037-eec170784d0b?auto=format&fit=crop&w=600&q=80', rating: 4.8 },
      { id: 37, title: 'Haldiram Nagpur Aloo Bhujia Namkeen', category: 'Snacks & Biscuits', weight: '400 g', mrp: 130, price: 110, image: 'https://images.unsplash.com/photo-1599490659213-e2b9527bd087?auto=format&fit=crop&w=600&q=80', rating: 4.9 },

      // ================= BEVERAGES & TEA =================
      { id: 38, title: 'Tata Tea Gold Leaf Tea with Long Leaves', category: 'Beverages & Tea', weight: '500 g', mrp: 330, price: 285, image: 'https://images.unsplash.com/photo-1576092768241-dec231879fc3?auto=format&fit=crop&w=600&q=80', rating: 4.9 },
      { id: 39, title: 'Nescafe Classic Instant Coffee Jar', category: 'Beverages & Tea', weight: '100 g', mrp: 320, price: 285, image: 'https://images.unsplash.com/photo-1514432324607-a09d9b4aefdd?auto=format&fit=crop&w=600&q=80', rating: 4.8 },
      { id: 40, title: 'Coca-Cola Soft Drink Chilled Bottle', category: 'Beverages & Tea', weight: '750 ml', mrp: 45, price: 39, image: 'https://images.unsplash.com/photo-1622483767028-3f66f32aef97?auto=format&fit=crop&w=600&q=80', rating: 4.7 },
      { id: 41, title: 'Real Fruit Power Mixed Fruit Juice', category: 'Beverages & Tea', weight: '1 Litre', mrp: 130, price: 108, image: 'https://images.unsplash.com/photo-1613478223719-2ab802602423?auto=format&fit=crop&w=600&q=80', rating: 4.8 },

      // ================= CLEANING & HOUSEHOLD =================
      { id: 42, title: 'Surf Excel Easy Wash Detergent Powder', category: 'Cleaning & Needs', weight: '1 kg', mrp: 155, price: 138, image: 'https://images.unsplash.com/photo-1583947215259-38e31be8751f?auto=format&fit=crop&w=600&q=80', rating: 4.7 },
      { id: 43, title: 'Vim Dishwash Gel Lemon Anti-Germ', category: 'Cleaning & Needs', weight: '500 ml', mrp: 125, price: 105, image: 'https://images.unsplash.com/photo-1585421514738-01798e348b17?auto=format&fit=crop&w=600&q=80', rating: 4.8 },
      { id: 44, title: 'Colin Glass & Surface Cleaner Spray', category: 'Cleaning & Needs', weight: '500 ml', mrp: 110, price: 95, image: 'https://images.unsplash.com/photo-1585421514738-01798e348b17?auto=format&fit=crop&w=600&q=80', rating: 4.6 },
      { id: 45, title: 'Harpic Power Plus Disinfectant Toilet Cleaner', category: 'Cleaning & Needs', weight: '1 Litre', mrp: 215, price: 185, image: 'https://images.unsplash.com/photo-1584813470613-5b1c1cad3d69?auto=format&fit=crop&w=600&q=80', rating: 4.8 },

      // ================= PERSONAL CARE =================
      { id: 46, title: 'Dettol Original Germ Protection Soap (Buy 3 Get 1)', category: 'Personal Care', weight: '125 g x 4', mrp: 210, price: 175, image: 'https://images.unsplash.com/photo-1607006314175-43a992525164?auto=format&fit=crop&w=600&q=80', rating: 4.8 },
      { id: 47, title: 'Colgate Strong Teeth Calcium Dental Cream', category: 'Personal Care', weight: '200 g (Pack of 2)', mrp: 180, price: 155, image: 'https://images.unsplash.com/photo-1559599101-f09722fb4948?auto=format&fit=crop&w=600&q=80', rating: 4.8 },
      { id: 48, title: 'Head & Shoulders Anti-Dandruff Smooth Shampoo', category: 'Personal Care', weight: '340 ml', mrp: 350, price: 295, image: 'https://images.unsplash.com/photo-1535585209827-a15fcdbc4c2d?auto=format&fit=crop&w=600&q=80', rating: 4.7 }
    ];

    /* ==========================================================================
       APP STATE
       ========================================================================== */
    let cart = [];
    let currentCategory = 'All';
    let searchQuery = '';
    let currentSort = 'popular';
    let appliedCoupon = null;
    let productInputQtys = {};

    /* ==========================================================================
       INITIALIZE
       ========================================================================== */
    window.addEventListener('DOMContentLoaded', () => {
      document.getElementById('currentYear').innerText = new Date().getFullYear();
      renderCategories();
      renderProducts();
      updateCartUI();
    });

    /* ==========================================================================
       CATEGORIES & NAVIGATION
       ========================================================================== */
    function renderCategories() {
      const container = document.getElementById('categoryContainer');
      container.innerHTML = CATEGORIES.map(cat => {
        const isActive = cat.id === currentCategory;
        const activeClass = isActive 
          ? 'bg-amber-500 text-slate-950 font-bold border-amber-500 shadow-sm' 
          : 'bg-white hover:bg-slate-50 text-slate-700 font-semibold border-slate-200';
        
        return `
          <button 
            onclick="filterCategory('${cat.id}')" 
            class="flex items-center gap-2 px-4 py-2.5 rounded-2xl border text-xs whitespace-nowrap transition transform active:scale-95 shrink-0 ${activeClass}"
          >
            <i class="fa-solid ${cat.icon}"></i>
            <span>${cat.name}</span>
          </button>
        `;
      }).join('');
    }

    function filterCategory(catId) {
      currentCategory = catId;
      renderCategories();
      
      const badge = document.getElementById('activeFilterBadge');
      if (catId !== 'All') {
        badge.innerText = catId;
        badge.classList.remove('hidden');
        document.getElementById('productGridTitle').innerText = `${catId} in Ranchi`;
      } else {
        badge.classList.add('hidden');
        document.getElementById('productGridTitle').innerText = 'Fresh Vegetables & Daily Groceries';
      }
      renderProducts();
    }

    /* ==========================================================================
       LIVE SEARCH
       ========================================================================== */
    function handleSearch(query) {
      searchQuery = query.trim().toLowerCase();
      const clearBtn = document.getElementById('clearSearchBtn');
      
      if (searchQuery.length > 0) {
        clearBtn.classList.remove('hidden');
        const section = document.getElementById('products-section');
        const offset = 90;
        const bodyRect = document.body.getBoundingClientRect().top;
        const elementRect = section.getBoundingClientRect().top;
        const elementPosition = elementRect - bodyRect;
        const offsetPosition = elementPosition - offset;

        window.scrollTo({
          top: offsetPosition,
          behavior: 'smooth'
        });
      } else {
        clearBtn.classList.add('hidden');
      }
      renderProducts();
    }

    function clearSearch() {
      document.getElementById('searchInput').value = '';
      searchQuery = '';
      document.getElementById('clearSearchBtn').classList.add('hidden');
      renderProducts();
    }

    function applySorting(sortMode) {
      currentSort = sortMode;
      renderProducts();
    }

    function resetFilters() {
      currentCategory = 'All';
      searchQuery = '';
      document.getElementById('searchInput').value = '';
      document.getElementById('clearSearchBtn').classList.add('hidden');
      renderCategories();
      renderProducts();
    }

    function getFilteredProducts() {
      return PRODUCTS.filter(p => {
        const matchesCat = (currentCategory === 'All') || (p.category === currentCategory);
        const matchesQuery = !searchQuery || 
          p.title.toLowerCase().includes(searchQuery) || 
          p.category.toLowerCase().includes(searchQuery) ||
          p.weight.toLowerCase().includes(searchQuery);
        return matchesCat && matchesQuery;
      }).sort((a, b) => {
        if (currentSort === 'price-low') return a.price - b.price;
        if (currentSort === 'price-high') return b.price - a.price;
        if (currentSort === 'discount') {
          return ((b.mrp - b.price) / b.mrp) - ((a.mrp - a.price) / a.mrp);
        }
        return b.rating - a.rating;
      });
    }

    /* ==========================================================================
       PRE-ADD QUANTITY CONTROLS
       ========================================================================== */
    function changeInputQty(productId, delta) {
      const current = productInputQtys[productId] || 1;
      const next = Math.max(1, Math.min(99, current + delta));
      productInputQtys[productId] = next;
      const inputEl = document.getElementById(`qtyInput_${productId}`);
      if (inputEl) inputEl.value = next;
    }

    function setDirectInputQty(productId, val) {
      let num = parseInt(val, 10);
      if (isNaN(num) || num < 1) num = 1;
      if (num > 99) num = 99;
      productInputQtys[productId] = num;
      const inputEl = document.getElementById(`qtyInput_${productId}`);
      if (inputEl) inputEl.value = num;
    }

    /* ==========================================================================
       RENDER PRODUCTS
       ========================================================================== */
    function renderProducts() {
      const filtered = getFilteredProducts();
      const grid = document.getElementById('productsGrid');
      const noResults = document.getElementById('noResults');
      const subtitle = document.getElementById('productCountSubtitle');

      if (searchQuery) {
        subtitle.innerHTML = `Found <strong class="text-amber-600">${filtered.length}</strong> items matching "<em>${searchQuery}</em>"`;
      } else {
        subtitle.innerText = `Showing ${filtered.length} fresh items available in Ranchi.`;
      }

      if (filtered.length === 0) {
        grid.innerHTML = '';
        noResults.classList.remove('hidden');
        return;
      }

      noResults.classList.add('hidden');
      grid.innerHTML = filtered.map(item => {
        const cartItem = cart.find(ci => ci.product.id === item.id);
        const cartQty = cartItem ? cartItem.quantity : 0;
        const discountPercent = Math.round(((item.mrp - item.price) / item.mrp) * 100);
        const preAddQty = productInputQtys[item.id] || 1;

        return `
          <div class="bg-white rounded-3xl p-3 sm:p-4 border border-slate-100 shadow-sm hover:shadow-xl transition-all duration-300 flex flex-col justify-between group relative">
            
            <div class="absolute top-3 left-3 z-10">
              <span class="bg-amber-400 text-slate-900 text-[10px] font-black px-2 py-0.5 rounded-lg shadow-sm">
                ${discountPercent}% OFF
              </span>
            </div>

            <div class="w-full aspect-square rounded-2xl bg-slate-50 overflow-hidden mb-3 relative flex items-center justify-center">
              <img 
                src="${item.image}" 
                alt="${item.title}" 
                class="w-full h-full object-cover group-hover:scale-105 transition duration-300"
                loading="lazy"
                onerror="this.src='https://placehold.co/400x400/f8fafc/334155?text=${encodeURIComponent(item.title)}'"
              />
              <div class="absolute bottom-1.5 right-1.5 bg-white/90 backdrop-blur-sm px-1.5 py-0.5 rounded-md text-[10px] font-bold text-slate-700 flex items-center gap-0.5">
                <i class="fa-solid fa-star text-amber-500 text-[9px]"></i> ${item.rating}
              </div>
            </div>

            <div class="flex-1 mb-2">
              <span class="text-[10px] uppercase font-bold tracking-wider text-slate-400 block">${item.category}</span>
              <h3 class="font-bold text-xs sm:text-sm text-slate-900 line-clamp-2 mt-0.5 leading-snug group-hover:text-amber-600 transition" title="${item.title}">
                ${item.title}
              </h3>
              <p class="text-xs text-slate-500 font-medium mt-1">${item.weight}</p>
            </div>

            <!-- Price & Quantity Selector Container -->
            <div class="pt-2 border-t border-slate-100 flex flex-col gap-2.5">
              <div class="flex items-baseline justify-between">
                <div>
                  <span class="text-[11px] text-slate-400 line-through">₹${item.mrp}</span>
                  <span class="font-extrabold text-sm sm:text-base text-slate-900 ml-1">₹${item.price}</span>
                </div>
                ${cartQty > 0 ? `<span class="text-[10px] font-bold text-emerald-700 bg-emerald-50 px-2 py-0.5 rounded-full">In Cart: ${cartQty}</span>` : ''}
              </div>

              <!-- Interactive Add-On & Quantity Section -->
              <div>
                ${cartQty === 0 ? `
                  <div class="flex items-center gap-1.5 w-full">
                    <div class="flex items-center bg-slate-100 border border-slate-200 rounded-xl overflow-hidden h-9 px-1">
                      <button 
                        type="button" 
                        onclick="changeInputQty(${item.id}, -1)" 
                        class="w-6 h-full flex items-center justify-center text-slate-600 hover:text-slate-900 text-xs font-bold active:scale-90"
                      >-</button>
                      <input 
                        type="number" 
                        id="qtyInput_${item.id}" 
                        value="${preAddQty}" 
                        min="1" 
                        max="99" 
                        onchange="setDirectInputQty(${item.id}, this.value)"
                        class="w-7 text-center bg-transparent text-xs font-black text-slate-800 outline-none"
                      />
                      <button 
                        type="button" 
                        onclick="changeInputQty(${item.id}, 1)" 
                        class="w-6 h-full flex items-center justify-center text-slate-600 hover:text-slate-900 text-xs font-bold active:scale-90"
                      >+</button>
                    </div>

                    <button 
                      onclick="addCustomQtyToCart(${item.id})" 
                      class="flex-1 h-9 bg-emerald-600 hover:bg-emerald-700 text-white font-extrabold text-xs rounded-xl transition flex items-center justify-center gap-1 shadow-sm active:scale-95"
                    >
                      <span>ADD</span>
                      <i class="fa-solid fa-plus text-[10px]"></i>
                    </button>
                  </div>
                ` : `
                  <div class="flex items-center justify-between bg-emerald-600 text-white rounded-xl overflow-hidden shadow-sm h-9 px-2">
                    <button onclick="updateCartItemQty(${item.id}, -1)" class="w-8 h-full flex items-center justify-center hover:bg-emerald-700 font-bold text-sm transition active:scale-90">-</button>
                    <div class="flex items-center gap-1">
                      <span class="text-xs font-black min-w-[20px] text-center font-mono">${cartQty}</span>
                      <span class="text-[10px] text-emerald-200 font-medium">added</span>
                    </div>
                    <button onclick="updateCartItemQty(${item.id}, 1)" class="w-8 h-full flex items-center justify-center hover:bg-emerald-700 font-bold text-sm transition active:scale-90">+</button>
                  </div>
                `}
              </div>

            </div>
          </div>
        `;
      }).join('');
    }

    /* ==========================================================================
       CART LOGIC
       ========================================================================== */
    function addCustomQtyToCart(productId) {
      const prod = PRODUCTS.find(p => p.id === productId);
      if (!prod) return;

      const qtyToAdd = productInputQtys[productId] || 1;
      const existing = cart.find(ci => ci.product.id === productId);

      if (existing) {
        existing.quantity += qtyToAdd;
      } else {
        cart.push({ product: prod, quantity: qtyToAdd });
      }

      showToast(`Added ${qtyToAdd}x "${prod.title.slice(0, 18)}..." to cart`);
      productInputQtys[productId] = 1;
      updateCartUI();
      renderProducts();
    }

    function addVegComboToCart() {
      // Add Potatoes, Onions, Tomatoes
      [101, 102, 103].forEach(id => {
        const p = PRODUCTS.find(prod => prod.id === id);
        if (p) {
          const item = cart.find(ci => ci.product.id === id);
          if (item) item.quantity += 1;
          else cart.push({ product: p, quantity: 1 });
        }
      });
      showToast('Daily Sabzi Combo added to Cart!');
      updateCartUI();
      renderProducts();
      toggleCart(true);
    }

    function updateCartItemQty(productId, delta) {
      const idx = cart.findIndex(ci => ci.product.id === productId);
      if (idx === -1) return;

      cart[idx].quantity += delta;
      if (cart[idx].quantity <= 0) {
        cart.splice(idx, 1);
      }

      updateCartUI();
      renderProducts();
    }

    function setCartItemDirectQty(productId, val) {
      const idx = cart.findIndex(ci => ci.product.id === productId);
      if (idx === -1) return;

      let num = parseInt(val, 10);
      if (isNaN(num) || num <= 0) {
        cart.splice(idx, 1);
      } else {
        cart[idx].quantity = Math.min(99, num);
      }

      updateCartUI();
      renderProducts();
    }

    function updateCartUI() {
      const totalCount = cart.reduce((sum, item) => sum + item.quantity, 0);
      const subtotal = cart.reduce((sum, item) => sum + (item.product.price * item.quantity), 0);
      
      const deliveryFee = subtotal >= 199 || subtotal === 0 ? 0 : 25;
      let discount = appliedCoupon ? appliedCoupon.discount : 0;
      const grandTotal = Math.max(0, subtotal + deliveryFee - discount);

      document.getElementById('cartCountBadge').innerText = totalCount;
      document.getElementById('headerCartTotal').innerText = `₹${subtotal}`;

      const cartItemList = document.getElementById('cartItemList');
      const emptyView = document.getElementById('emptyCartView');
      const footerSummary = document.getElementById('cartFooterSummary');

      if (totalCount === 0) {
        cartItemList.innerHTML = '';
        emptyView.classList.remove('hidden');
        footerSummary.classList.add('hidden');
      } else {
        emptyView.classList.add('hidden');
        footerSummary.classList.remove('hidden');

        const freeDeliveryStatus = document.getElementById('freeDeliveryStatus');
        const freeDeliveryBadge = document.getElementById('freeDeliveryBadge');
        const freeDeliveryProgress = document.getElementById('freeDeliveryProgress');

        if (subtotal >= 199) {
          freeDeliveryStatus.innerHTML = '<span class="text-emerald-700 font-bold"><i class="fa-solid fa-circle-check"></i> Free Ranchi 10-Min Delivery Unlocked!</span>';
          freeDeliveryBadge.innerText = 'FREE';
          freeDeliveryBadge.className = 'text-emerald-700 font-extrabold';
          freeDeliveryProgress.style.width = '100%';
        } else {
          const remaining = 199 - subtotal;
          const percent = Math.min(100, Math.round((subtotal / 199) * 100));
          freeDeliveryStatus.innerText = `Add ₹${remaining} more for Free Delivery`;
          freeDeliveryBadge.innerText = 'Standard ₹25';
          freeDeliveryBadge.className = 'text-amber-700 font-bold';
          freeDeliveryProgress.style.width = `${percent}%`;
        }

        cartItemList.innerHTML = cart.map(item => `
          <div class="flex items-center justify-between gap-3 bg-slate-50 p-3 rounded-2xl border border-slate-100">
            <img src="${item.product.image}" class="w-14 h-14 rounded-xl object-cover bg-white shrink-0 border border-slate-200" alt="${item.product.title}">
            <div class="flex-1 min-w-0">
              <h4 class="font-bold text-xs text-slate-800 truncate">${item.product.title}</h4>
              <p class="text-[11px] text-slate-400">${item.product.weight}</p>
              <div class="text-xs font-black text-slate-900 mt-0.5">₹${item.product.price} <span class="text-[10px] font-normal text-slate-400">× ${item.quantity}</span></div>
            </div>
            
            <div class="flex items-center bg-white border border-slate-200 rounded-xl overflow-hidden shadow-xs h-8">
              <button onclick="updateCartItemQty(${item.product.id}, -1)" class="px-2.5 h-full text-slate-600 hover:bg-slate-100 text-xs font-bold">-</button>
              <input 
                type="number" 
                value="${item.quantity}" 
                min="1" 
                max="99" 
                onchange="setCartItemDirectQty(${item.product.id}, this.value)"
                class="w-7 text-center bg-transparent text-xs font-black text-slate-800 outline-none"
              />
              <button onclick="updateCartItemQty(${item.product.id}, 1)" class="px-2.5 h-full text-slate-600 hover:bg-slate-100 text-xs font-bold">+</button>
            </div>
          </div>
        `).join('');

        document.getElementById('billSubtotal').innerText = `₹${subtotal}`;
        document.getElementById('billDeliveryFee').innerText = deliveryFee === 0 ? 'FREE' : `₹${deliveryFee}`;
        
        const discRow = document.getElementById('discountRow');
        if (discount > 0) {
          discRow.classList.remove('hidden');
          document.getElementById('billDiscount').innerText = `- ₹${discount}`;
        } else {
          discRow.classList.add('hidden');
        }

        document.getElementById('billGrandTotal').innerText = `₹${grandTotal}`;
        document.getElementById('checkoutBtnTotal').innerText = `₹${grandTotal}`;
        document.getElementById('checkoutFinalAmount').innerText = `₹${grandTotal}`;
      }
    }

    function toggleCart(isOpen) {
      const backdrop = document.getElementById('cartDrawerBackdrop');
      const drawer = document.getElementById('cartDrawer');

      if (isOpen) {
        backdrop.classList.remove('hidden');
        setTimeout(() => backdrop.classList.remove('opacity-0'), 10);
        drawer.classList.remove('translate-x-full');
        document.body.classList.add('overflow-hidden');
      } else {
        backdrop.classList.add('opacity-0');
        drawer.classList.add('translate-x-full');
        setTimeout(() => backdrop.classList.add('hidden'), 300);
        document.body.classList.remove('overflow-hidden');
      }
    }

    function applyCoupon() {
      const code = document.getElementById('couponInput').value.trim().toUpperCase();
      const feedback = document.getElementById('couponFeedback');
      feedback.classList.remove('hidden');

      if (code === 'PAWAN100' || code === 'APNA100') {
        appliedCoupon = { code: code, discount: 100 };
        feedback.className = 'text-[11px] font-semibold text-emerald-600';
        feedback.innerHTML = `<i class="fa-solid fa-check mr-1"></i> Promo ${code} applied! Saved ₹100`;
      } else if (code === 'FREESHIP') {
        appliedCoupon = { code: 'FREESHIP', discount: 25 };
        feedback.className = 'text-[11px] font-semibold text-emerald-600';
        feedback.innerHTML = '<i class="fa-solid fa-check mr-1"></i> Free Shipping coupon applied!';
      } else {
        appliedCoupon = null;
        feedback.className = 'text-[11px] font-semibold text-red-500';
        feedback.innerHTML = '<i class="fa-solid fa-circle-exclamation mr-1"></i> Invalid coupon. Try PAWAN100';
      }
      updateCartUI();
    }

    /* ==========================================================================
       CHECKOUT & DISPATCH TO p01hariprajapati@gmail.com
       ========================================================================== */
    function openCheckoutModal() {
      if (cart.length === 0) {
        showToast('Your basket is empty!');
        return;
      }
      toggleCart(false);
      openModal('checkoutModal');
    }

    async function handlePlaceOrder(event) {
      event.preventDefault();

      if (cart.length === 0) {
        showToast('Cart is empty!');
        return;
      }

      const submitBtn = document.getElementById('submitOrderBtn');
      submitBtn.disabled = true;
      submitBtn.innerHTML = `<i class="fa-solid fa-circle-notch fa-spin"></i> <span>Sending Order Details...</span>`;

      const name = document.getElementById('custName').value.trim();
      const phone = document.getElementById('custPhone').value.trim();
      const area = document.getElementById('custArea').value;
      const address = document.getElementById('custAddress').value.trim();
      const paymentMethod = document.querySelector('input[name="paymentMethod"]:checked').value;

      const subtotal = cart.reduce((sum, item) => sum + (item.product.price * item.quantity), 0);
      const deliveryFee = subtotal >= 199 ? 0 : 25;
      const discount = appliedCoupon ? appliedCoupon.discount : 0;
      const grandTotal = Math.max(0, subtotal + deliveryFee - discount);
      const randomOrderId = '#PM-' + Math.floor(10000 + Math.random() * 90000);

      const itemsListText = cart.map(item => 
        `• ${item.product.title} (${item.product.weight}) x ${item.quantity} = ₹${item.product.price * item.quantity}`
      ).join('\n');

      let isSuccess = false;

      // Submit directly using your activated FormSubmit endpoint[cite: 1]
      try {
        const response = await fetch(`https://formsubmit.co/ajax/${FORMSUBMIT_TOKEN}`, {
          method: "POST",
          headers: {
            "Content-Type": "application/json",
            "Accept": "application/json"
          },
          body: JSON.stringify({
            _subject: `🛒 New Pawan Mart Ranchi Order: ${randomOrderId} from ${name} (₹${grandTotal})`,
            Customer_Name: name,
            Customer_Phone: phone,
            City: "Ranchi, Jharkhand",
            Neighborhood: area,
            Address: address,
            Payment_Method: paymentMethod,
            Ordered_Items: `\n${itemsListText}`,
            Total_Bill: `₹${grandTotal}`,
            _template: "table"
          })
        });

        if (response.ok) {
          isSuccess = true;
        }
      } catch (err) {
        console.warn('Network call failed, using mail client fallback...', err);
      }

      if (!isSuccess) {
        const fullEmailBody = `Order ID: ${randomOrderId}\nCustomer: ${name} (${phone})\nArea: ${area}\nAddress: ${address}\nPayment: ${paymentMethod}\n\nItems:\n${itemsListText}\n\nTotal: ₹${grandTotal}`;
        const mailtoLink = `mailto:${STORE_OWNER_EMAIL}?subject=${encodeURIComponent(`New Pawan Mart Order: ${randomOrderId} - ${name}`)}&body=${encodeURIComponent(fullEmailBody)}`;
        window.open(mailtoLink, "_blank");
      }

      document.getElementById('confirmedOrderId').innerText = randomOrderId;
      document.getElementById('confirmedCustName').innerText = `${name} (${phone})`;

      cart = [];
      appliedCoupon = null;
      updateCartUI();
      renderProducts();
      document.getElementById('orderCheckoutForm').reset();
      
      closeModal('checkoutModal');
      openModal('orderSuccessModal');
      showToast(`Order details forwarded to ${STORE_OWNER_EMAIL}`);

      submitBtn.disabled = false;
      submitBtn.innerHTML = `<i class="fa-solid fa-check"></i> <span>Confirm & Place Order</span>`;
    }

    /* ==========================================================================
       MODALS & TOAST HELPERS
       ========================================================================== */
    function openModal(id) {
      document.getElementById(id).classList.remove('hidden');
      document.body.classList.add('overflow-hidden');
    }

    function closeModal(id) {
      document.getElementById(id).classList.add('hidden');
      document.body.classList.remove('overflow-hidden');
    }

    function showToast(message) {
      const container = document.getElementById('toastContainer');
      const toast = document.createElement('div');
      toast.className = 'bg-slate-900/95 backdrop-blur-md text-white text-xs font-semibold px-4 py-2.5 rounded-2xl shadow-2xl flex items-center gap-2 transform translate-y-3 transition-all duration-300 pointer-events-auto border border-slate-700/60';
      toast.innerHTML = `
        <span class="w-2 h-2 rounded-full bg-amber-400"></span>
        <span>${message}</span>
      `;
      container.appendChild(toast);

      setTimeout(() => toast.classList.remove('translate-y-3'), 10);
      setTimeout(() => {
        toast.classList.add('opacity-0', 'translate-y-2');
        setTimeout(() => toast.remove(), 300);
      }, 3200);
    }
  </script>
</body>
</html>
