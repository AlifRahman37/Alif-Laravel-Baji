<!DOCTYPE html>
<html lang="bn">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>777win | Leading Sports Exchange & Live Casino</title>
    
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;500;700;900&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.css" />

    <style>
        :root {
            --primary-green: #00a859;
            --bg-body: #f0f2f5;
            --league-yellow: #f7bc15;
            --back-blue: #a5d9fe;
            --lay-pink: #f9d0d9;
        }

        body { 
            font-family: 'Roboto', sans-serif; 
            background-color: var(--bg-body); 
            color: #333;
        }

        .no-scrollbar::-webkit-scrollbar { display: none; }
        .glass-nav {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            border-bottom: 1px solid #e5e7eb;
        }

        .odds-box {
            width: 60px; height: 42px;
            display: flex; flex-direction: column;
            align-items: center; justify-content: center;
            border-radius: 4px; border: 1px solid rgba(0,0,0,0.03);
        }
        .bg-back { background-color: var(--back-blue); color: #0369a1; }
        .bg-lay { background-color: var(--lay-pink); color: #be185d; }
        
        .live-dot {
            width: 6px; height: 6px;
            background-color: #ef4444;
            border-radius: 50%;
            display: inline-block;
            animation: pulse 1.5s infinite;
        }
        @keyframes pulse {
            0% { transform: scale(1); opacity: 1; }
            50% { transform: scale(1.5); opacity: 0.5; }
            100% { transform: scale(1); opacity: 1; }
        }
    </style>
</head>
<body class="pb-20">

    <header class="glass-nav sticky top-0 z-[2000] px-4 py-3 flex justify-between items-center">
        <div class="flex items-center gap-3">
            <i class="fa-solid fa-bars text-xl text-gray-600"></i>
            <h1 class="text-2xl font-black italic tracking-tighter text-green-600">777WIN</h1>
        </div>
        <div class="flex gap-2">
            {{-- লারাভেল রাউট ব্যবহার করা হয়েছে --}}
            <a href="{{ url('/register') }}" class="px-4 py-1.5 border-2 border-green-500 text-green-600 rounded-lg font-bold text-sm">Sign up</a>
            <a href="{{ url('/login') }}" class="px-4 py-1.5 bg-green-600 text-white rounded-lg font-bold text-sm shadow-lg">Login</a>
        </div>
    </header>

    {{-- নেভিগেশন ট্যাব --}}
    <nav class="bg-white sticky top-[57px] z-[1999] border-b flex overflow-x-auto no-scrollbar">
        <button class="px-6 py-3 text-sm font-black text-green-600 border-b-4 border-green-600 whitespace-nowrap">LIVE</button>
        <button class="px-6 py-3 text-sm font-bold text-gray-400 whitespace-nowrap">UPCOMING</button>
        <button class="px-6 py-3 text-sm font-bold text-gray-400 whitespace-nowrap">LEAGUES</button>
    </nav>

    {{-- ব্যানার স্লাইডার --}}
    <div class="swiper mySwiper p-4 bg-white">
        <div class="swiper-wrapper">
            <div class="swiper-slide">
                <div class="h-44 rounded-3xl bg-gradient-to-tr from-green-600 to-green-400 p-6 flex items-center justify-between text-white relative overflow-hidden">
                    <div>
                        <h4 class="text-xs font-bold uppercase tracking-widest opacity-80">Welcome Bonus</h4>
                        <h2 class="text-4xl font-black italic leading-tight mt-1">BIG PUNCH<br><span class="text-yellow-300">WIN PRIZES</span></h2>
                    </div>
                </div>
            </div>
        </div>
    </div>

    {{-- গেম ক্যাটাগরি --}}
    <section class="bg-white py-4 flex overflow-x-auto no-scrollbar gap-4 px-4 border-b">
        <div class="flex flex-col items-center min-w-[75px]">
            <div class="w-14 h-14 bg-green-600 rounded-2xl flex items-center justify-center text-white shadow-xl shadow-green-100"><i class="fa-solid fa-trophy text-2xl"></i></div>
            <span class="text-[10px] font-black mt-2 text-green-600 uppercase tracking-tighter">Sports</span>
        </div>
        <div class="flex flex-col items-center min-w-[75px]">
            <div class="w-14 h-14 bg-white rounded-2xl flex items-center justify-center text-gray-400 border border-gray-100"><i class="fa-solid fa-clover text-2xl"></i></div>
            <span class="text-[10px] font-black mt-2 text-gray-500 uppercase tracking-tighter">Casino</span>
        </div>
    </section>

    {{-- আইপিএল কার্ড (উদাহরণ) --}}
    <div class="bg-white mt-3 border-b border-gray-200">
        <div class="bg-yellow-400 px-4 py-2 flex justify-between items-center text-xs font-black uppercase">
            <span><i class="fa-solid fa-medal mr-2"></i> Indian Premier League (IPL)</span>
            <i class="fa-solid fa-chevron-right text-[10px]"></i>
        </div>
        <div class="p-4 flex justify-between items-center border-b border-gray-50">
            <div>
                <span class="font-bold text-sm text-gray-700 block">Mumbai Indians</span>
                <span class="text-[9px] text-orange-500 font-bold flex items-center gap-1"><span class="live-dot"></span> LIVE NOW</span>
            </div>
            <div class="flex gap-2">
                <div class="odds-box bg-back"><span class="font-black text-sm">2.44</span><span class="text-[8px] opacity-70">2.1K</span></div>
                <div class="odds-box bg-lay"><span class="font-black text-sm">2.46</span><span class="text-[8px] opacity-70">850</span></div>
            </div>
        </div>
    </div>

    {{-- বটম নেভিগেশন --}}
    <nav class="fixed bottom-0 left-0 right-0 bg-white border-t h-16 flex justify-around items-center px-4 z-[3000] shadow-lg">
        <a href="{{ url('/') }}" class="flex flex-col items-center text-green-600">
            <i class="fa-solid fa-house-chimney text-lg"></i>
            <span class="text-[9px] font-black uppercase mt-1">Home</span>
        </a>
        <a href="{{ url('/deposit') }}" class="relative">
            <div class="w-14 h-14 bg-green-500 rounded-full -mt-10 border-4 border-[#f0f2f5] flex items-center justify-center text-white shadow-xl shadow-green-200">
                <i class="fa-solid fa-plus text-2xl"></i>
            </div>
            <span class="text-[9px] font-black uppercase mt-1 text-gray-400 text-center block">Deposit</span>
        </a>
        <a href="{{ url('/profile') }}" class="flex flex-col items-center text-gray-400">
            <i class="fa-solid fa-user-gear text-lg"></i>
            <span class="text-[9px] font-black uppercase mt-1">Account</span>
        </a>
    </nav>

    <script src="https://cdn.jsdelivr.net/npm/swiper@11/swiper-bundle.min.js"></script>
    <script>
        var swiper = new Swiper(".mySwiper", { loop: true, autoplay: { delay: 4000 } });
        console.log("Integrated by Alif Rahman for 777win project.");
    </script>
</body>
</html>
