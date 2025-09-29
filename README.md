## 🌱 ESP32 Tabanlı Akıllı Sera Kontrol Sistemi ##
## 📌 ESP32 Hakkında

ESP32, Espressif Systems tarafından geliştirilen, düşük maliyetli ve yüksek performanslı bir mikrodenetleyici kartıdır. Dahili Wi-Fi ve Bluetooth desteği sayesinde IoT projelerinde sıklıkla kullanılmaktadır.
ESP32’nin başlıca özellikleri:

🔹Çift çekirdekli 32-bit işlemci
🔹2.4 GHz Wi-Fi ve Bluetooth/BLE desteği
🔹Çok sayıda dijital/analog giriş çıkış pinleri
🔹Düşük güç tüketimi (batarya ile uzun süreli kullanım için uygun)
🔹Geniş topluluk ve kütüphane desteği
🔹Bu proje, ESP32’nin sensör ve aktüatörlerle etkileşimini kullanarak akıllı bir sera otomasyonu gerçekleştirmektedir.

## 🎯 Projenin Amacı

Tarımda verimliliği artırmak ve insan müdahalesini azaltmak amacıyla sera ortamının sıcaklık, nem, ışık ve CO₂ seviyelerinin otomatik kontrol edilmesi hedeflenmiştir.
Sistem, gerektiğinde manuel butonlarla da kontrol edilebilir.

## ⚙️ Kullanılan Donanım ve Modüller

● ESP32 Geliştirme Kartı → Projenin merkezi kontrol birimi

● DHT22 (Sıcaklık & Nem Sensörü) → Ortam sıcaklığı ve nem ölçümü

● MQ-135 (CO₂ Sensörü) → Karbondioksit seviyesini ölçme

● LDR (Işık Sensörü) → Ortam ışık seviyesini algılama

● 16x4 I2C LCD Ekran → Sistem verilerini kullanıcıya gösterme

● Fan → Yüksek sıcaklık veya yüksek CO₂ durumunda devreye girme

● Su Pompası → Düşük nem seviyesinde sulama yapma

● LED Aydınlatma → Yetersiz ışık veya gece koşullarında bitkileri aydınlatma

● Buzzer → Kritik durumlarda (ör. düşük CO₂) kullanıcıyı uyarma

● Butonlar → Manuel fan ve pompa kontrolü

## 🛠️ Çalışma Prensibi

🔻Sıcaklık & Nem Kontrolü
 •Nem %40’ın altına düştüğünde pompa otomatik devreye girer.

 •Sıcaklık 30°C’nin üzerine çıktığında fan otomatik çalışır.

🔻CO₂ Seviyesi
•MQ-135 sensöründen alınan veri belirlenen eşik değerine göre kontrol edilir.
•CO₂ değeri yüksekse fan devreye girer, düşükse buzzer ile kullanıcı uyarılır.

🔻Işık Kontrolü

•Ortam ışığı yetersizse veya saat 18:00 sonrası/gün doğmadan önce LED aydınlatma aktif olur.

🔻Manuel Kontrol

•Kullanıcı butonlar yardımıyla fan veya pompayı manuel olarak açıp kapatabilir.

🔻LCD Gösterge

•Anlık sıcaklık, nem, CO₂ değeri, fan ve pompa durumları ekranda gösterilir.

## 📊 Proje Çıktısı ve İşlevsellik

Bu sistem sayesinde:

  •Otomatik iklimlendirme yapılır.
  •Bitki büyümesi için ideal koşullar sağlanır.
  •Gereksiz enerji ve su tüketiminin önüne geçilir.
  •Manuel kontrol butonları ile kullanıcı her zaman müdahale edebilir.
  •LCD ekran üzerinden gerçek zamanlı veriler takip edilebilir.

## ✅ Sonuç
ESP32 tabanlı akıllı sera kontrol sistemi, tarımsal üretimde otomasyon, enerji verimliliği ve sürdürülebilirlik açısından önemli bir katkı sağlar.
Sensörlerden alınan veriler doğrultusunda sera ortamı sürekli olarak denetlenir ve otomatik müdahaleler yapılır. Bu sayede, ürün kalitesi ve verimlilik artışı sağlanır.
