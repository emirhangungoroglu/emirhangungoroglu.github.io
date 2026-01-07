---
layout: post
title: "VANTAVIGIL v5.0: Forensic Intelligence & Analysis Station"
date: 2026-01-07
author: Emirhan Gungoroglu
categories: [blog, cybersecurity]
---

<div class="vanta-blog-wrapper">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700;900&family=JetBrains+Mono:wght@400;700&display=swap');

        .vanta-blog-wrapper {
            background: #020202;
            color: #ccc;
            font-family: 'JetBrains Mono', monospace;
            padding: 40px;
            border: 1px solid #111;
            max-width: 1000px;
            margin: 0 auto;
            line-height: 1.8;
            position: relative;
        }

        /* DİL SEÇİCİ */
        .vanta-lang-nav {
            display: flex;
            justify-content: flex-end;
            gap: 15px;
            margin-bottom: 40px;
            border-bottom: 1px solid #111;
            padding-bottom: 20px;
        }

        .vanta-btn {
            background: transparent;
            color: #00d2ff;
            border: 1px solid #00d2ff;
            padding: 8px 25px;
            cursor: pointer;
            font-family: 'Orbitron', sans-serif;
            font-size: 11px;
            letter-spacing: 2px;
            transition: 0.3s;
        }

        .vanta-btn.active {
            background: #00d2ff;
            color: #000;
            box-shadow: 0 0 15px rgba(0, 210, 255, 0.4);
        }

        /* BAŞLIKLAR */
        .section-header {
            color: #00d2ff;
            border-left: 4px solid #00d2ff;
            padding-left: 15px;
            margin: 50px 0 20px 0;
            font-family: 'Orbitron', sans-serif;
            font-size: 1.2rem;
            letter-spacing: 4px;
            text-transform: uppercase;
        }

        .vanta-quote {
            background: #080808;
            border-left: 4px solid #00ff41;
            padding: 25px;
            margin: 30px 0;
            font-style: italic;
            color: #fff;
            border-radius: 0 10px 10px 0;
        }

        /* KARTLAR */
        .vanta-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
            margin: 40px 0;
        }

        .vanta-card {
            background: rgba(10, 10, 10, 0.8);
            border: 1px solid #1a1a1e;
            padding: 25px;
            border-radius: 12px;
            transition: 0.3s;
        }

        .vanta-card:hover {
            border-color: #00ff41;
            transform: translateY(-5px);
            box-shadow: 0 10px 30px rgba(0, 255, 65, 0.05);
        }

        .vanta-card h4 {
            color: #00ff41;
            margin-bottom: 15px;
            font-family: 'Orbitron', sans-serif;
            letter-spacing: 2px;
        }

        /* ÖNE ÇIKAN ÖZELLİK LİSTESİ */
        .vanta-list {
            list-style: none;
            padding: 0;
        }

        .vanta-list li {
            margin-bottom: 15px;
            padding-left: 25px;
            position: relative;
        }

        .vanta-list li::before {
            content: ">";
            position: absolute;
            left: 0;
            color: #00d2ff;
            font-weight: bold;
        }

        .vanta-cta-box {
            text-align: center;
            margin-top: 80px;
            padding-top: 50px;
            border-top: 1px solid #111;
        }

        .vanta-huge-btn {
            display: inline-block;
            padding: 20px 60px;
            font-family: 'Orbitron', sans-serif;
            font-size: 1.5rem;
            font-weight: 900;
            color: #000;
            background: #00d2ff;
            text-decoration: none;
            letter-spacing: 10px;
            transition: 0.4s;
            border-radius: 5px;
        }

        .vanta-huge-btn:hover {
            background: #fff;
            box-shadow: 0 0 50px #00d2ff;
            transform: scale(1.05);
        }

        #vanta-en { display: none; }
    </style>

    <div class="vanta-lang-nav">
        <button onclick="setVantaLang('tr')" id="vtr" class="vanta-btn active">TÜRKÇE</button>
        <button onclick="setVantaLang('en')" id="ven" class="vanta-btn">ENGLISH</button>
    </div>

    <div id="vanta-tr">
        <h1 style="color:#fff; text-align:center; letter-spacing:10px; font-family:'Orbitron';">VANTAVIGIL // ANALİZ GÜNCELLEMESİ</h1>
        
        <div class="vanta-quote">
            "Siber istihbarat, veriyi sadece toplamak değil; onun dijital parmak izini doğru okumaktır."
        </div>

        <h3 class="section-header">01_ DASHBOARD VE NAVİGASYON EVRİMİ</h3>
        <p>Vantavigil ana sayfasını (Home Page), gerçek bir <strong>Cybersecurity Dashboard</strong> deneyimine dönüştürdük. Profesyonel gri tonlarındaki yeni <strong>Navbar</strong>, merkezi "VANTAVIGIL" kimliği ve sağ üstteki <strong>"STATUS: ONLINE"</strong> pulse efekti ile operasyonel bir hava kazandı.</p>
        <ul class="vanta-list">
            <li><strong>5 Modüllü Grid:</strong> Gelecekteki araçlarımız için ölçeklenebilir, şık bir kart düzeni.</li>
            <li><strong>Şeffaflık Modülleri:</strong> Hem ana menüde hem de analiz sayfasında bulunan <strong>"?" butonları</strong> ile sistemin çalışma mantığını ve güvenlik politikamızı kullanıcıya anlık olarak sunuyoruz.</li>
        </ul>

        <h3 class="section-header">02_ YENİ BİRİM: FILE ANALYSIS CENTER</h3>
        <p>Bugün yayına aldığımız <strong>Module_02</strong>, basit bir hash hesaplayıcının ötesine geçerek kapsamlı bir adli bilişim (forensics) istasyonu görevi görüyor.</p>
        
        

        <div class="vanta-grid">
            <div class="vanta-card">
                <h4>MAGIC BYTES ANALİZİ</h4>
                <p>Dosya uzantısı yanıltıcı olsa bile, ilk 8 byte'lık hex imzasını okuyarak dosyanın gerçek türünü (EXE, PDF, PNG vb.) anında tespit eder.</p>
            </div>
            <div class="vanta-card">
                <h4>HİBRİT İSTİHBARAT</h4>
                <p>Hesaplanan SHA-256 imzası üzerinden VirusTotal ve Hybrid Analysis veritabanlarına doğrudan pivot yaparak tehdit seviyesini sorgular.</p>
            </div>
        </div>

        <h3 class="section-header">03_ %100 YEREL VE GÜVENLİ (ZERO-LOG)</h3>
        <p>En büyük önceliğimiz gizlilik. Vantavigil'e yüklediğiniz hiçbir dosya sunucularımıza <strong>GİTMEZ</strong>. Tüm işlemler JavaScript'in <code>FileReader</code> API'si ve <code>CryptoJS</code> kütüphanesi ile tamamen sizin tarayıcı belleğinizde gerçekleşir.</p>
    </div>

    <div id="vanta-en">
        <h1 style="color:#fff; text-align:center; letter-spacing:10px; font-family:'Orbitron';">VANTAVIGIL // ANALYSIS UPDATE</h1>
        
        <div class="vanta-quote">
            "Cyber intelligence is not just about collecting data; it's about correctly reading its digital fingerprint."
        </div>

        <h3 class="section-header">01_ DASHBOARD & NAVIGATION EVOLUTION</h3>
        <p>We've transformed the Vantavigil home page into a true <strong>Cybersecurity Dashboard</strong> experience. The new <strong>Navbar</strong> in professional grey tones, featuring a centered "VANTAVIGIL" identity and a <strong>"STATUS: ONLINE"</strong> pulse effect, provides a high-end operational feel.</p>
        <ul class="vanta-list">
            <li><strong>5-Module Grid:</strong> A scalable, sleek card layout designed for our future toolset.</li>
            <li><strong>Transparency Modules:</strong> Using the <strong>"?" info buttons</strong> in both the main menu and analysis pages, we provide real-time information about our security policy and system logic.</li>
        </ul>

        <h3 class="section-header">02_ NEW UNIT: FILE ANALYSIS CENTER</h3>
        <p>The newly released <strong>Module_02</strong> goes beyond a simple hash generator, serving as a comprehensive digital forensics station.</p>

        <div class="vanta-grid">
            <div class="vanta-card">
                <h4>MAGIC BYTES ANALYSIS</h4>
                <p>Even if file extensions are misleading, it detects the true file type (EXE, PDF, PNG, etc.) by reading the first 8 bytes of the hex signature.</p>
            </div>
            <div class="vanta-card">
                <h4>HYBRID INTELLIGENCE</h4>
                <p>Performs direct pivots to VirusTotal and Hybrid Analysis databases using the computed SHA-256 signature to query threat levels.</p>
            </div>
        </div>

        <h3 class="section-header">03_ 100% LOCAL & SECURE (ZERO-LOG)</h3>
        <p>Privacy is our core mission. No files uploaded to Vantavigil <strong>EVER LEAVE</strong> your device. All processing is executed within your browser's memory using the <code>FileReader</code> API and <code>CryptoJS</code> library.</p>
    </div>

    <div class="vanta-cta-box">
        <a href="https://emirhangungoroglu.github.io/vantavigil/" class="vanta-huge-btn">VANTAVIGIL</a>
    </div>

    <script>
        function setVantaLang(l) {
            document.getElementById('vanta-tr').style.display = (l === 'tr' ? 'block' : 'none');
            document.getElementById('vanta-en').style.display = (l === 'en' ? 'block' : 'none');
            document.getElementById('vtr').className = 'vanta-btn' + (l === 'tr' ? ' active' : '');
            document.getElementById('ven').className = 'vanta-btn' + (l === 'en' ? ' active' : '');
        }
    </script>
</div>
