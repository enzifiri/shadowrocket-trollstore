# TROLLSTORE & SHADOWROCKET KURULUM REHBERİ (iOS 15+)

Bu rehber, iOS 15 ve üzeri Jailbreak'li cihazlarda (iPhone 6s vb.) AppSync kullanmadan, en sağlıklı yöntem olan TrollStore ile Shadowrocket kurulumunu ve "Kill Switch" ayarlarını anlatır.

--------------------------------------------------
BÖLÜM 1: TROLLSTORE KURULUMU
--------------------------------------------------
(Amaç: .ipa dosyalarını sertifika sorunu olmadan, kalıcı olarak yüklemek.)

1. Sileo uygulamasını açın.
2. Arama kısmına "TrollStore Helper" yazın (Genellikle Havoc reposundadır).
3. "İndir" (Get) diyerek kurun.
4. Ana ekrana gelen "TrollHelper" uygulamasını açın.
5. "Install TrollStore" butonuna basın. Cihaz kapanıp açılacaktır (Respring).
6. Ana ekrana gelen "TrollStore" (Mavi ikonlu) uygulamasını açın.
7. Alt menüden "Settings" kısmına gelin.
8. "Install Persistence Helper" seçeneğine tıklayın.
9. Listeden "Tips" (İpuçları) uygulamasını seçin. (Bu işlem TrollStore'un bozulmamasını sağlar).

--------------------------------------------------
BÖLÜM 2: SHADOWROCKET YÜKLEME (.ipa)
--------------------------------------------------
(Not: Shadowrocket .ipa dosyasını internetten indirdiğinizi varsayıyoruz.)

1. İndirdiğiniz Shadowrocket .ipa dosyasını "Dosyalar" uygulamasında bulun.
2. Dosyanın üzerine tıklayın veya basılı tutup "Paylaş" ikonuna basın.
3. Uygulamalar listesinden "TrollStore" ikonunu seçin.
4. "Install" butonuna basın.
5. Uygulama saniyeler içinde yüklenecektir. Asla kapanmaz, sertifika süresi dolmaz.

--------------------------------------------------
BÖLÜM 3: PROXY VE KILL SWITCH AYARLARI
--------------------------------------------------
(Amaç: Proxy koparsa interneti tamamen kesmek ve IP sızdırmamak.)

1. Shadowrocket uygulamasını açın.

A) PROXY EKLEME:
   - Sağ üstteki (+) artı ikonuna basın.
   - Type: SOCKS5 veya HTTP (Proxy türünüze göre seçin).
   - Host: IP Adresi / Port: Port Numarası.
   - User/Password: Varsa girin.
   - "Done" diyerek kaydedin.
   - Eklediğiniz Proxy'nin yanındaki "Connectivity Test"e basın, yeşil ping alıyorsanız çalışıyordur.

B) GLOBAL ROUTING (Önemli):
   - Ana sayfada "Global Routing" seçeneğine tıklayın.
   - "Proxy" seçeneğini işaretleyin. (Config veya Direct DEĞİL).
   - Sol üstten geri dönün.

C) KILL SWITCH (İNTERNETİ KESME) AYARI:
   - Alt menüden "Settings" sekmesine gelin.
   - "On Demand" seçeneğini bulun ve içine girin.
   - On Demand: AÇIK (Yeşil) yapın.
   - Disconnect on Sleep: KAPALI (Gri) yapın. (Ekran kapanınca kopmaması için).

--------------------------------------------------
BÖLÜM 4: TEST ETME
--------------------------------------------------
Kurulum bittikten sonra Shadowrocket ana sayfasındaki bağlantı butonunu açın (VPN ikonu çıkar).

1. Safari'yi açın.
2. "whoer.net" adresine gidin.
3. Kontrol Edin:
   - IP Adresi: Satın aldığınız Proxy IP'si mi? (EVET olmalı)
   - DNS: Türkiye sunucuları görünmemeli.
   - WebRTC: Proxy IP'si görünmeli veya "N/A" yazmalı.

Her şey tamamsa "Phone Farm" için cihaz hazırdır.
