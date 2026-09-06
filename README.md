<h1 align="center">TranslateNX </h1>

<div align="center">
  <img src="assets/logo.png" alt="TranslateNX Logo" width="200">

  ---
    
  <p align="center">
  <b>(EN)</b> TranslateNX is a revolutionary real-time translation overlay for the Nintendo Switch. It seamlessly reads text directly from your games and translates it on-the-fly, breaking language barriers without needing any game-specific patches or mods.

  ---

  <b>(TR)</b> TranslateNX, Nintendo Switch için devrim niteliğinde anlık çeviri aracıdır. Oyunlardaki metinleri doğrudan okuyup anında çevirerek, oyun yamalarına veya modlarına ihtiyaç duymadan dil engellerini ortadan kaldırır.
  </p>

  <br>

<a href="#en-setup-and-usage-guide" style="text-decoration:none;"><img src="https://img.shields.io/badge/Language-English-blue?style=for-the-badge" alt="English"></a> &nbsp;&nbsp; <a href="#tr-kurulum-ve-kullanım-rehberi" style="text-decoration:none;"><img src="https://img.shields.io/badge/Dil-Türkçe-red?style=for-the-badge" alt="Türkçe"></a>
</div>

---

## (EN) Setup and Usage Guide

### ✨ Features
* **Real-time Translation:** Translate on-screen game text instantly.
* **OCR Technology:** Directly reads text from the screen, no game mods required.
* **Wide Language Support:** Support for 104 different languages.
* **Practical Use:** Translate quickly without leaving the game using the UltraHand Overlay menu.
* **Multiple Service Options:** Supports Google Cloud Vision, OCR.space, DeepL, Google Cloud Translate, and MyMemory.

<div align="center">
  <img src="assets/TranslateNX4EN.png" alt="TranslateNX Screenshot" width="1000">
</div>

### ⚠️ Step 1: Critical Prep (Required)
To prevent your console from crashing, you must increase the **UltraHand memory limit**:
1. Open the UltraHand menu.
2. Press `+` to open settings, then go to **System**.
3. Change **Overlay Memory** from **4MB to 8MB**.

**IMPORTANT: If you continue to experience crashes, please turn off the enabled modules in Sysmodules.**

### 💾 Step 2: Installation
**Requirements:** You MUST have [nx-ovlloader](https://github.com/ppkantorski/nx-ovlloader) and [Ultrahand-Overlay](https://github.com/ppkantorski/Ultrahand-Overlay) installed for this app to work!

**Method 1: Homebrew App Store (Automatic Installation)**
You can download and install the application directly on your Switch via the HB App Store.

<div align="center">
   <a href="https://hb-app.store/switch/TranslateNX">
  <img src="assets/hbappstore.png" alt="HB App Store" width="250">
  <br>
  <a href="https://apps.fortheusers.org/switch/TranslateNX">HB Store Download Link</a>
</div>
<br>

**Method 2: Manual Installation**
You can install the application by downloading it on your computer and transferring it to your SD card.
* Download the [latest release](https://github.com/sertay1/TranslateNX/releases) `.zip` file. Extract it and drag all the contents directly to the root of your SD card. The files are already placed in their correct folder paths.

### 🔑 Step 3: Getting API Keys
TranslateNX needs services to read (OCR) and translate text. For the best performance, we highly recommend using Google Cloud Vision for OCR and DeepL for Translation.

#### 🔍 OCR API Options
**1. Google Cloud Vision (1000 Uses/Month) — ⭐ RECOMMENDED**
* Go to [Google Cloud Vision](https://cloud.google.com/vision) and click "Try Vision AI Free" to complete registration.
* On the Cloud Vision API page, click the "Enable" button.
* Go to the **Credentials** tab on the left menu. Select **Create Credentials > API Key** from the top.
* Name your API. In the *Select API restrictions* section, choose **Cloud Vision API**, click OK, and then Create. Your API key will appear in seconds.

**2. OCR.space (500 Uses/Day) — Alternative**
* Register at [OCR.space Free Key](https://ocr.space/OCRAPI).
* Click the confirmation link sent to your email. You will receive a second email with your API key seconds after confirming.

#### 🌍 Translation API Options
**1. DeepL (1,000,000 Characters Once) — ⭐ RECOMMENDED**
*(Note: 1 million characters will last a very long time. You can create a new free account when it runs out).*
* Sign up at [DeepL](https://www.deepl.com). Click your profile icon at the top right, then **Account**.
* Go to **API Plans** in the bottom left corner and subscribe to the free plan (it may ask for details but will not charge).
* Go to the **API Keys & Limits** tab and click **Create Key**.
* Name your API, select "All access", and click Create Key.

**2. Google Cloud Translate (500,000 Characters/Month) — Alternative**
*(Note: It may ask for card details and put a small hold during signup, but it is free as long as you stay within the quota).*
* Go to [Google Cloud Translate](https://cloud.google.com/translate) and register.
* Enable the **Cloud Translation API**.
* Go to **Credentials > Create Credentials > API Key**.
* Name your API, select Cloud Translation API from restrictions, and click Create.

**3. MyMemory (5,000 Characters/Day) — Fallback**
This is built-in. No API key is required. Simply select it from the app settings if you need a quick fallback.

#### 🤖 AI API Options
**1. Puter AI — 
* Go to [Puter.com](https://puter.com) and create a free account.
* Once logged in, open the developer dashboard to generate your API key.
* Puter AI offers generous limits for executing AI-based translations, providing context-aware and natural-sounding results.

**2. Google Gemini AI — Alternative**
* Go to [Google AI Studio](https://aistudio.google.com) and sign in with your Google account.
* Click on **"Get API key"** from the left menu and create a new key.
* Gemini provides extremely fast and smart context-based translations for complex game scenarios.

### 📝 Step 4: Entering API Keys
You can enter your API keys into the app using one of two methods:
* **Method 1 (Via Switch):** Open the TranslateNX app from the Hbmenu and type your API keys directly into the app interface.
* **Method 2 (Via PC - Easier):** Connect your Switch to your PC. Open the `SD:/config/translate/config.ini` file. Paste your API keys next to the respective fields, save, and put the file back on your Switch.

### 🎮 Step 5: How to Use
1. **Open UltraHand:** While in-game, swipe your finger from the left edge of the screen to the right, or press **L + R + D-Pad Down + Right Stick**.
2. **Launch TranslateNX:** Select TranslateNX from the list. *(Tip: You can press Y while hovering over it to set it as a shortcut).*
3. **Configure Settings:** Go to Settings. Select the OCR and Translation APIs you acquired.
4. **Set Languages:** 
   * **Source:** The original language of the game.
   * **Target:** Your language.
5. **Start Translating:** When there is text on the screen, open the TranslateNX menu and press **"Start Translating"**.
*(Note: The first translation might take a bit longer. Speed depends on the API and your internet connection).*

---

## 🔗 Contact and Donate

### SertAy

| Links | QR Code |
| :--- | :--- |
| **All Links:** [My Linktree](https://linktr.ee/yamanx) | <a href="https://linktr.ee/yamanx"><img src="assets/qr_SertAyTumLinkler.png" width="120"/></a> |

---

## (TR) Kurulum ve Kullanım Rehberi

### ✨ Özellikler
* **Anlık Çeviri:** Oyun oynarken ekrandaki yazıları anında Türkçe'ye çevirin.
* **OCR Teknolojisi:** Ekrandaki metni doğrudan okur, oyun modlarına ihtiyaç duymaz.
* **Geniş Dil Desteği:** 104 farklı dil desteği.
* **Pratik Kullanım:** UltraHand Overlay menüsü sayesinde oyundan çıkmadan hızlıca çeviri yapın.
* **Çoklu Servis Seçeneği:** Google Cloud Vision, OCR.space, DeepL, Google Cloud Translate ve MyMemory destekler.

<div align="center">
  <img src="assets/TranslateNX4TR.png" alt="TranslateNX Ekran Görüntüsü" width="1000">
</div>

### ⚠️ 1. Aşama: Kritik Ön Hazırlık (Zorunlu)
Cihazın çökmesini (crash) önlemek için **UltraHand bellek ayarını** değiştirmeniz şarttır:
1. UltraHand menüsünü açın.
2. `+` tuşuna basarak ayarlara, ardından **System** bölümüne girin.
3. **Overlay Memory** değerini **4MB'den 8MB'a** yükseltin.

**ÖNEMLİ: Eğer crash hatası almaya devam ederseniz. Sysmodules'te açık olan modülleri kapatınız.**

### 💾 2. Aşama: Kurulum
**Zorunlu Gereksinimler:** Uygulamanın çalışması için cihazınızda [nx-ovlloader](https://github.com/ppkantorski/nx-ovlloader) ve [Ultrahand-Overlay](https://github.com/ppkantorski/Ultrahand-Overlay) yüklü olmak ZORUNDADIR!

**Yöntem 1: Homebrew App Store (Otomatik Kurulum)**
Uygulamayı doğrudan Switch üzerinden HB App Store aracılığıyla indirip kurabilirsiniz.

<div align="center">
   <a href="https://hb-app.store/switch/TranslateNX">
  <img src="assets/hbappstore.png" alt="HB App Store" width="250">
  <br>
  <a href="https://apps.fortheusers.org/switch/TranslateNX">HB Store İndirme Linki</a>
</div>
<br>

**Yöntem 2: Manuel Kurulum**
Uygulamayı bilgisayarınıza indirip SD kartınıza atarak kurabilirsiniz.
* İndirdiğiniz [en güncel sürüm](https://github.com/sertay1/TranslateNX/releases) `.zip` dosyasını bilgisayara çıkartın. Çıkan tüm dosyaları doğrudan SD kartınızın ana dizinine sürükleyip bırakın (Dosyalar kendi yollarına hazır yerleştirilmiştir).

### 🔑 3. Aşama: Gerekli API'lerin Alınması
TranslateNX'in en iyi performansla çalışması için iki farklı sisteme ihtiyacı vardır. En iyi, en hızlı ve ücretsiz deneyim için OCR olarak **Google Cloud Vision**, çeviri için ise **DeepL** kullanmanızı tavsiye ederiz.

#### 🔍 OCR API Seçenekleri
**1. Google Cloud Vision (Aylık 1000 Kullanım) — ⭐ ÖNERİLEN**
* [Google Cloud Vision](https://cloud.google.com/vision) adresine gidin ve "Try Vision AI Free" butonuna tıklayıp gerekli kayıt işlemlerini tamamlayın.
* Açılan Cloud Vision API sayfasında "Enable" (Etkinleştir) butonuna basın.
* Sol menüden **Credentials** (Kimlik Bilgileri) sekmesine girin. Üst kısımdan **Create Credentials > API Key** yolunu izleyin.
* API'nize bir isim verin. *Select API restrictions* kısmından **Cloud Vision API**'yi seçin ve OK'a, ardından Create'e basın. API anahtarınız saniyeler içinde ekranda belirecektir.

**2. OCR.space (Günlük 500 Kullanım) — Alternatif**
* [OCR.space Free Key](https://ocr.space/OCRAPI) adresinden kayıt olun.
* E-posta adresinize gelen onay bağlantısına tıklayın. Onayladıktan saniyeler sonra API anahtarınızın bulunduğu ikinci bir e-posta alacaksınız.

#### 🌍 Çeviri API Seçenekleri
**1. DeepL (Tek Seferlik 1.000.000 Karakter) — ⭐ ÖNERİLEN**
*(Not: 1 milyon karakterlik kota genellikle sizi çok uzun süre idare edecektir. Kota dolduğunda yeni bir ücretsiz hesap açabilirsiniz).*
* [DeepL](https://www.deepl.com) sitesine gidip kayıt olun. Sağ üstteki profil simgenize, ardından **Hesap** butonuna tıklayın.
* Sol alt köşedeki **API Plans** menüsüne girin ve ücretsiz plana abone olun (Kayıt için bazı bilgiler isteyebilir ancak ücret kesmez).
* Açılan ekranda **API Keys & Limits** sekmesine tıklayın ve **Create Key** butonuna basın.
* API'nize bir isim verin, "All access" seçeneğini işaretleyin ve Create Key'e tıklayın.

**2. Google Cloud Translate (Aylık 500.000 Karakter) — Alternatif**
*(Not: Kayıt sırasında kart bilgisi isteyebilir ve küçük bir provizyon ücreti kesip iade edebilir. Aylık kotayı aşmadığınız sürece tamamen ücretsizdir).*
* [Google Cloud Translate](https://cloud.google.com/translate) adresine gidin ve kayıt işlemlerini tamamlayın.
* **Cloud Translation API** sayfasında "Enable" butonuna basın.
* **Credentials** sekmesine girip **Create Credentials > API Key** yolunu izleyin.
* API'nize isim verin, kısıtlamalar bölümünden Cloud Translation API'yi seçip Create butonuna basın.

**3. MyMemory (Günlük 5.000 Karakter) — Kurtarıcı**
Bu sistem TranslateNX içinde hazır kurulu gelir. API anahtarı almanıza gerek yoktur. Ayarlardan direkt seçerek zor anlarda pratik bir şekilde kullanabilirsiniz.

#### 🤖 Yapay Zeka (AI) API Seçenekleri
**1. Puter AI — 
* [Puter.com](https://puter.com) adresine gidin ve ücretsiz bir hesap oluşturun.
* Hesabınıza giriş yaptıktan sonra geliştirici paneli üzerinden API anahtarınızı (API key) oluşturun.
* Puter AI, oyun diyaloglarının bağlamını çok iyi anlayan ve oldukça doğal hissettiren çeviriler sunan cömert limitlere sahip bir yapay zekadır.
  
**2. Google Gemini AI — Alternatif**
* [Google AI Studio](https://aistudio.google.com) adresine gidin ve Google hesabınızla giriş yapın.
* Sol menüden **"Get API key"** (API anahtarı al) seçeneğine tıklayın ve yeni bir anahtar oluşturun.
* Gemini, karmaşık oyun metinlerini çok daha hızlı ve akıllı bir şekilde analiz ederek mükemmel hikaye çevirileri sunar.

### 📝 4. Aşama: API Anahtarları Nereye Girilecek?
Aldığınız API anahtarlarını uygulamaya tanıtmak için aşağıdaki iki yöntemden birini tercih edebilirsiniz:
* **Yöntem 1 (Switch Üzerinden):** Hbmenu üzerinden TranslateNX uygulamasına girerek API anahtarlarınızı doğrudan uygulama arayüzünden ilgili yerlere yazabilirsiniz.
* **Yöntem 2 (Bilgisayar Üzerinden - Pratik Yol):** Switch'inizi bilgisayarınıza bağlayın. `SD:/config/translate/config.ini` dosyasını bilgisayarınızda bir metin belgesi olarak açıp API anahtarlarını gerekli yerlere yapıştırın, kaydedin ve dosyayı tekrar Switch'e atın.

### 🎮 5. Aşama: Uygulamanın Kullanımı
1. **UltraHand'i Açın:** Parmağınızı ekranın sol kenarından sağa doğru kaydırarak veya **L + R + D-Pad Aşağı + Sağ Analog (R-Stick)** kombinasyonuna basarak UltraHand arayüzünü çağırın.
2. **TranslateNX'i Başlatın:** Listeden Translate seçeneğinin üzerine gelin ve uygulamayı açın. *(İpucu: Üzerindeyken Y tuşuna basarak hızlı erişim için kısayol atayabilirsiniz).*
3. **Ayarları Yapılandırın:** Ayarlar bölümüne girin. Aldığınız OCR ve Çeviri API'lerini seçin.
4. **Dilleri Belirleyin:**
   * **Kaynak Dil:** Oynadığınız oyunun orijinal dili.
   * **Hedef Dil:** Çevirinin yapılmasını istediğiniz kendi diliniz.
5. **Çeviriye Başlayın:** Oyunda çevirmek istediğiniz bir metin ekrandayken TranslateNX arayüzünü açın ve **"Çeviriye Başla"** butonuna basın.
*(Not: İşlem ilk seferinde biraz yavaş olabilir, çeviri hızı kullandığınız API'ye ve internet bağlantınıza göre değişiklik gösterecektir).*

---

## 🔗 İletişim ve Bağış

### SertAy

| Linkler | QR Kod |
| :--- | :--- |
| **Tüm Linkler:** [Linktree Sayfam](https://linktr.ee/yamanx) | <a href="https://linktr.ee/yamanx"><img src="assets/qr_SertAyTumLinkler.png" width="120"/></a> |

---

## 📄 License / Lisans

Telif Hakkı — © 2026 **SertAy**.  
Bu proje kişisel ve ticari olmayan kullanım için açıktır. Projenin kaynak belirtilmeksizin paylaşılması, sahiplenilmesi veya satılması kesinlikle yasaktır. Detaylar için lütfen [LICENSE](LICENSE) dosyasını inceleyiniz.

Copyright (c) 2026 **SertAy**.  
This project is available for personal and non-commercial use with mandatory author attribution. Claiming authorship, unauthorized redistribution, or selling this software is strictly prohibited. Please see the [LICENSE](LICENSE) file for details.
