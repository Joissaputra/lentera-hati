
<html lang="id" class="scroll-smooth">
<head>
  
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    
    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@200;300;400&family=Syne:wght@400;500&display=swap" rel="stylesheet">

    <!-- Swiper JS for Sliders -->
    <link rel="stylesheet" href="https://unpkg.com/swiper/swiper-bundle.min.css" />
    <script src="https://unpkg.com/swiper/swiper-bundle.min.js"></script>

    <!-- Feather Icons -->
    <script src="https://unpkg.com/feather-icons"></script>

    <style>
        body {
            font-family: 'Poppins', sans-serif;
            background-color: #0A0B1A; /* Deep Indigo */
            color: #E5E7EB; /* Gray 200 */
        }
        .font-heading {
            font-family: 'Syne', sans-serif;
            font-weight: 800;
        }
        .hero-bg {
            background: linear-gradient(to top, #0A0B1A 10%, rgba(10, 11, 26, 0.7)), url('https://images.unsplash.com/photo-1506126613408-eca0ce68773?q=80&w=1200&auto=format&fit=crop') center center/cover no-repeat;
        }
        .gradient-text {
            background: linear-gradient(90deg, #A855F7, #EC4899);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        .btn-primary {
            background-color: #A855F7; /* Purple 500 */
            color: #111827;
            font-weight: 700;
            border-radius: 9999px;
            padding: 0.8rem 1.8rem;
            transition: all 0.3s ease;
            box-shadow: 0 4px 20px rgba(168, 85, 247, 0.3);
        }
        .btn-primary:hover {
            transform: translateY(-3px) scale(1.05);
            box-shadow: 0 7px 25px rgba(168, 85, 247, 0.4);
        }
        .card-bg {
            background: rgba(255, 255, 255, 0.05);
            border: 1px solid rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
            -webkit-backdrop-filter: blur(10px);
        }
        .swiper-pagination-bullet-active {
            background: #A855F7 !important;
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
        .accordion-content {
            max-height: 0;
            overflow: hidden;
            transition: max-height 0.5s ease-in-out, padding 0.5s ease-in-out;
        }
    </style>
</head>
<body class="antiasa">

    <!-- Header -->
    <header class="fixed top-0 left-0 w-full z-50 bg-gray-900/50 backdrop-blur-sm">
        <nav class="container mx-auto px-6 py-4 flex justify-between items-center">
            <a href="#" class="font-heading text-xl font-bold text-white">
                Lentera<span class="text-purple-400">Hati</span>
            </a>
            <a href="#pendaftaran" class="btn-primary text-sm">
                Daftar Kelas
            </a>
        </nav>
    </header>

    <!-- Hero Section -->
    <section class="hero-bg min-h-screen flex items-center justify-center text-center pt-20 px-4">
        <div>
            <div class="inline-block bg-purple-400/10 text-purple-300 text-sm font-semibold px-4 py-1 rounded-full mb-4">
                PEMBUKAAN KELAS GELOMBANG 37
            </div>
            <h1 class="font-heading text-4xl md:text-6xl text-white leading-tight">
                Temukan <span class="gradient-text">Kedamaian Batin</span> & Keseimbangan Hidup
            </h1>
            <p class="mt-6 text-lg max-w-2xl mx-auto text-gray-300">
                Bergabunglah dalam kelas Reiki GRATIS kami dan mulailah perjalanan penyembuhan diri Anda yang mendalam bersama komunitas yang suportif.
            </p>
            <div class="mt-10">
                <a href="#pendaftaran" class="btn-primary text-lg">
                    Amankan Tempatmu Sekarang
                </a>
            </div>
        </div>
    </section>

    <main class="overflow-x-hidden">
        
        <!-- About Reiki Section - NEW -->
        <section class="py-20 px-6">
            <div class="text-center max-w-3xl mx-auto fade-in">
                <h2 class="font-heading text-3xl text-white">Apa Itu Reiki?</h2>
                <p class="mt-4 text-gray-300 max-w-2xl mx-auto">
                    Reiki adalah teknik penyembuhan energi kuno dari Jepang yang bekerja dengan menyalurkan "energi kehidupan universal" melalui sentuhan lembut. Praktik ini membantu menyeimbangkan energi tubuh, pikiran, dan jiwa, sehingga mendukung proses penyembuhan alami.
                </p>
                <div class="mt-8 text-left max-w-xl mx-auto">
                    <h3 class="font-bold text-xl text-white">Manfaat Utama Reiki:</h3>
                    <ul class="mt-4 list-disc list-inside space-y-2 text-gray-400">
                        <li>Mengurangi stres dan kecemasan</li>
                        <li>Meningkatkan kualitas tidur</li>
                        <li>Meringankan rasa sakit fisik</li>
                        <li>Mendukung keseimbangan emosional</li>
                        <li>Memperkuat sistem kekebalan tubuh</li>
                        <li>Meningkatkan kejernihan mental dan fokus</li>
                        <li>Membuka pintu menuju pertumbuhan spiritual</li>
                    </ul>
                </div>
            </div>
        </section>

        <!-- Programs Section -->
        <section class="py-20 px-6">
            <div class="text-center max-w-3xl mx-auto fade-in">
                <h2 class="font-heading text-3xl text-white">Kurikulum Pembelajaran Komprehensif</h2>
                <p class="mt-2 text-gray-400">Setiap program dirancang untuk membimbing Anda secara holistik dalam seni penyembuhan energi.</p>
            </div>
            <div id="accordion-container" class="mt-12 max-w-2xl mx-auto space-y-4">
                <!-- Accordion Item 1 -->
                <div class="card-bg rounded-xl fade-in">
                    <button class="accordion-header w-full flex justify-between items-center text-left p-5">
                        <span class="text-lg font-semibold text-white">Usui Tradisional Reiki</span>
                        <i data-feather="chevron-down" class="w-5 h-5 text-purple-400 transition-transform duration-500 accordion-icon"></i>
                    </button>
                    <div class="accordion-content px-5">
                        <p class="text-gray-400 pb-5">Mempelajari fondasi utama penyembuhan energi, termasuk sejarah, prinsip, posisi tangan untuk menyembuhkan diri sendiri dan orang lain, serta penggunaan simbol-simbol suci Reiki untuk memperkuat aliran energi.</p>
                    </div>
                </div>
                <!-- Accordion Item 2 -->
                <div class="card-bg rounded-xl fade-in">
                    <button class="accordion-header w-full flex justify-between items-center text-left p-5">
                        <span class="text-lg font-semibold text-white">Shambala</span>
                        <i data-feather="chevron-down" class="w-5 h-5 text-purple-400 transition-transform duration-500 accordion-icon"></i>
                    </button>
                    <div class="accordion-content px-5">
                        <p class="text-gray-400 pb-5">Menggabungkan energi Reiki dengan getaran cinta kasih dari para Ascended Masters. Shambala mempercepat proses penyembuhan dan pertumbuhan spiritual, membuka kesadaran akan multidimensionalitas diri.</p>
                    </div>
                </div>
                <!-- Accordion Item 3 -->
                <div class="card-bg rounded-xl fade-in">
                    <button class="accordion-header w-full flex justify-between items-center text-left p-5">
                        <span class="text-lg font-semibold text-white">Kundalini Reiki</span>
                        <i data-feather="chevron-down" class="w-5 h-5 text-purple-400 transition-transform duration-500 accordion-icon"></i>
                    </button>
                    <div class="accordion-content px-5">
                        <p class="text-gray-400 pb-5">Fokus pada aktivasi dan pembersihan jalur energi Kundalini, yaitu energi spiritual yang tertidur di dasar tulang belakang. Tujuannya adalah untuk mencapai pencerahan, meningkatkan intuisi, dan vitalitas tubuh.</p>
                    </div>
                </div>
                  <!-- Accordion Item 4 -->
                <div class="card-bg rounded-xl fade-in">
                    <button class="accordion-header w-full flex justify-between items-center text-left p-5">
                        <span class="text-lg font-semibold text-white">Ho'oponopono</span>
                        <i data-feather="chevron-down" class="w-5 h-5 text-purple-400 transition-transform duration-500 accordion-icon"></i>
                    </button>
                    <div class="accordion-content px-5">
                        <p class="text-gray-400 pb-5">Teknik kuno dari Hawaii untuk pembersihan mental dan emosional. Melalui empat frasa kunci, Anda akan belajar melepaskan beban masa lalu, memaafkan, dan menciptakan kedamaian batin sejati.</p>
                    </div>
                </div>
                <!-- Accordion Item 5 - NEW -->
                <div class="card-bg rounded-xl fade-in">
                    <button class="accordion-header w-full flex justify-between items-center text-left p-5">
                        <span class="text-lg font-semibold text-white">Reiki White Lotus</span>
                        <i data-feather="chevron-down" class="w-5 h-5 text-purple-400 transition-transform duration-500 accordion-icon"></i>
                    </button>
                    <div class="accordion-content px-5">
                        <p class="text-gray-400 pb-5">Reiki White Lotus adalah sistem energi yang berfokus pada pemurnian mendalam, membawa kedamaian, dan membuka potensi spiritual.membantu membersihkan energi negatif, dan menciptakan aura yang lebih terang dan murni.</p>
                    </div>
                </div>
                <!-- Accordion Item 6 - NEW -->
                <div class="card-bg rounded-xl fade-in">
                    <button class="accordion-header w-full flex justify-between items-center text-left p-5">
                        <span class="text-lg font-semibold text-white">Program Khusus Lainnya</span>
                        <i data-feather="chevron-down" class="w-5 h-5 text-purple-400 transition-transform duration-500 accordion-icon"></i>
                    </button>
                    <div class="accordion-content px-5">
                        <p class="text-gray-400 pb-5">Selain kurikulum utama, kami juga menawarkan berbagai program khusus seperti pelatihan untuk menjadi Master Reiki, sesi penyembuhan jarak jauh (distant healing), dan lokakarya tematik untuk memperdalam praktik spiritual Anda.</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Facilities Section -->
        <section class="py-20 px-6 bg-gray-900/50">
            <div class="text-center max-w-3xl mx-auto fade-in">
                <h2 class="font-heading text-3xl text-white">Fasilitas & Dukungan Premium</h2>
                <p class="mt-2 text-gray-400">Kami menyediakan semua yang Anda butuhkan untuk perjalanan spiritual yang optimal.</p>
            </div>
            <div class="mt-12 grid grid-cols-1 sm:grid-cols-2 gap-8 max-w-3xl mx-auto">
                <!-- Facility Card 1 -->
                <div class="text-center fade-in">
                    <div class="mx-auto bg-purple-500/10 w-16 h-16 rounded-full flex items-center justify-center">
                        <i data-feather="life-buoy" class="w-8 h-8 text-purple-400"></i>
                    </div>
                    <h3 class="mt-4 text-xl font-bold text-white">Bimbingan Gratis Tanpa Batas</h3>
                    <p class="mt-2 text-gray-400">Akses seumur hidup ke materi, konsultasi pribadi, dan bimbingan berkelanjutan tanpa biaya tambahan.</p>
                </div>
                <!-- Facility Card 2 -->
                <div class="text-center fade-in">
                    <div class="mx-auto bg-purple-500/10 w-16 h-16 rounded-full flex items-center justify-center">
                        <i data-feather="award" class="w-8 h-8 text-purple-400"></i>
                    </div>
                    <h3 class="mt-4 text-xl font-bold text-white">Mentor Profesional</h3>
                    <p class="mt-2 text-gray-400">Belajar langsung dari para praktisi dan ahli bersertifikasi yang berdedikasi pada kemajuan Anda.</p>
                </div>
                <!-- Facility Card 3 -->
                <div class="text-center fade-in">
                    <div class="mx-auto bg-purple-500/10 w-16 h-16 rounded-full flex items-center justify-center">
                        <i data-feather="wifi" class="w-8 h-8 text-purple-400"></i>
                    </div>
                    <h3 class="mt-4 text-xl font-bold text-white">Pembelajaran Full Daring</h3>
                    <p class="mt-2 text-gray-400">Nikmati fleksibilitas belajar dari mana saja melalui grup WhatsApp/Telegram dan sesi Zoom interaktif.</p>
                </div>
                <!-- Facility Card 4 -->
                <div class="text-center fade-in">
                    <div class="mx-auto bg-purple-500/10 w-16 h-16 rounded-full flex items-center justify-center">
                        <i data-feather="shield" class="w-8 h-8 text-purple-400"></i>
                    </div>
                    <h3 class="mt-4 text-xl font-bold text-white">Pemurnian & Penyembuhan</h3>
                    <p class="mt-2 text-gray-400">Sesi khusus untuk membersihkan aura dan chakra, serta layanan penyembuhan jarak jauh untuk mendukung kesejahteraan Anda.</p>
                </div>
            </div>
        </section>

        <!-- Gallery Section -->
        <section class="py-20">
            <div class="text-center px-6 fade-in">
                <h2 class="font-heading text-3xl text-white">Galeri Komunitas</h2>
                <p class="mt-2 text-gray-400">Potret kebersamaan dalam setiap sesi kami.</p>
            </div>
            <div class="swiper-container mt-12 fade-in" id="gallery-slider">
                <div class="swiper-wrapper">
                    <!-- Corrected image URLs and alt text -->
                    <div class="swiper-slide"><img src="https://www.dropbox.com/scl/fi/dfcoznksdgnm2wehk27xa/IMG-20250408-WA0006.jpg?rlkey=k4gpc1ofdqdsh6t41vsovj6rw&st=1459vaem&raw=1" alt="Kegiatan Reiki 1" class="rounded-2xl aspect-video object-cover"></div>
                    <div class="swiper-slide"><img src="https://www.dropbox.com/scl/fi/7olljvfvvch1ki9974hqv/IMG-20250408-WA0004.jpg?rlkey=yh1xkpa1ppsdg9w4aq4x1autc&st=qq37r1zo&raw=1" alt="Kegiatan Reiki 2" class="rounded-2xl aspect-video object-cover"></div>
                    <div class="swiper-slide"><img src="https://www.dropbox.com/scl/fi/9jfucfcea5n26focmzcri/IMG-20230501-WA0009.jpg?rlkey=tu3i598tcwsb79mi6infnhvxe&st=unipufz7&raw=1" alt="Kegiatan Reiki 3" class="rounded-2xl aspect-video object-cover"></div>
                    <div class="swiper-slide"><img src="https://www.dropbox.com/scl/fi/n01pu9s3ropfn4akq3lwq/FB_IMG_1755507226204.jpg?rlkey=34uque5evelk4qj17p1ugyvne&st=ydaz2ns4&raw=1" alt="Kegiatan Reiki 4" class="rounded-2xl aspect-video object-cover"></div>
                    <!-- NEW SLIDES ADDED HERE -->
                    <div class="swiper-slide"><img src="https://images.unsplash.com/photo-1544410191-23d24075196f?q=80&w=1200&auto=format&fit=crop" alt="Komunitas Meditasi" class="rounded-2xl aspect-video object-cover"></div>
                    <div class="swiper-slide"><img src="https://images.unsplash.com/photo-1517482438596-f0f72535091c?q=80&w=1200&auto=format&fit=crop" alt="Latihan Relaksasi" class="rounded-2xl aspect-video object-cover"></div>
                    <div class="swiper-slide"><img src="https://images.unsplash.com/photo-1599908643878-5779035e4d22?q=80&w=1200&auto=format&fit=crop" alt="Penyembuhan Energi" class="rounded-2xl aspect-video object-cover"></div>
                    <div class="swiper-slide"><img src="https://images.unsplash.com/photo-1588725455938-1a5c602c3751?q=80&w=1200&auto=format&fit=crop" alt="Sesi Bimbingan" class="rounded-2xl aspect-video object-cover"></div>
                    <div class="swiper-slide"><img src="https://images.unsplash.com/photo-1517377561962-d45ac1a9a81f?q=80&w=1200&auto=format&fit=crop" alt="Kebersamaan Peserta" class="rounded-2xl aspect-video object-cover"></div>
                    <div class="swiper-slide"><img src="https://images.unsplash.com/photo-1506126613408-eca0ce68773?q=80&w=1200&auto=format&fit=crop" alt="Lentera Hati Komunitas" class="rounded-2xl aspect-video object-cover"></div>
                </div>
                <div class="swiper-pagination mt-8 relative"></div>
            </div>
        </section>

        <!-- Testimonials Section -->
        <section class="py-20 px-6 bg-gray-900/50">
            <div class="text-center max-w-3xl mx-auto fade-in">
                <h2 class="font-heading text-3xl text-white">Apa Kata Mereka?</h2>
            </div>
            <div class="mt-12 max-w-2xl mx-auto space-y-8">
                <!-- Testimonial 1 -->
                <div class="card-bg p-6 rounded-2xl border-l-4 border-purple-400 fade-in">
                    <p class="text-lg italic text-gray-200">"Ikut kelas ini adalah keputusan terbaik. Pikiran jadi lebih jernih, tidur lebih nyenyak, dan yang paling penting, saya merasa lebih 'utuh'. Mentornya sangat sabar dan komunitasnya positif banget."</p>
                    <p class="mt-4 font-bold text-right text-white">- Maya, Karyawan Swasta</p>
                </div>
                <!-- Testimonial 2 -->
                <div class="card-bg p-6 rounded-2xl border-l-4 border-pink-300 fade-in">
                    <p class="text-lg italic text-gray-200">"Sebagai orang yang gampang cemas, materi Ho'oponopono benar-benar mengubah cara pandang saya. Belajar melepaskan beban itu ternyata melegakan. Terima kasih Lentera Hati!"</p>
                    <p class="mt-4 font-bold text-right text-white">- Dito, Mahasiswa</p>
                </div>
            </div>
        </section>


        <!-- CTA / Registration Section -->
        <section id="pendaftaran" class="py-20 px-6 text-center">
            <div class="fade-in">
                <h2 class="font-heading text-4xl gradient-text">Siap Memulai Perjalanan Anda?</h2>
                <p class="mt-4 text-lg text-gray-300 max-w-md mx-auto">
                    Pendaftaran Gelombang 37 telah dibuka. Hubungi admin kami melalui WhatsApp untuk bergabung. Tempat terbatas!
                </p>
                <div class="mt-10 flex flex-col gap-4 max-w-xs mx-auto">
                    <!-- Updated WhatsApp link for Admin Terru with pre-filled message -->
                    <a href="https://wa.me/6282231691821?text=Saya....%2C%20Domisili.....%20Berminat%20Bergabung%20Dengan%20Lentera%20Hati%20Indonesia" target="_blank" class="block w-full bg-green-500 text-white font-bold py-4 px-6 rounded-full text-lg hover:bg-green-600 transition-all transform hover:scale-105">
                        Chat Admin Terru
                    </a>
                    <!-- Updated WhatsApp link for Admin Jois with pre-filled message -->
                    <a href="https://wa.me/6288221544982?text=Saya....%2C%20Domisili.....%20Berminat%20Bergabung%20Dengan%20Lentera%20Hati%20Indonesia" target="_blank" class="block w-full bg-gray-700 text-white font-bold py-4 px-6 rounded-full text-lg hover:bg-gray-600 transition-all transform hover:scale-105">
                        Chat Admin Jois
                    </a>
                </div>
            </div>
        </section>
    </main>

    <!-- Footer -->
    <footer class="text-center py-10 px-6 border-t border-gray-800">
        <p class="text-gray-500 text-sm">&copy; 2024 REIKI LENTERA HATI INDONESIA. Dirancang dengan Penuh Cinta.</p>
    </footer>

    <script>
        // Initialize Feather Icons
        feather.replace();

        // Accordion Logic
        document.addEventListener('DOMContentLoaded', () => {
            const accordionHeaders = document.querySelectorAll('.accordion-header');
            accordionHeaders.forEach(header => {
                header.addEventListener('click', () => {
                    const content = header.nextElementSibling;
                    const icon = header.querySelector('.accordion-icon');
                    
                    // Close all other accordions
                    document.querySelectorAll('.accordion-content').forEach(c => {
                        if (c !== content) {
                            c.style.maxHeight = null;
                            const otherIcon = c.previousElementSibling.querySelector('.accordion-icon');
                            if (otherIcon) {
                                otherIcon.style.transform = 'rotate(0deg)';
                            }
                        }
                    });

                    // Toggle the clicked accordion
                    if (content.style.maxHeight) {
                        content.style.maxHeight = null;
                        if (icon) icon.style.transform = 'rotate(0deg)';
                    } else {
                        content.style.maxHeight = content.scrollHeight + "px";
                        if (icon) icon.style.transform = 'rotate(180deg)';
                    }
                });
            });
        });


        // Initialize Gallery Swiper
        var gallerySlider = new Swiper('#gallery-slider', {
            loop: true,
            slidesPerView: 1.2,
            spaceBetween: 16,
            centeredSlides: true,
            pagination: {
                el: '.swiper-pagination',
                clickable: true,
            },
            autoplay: {
                delay: 3500,
                disableOnInteraction: false,
            },
        });

        // Scroll Animation
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('visible');
                }
            });
        }, {
            threshold: 0.1
        });

        document.querySelectorAll('.fade-in').forEach(el => {
            observer.observe(el);
        });
    </script>

</body>
</html>

