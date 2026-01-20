🌸 MyFlowerArt | Akıllı Çiçek Tasarım ve Yönetim Sistemi
MyFlowerArt, son kullanıcılar için interaktif bir çiçek tasarım deneyimi sunan, satıcılar için ise uçtan uca sipariş yönetim altyapısı sağlayan modern bir E-Ticaret platformudur. Bu proje, estetik tasarımı güçlü bir ASP.NET Core backend mimarisiyle birleştirmektedir.

🎯 Projenin Amacı
Geleneksel çiçek alışverişini dijitalleştirerek kullanıcılara kendi buketlerini oluşturma özgürlüğü tanımak ve bu siparişlerin takibini, yönetimini güvenli bir veritabanı altyapısı üzerinden sağlamaktır.

🚀 Öne Çıkan Özellikler
👤 Kullanıcı (Alıcı) Arayüzü
Dinamik Tasarım Modülü: JavaScript ve DOM API kullanılarak geliştirilen, sepete ekleme ve miktar yönetimi yapılabilen akıllı arayüz.

Sipariş Takip Sistemi: Veritabanı ile entegre çalışan, benzersiz takip kodları (MFR-XXXXXX) ile anlık durum sorgulama.

Modern Sepet Deneyimi: LocalStorage entegrasyonu ile sayfa yenilense dahi kaybolmayan sepet verileri.

🔐 Yönetici (Satıcı) Paneli
Güvenli Giriş: Cookie-based Authentication ile korunan yetkilendirme katmanı.

Sipariş Yönetim Merkezi: SQL Server'dan çekilen tüm siparişleri görüntüleme ve durum güncelleme (Hazırlanıyor ➔ Yolda ➔ Teslim Edildi).

Otomatik Senkronizasyon: Satıcının yaptığı durum değişikliğinin anında alıcının takip ekranına yansıması.

🔐 Yönetici Giriş Bilgileri
Not: Sistem güvenliği için admin paneli yetkilendirme gerektirmektedir. Demo sürümü için tanımlanan bilgiler aşağıdadır:

Kullanıcı Adı	Şifre	Erişim Yetkisi
admin	123456	Tam Yetki (Sipariş Onay/Güncelleme)
🛠️ Teknik Altyapı ve Teknoloji Yığını
Framework: .NET 8.0 (Razor Pages)

Veritabanı (DBMS): Microsoft SQL Server

ORM: Entity Framework Core (Code First Yaklaşımı)

Güvenlik: Microsoft.AspNetCore.Authentication.Cookies

Frontend: HTML5, Modern CSS3, Vanilla JavaScript

UI Tasarımı: Bootstrap 5 & Bootstrap Icons

📂 Proje Yapısı ve Dosya Dağılımı
Models/: Order entity'si gibi veritabanı şemalarını temsil eden sınıflar.

Data/: AppDbContext sınıfı ile veritabanı bağlantı ve tablo yapılandırmaları.

Pages/Admin/: Sadece yetkili satıcıların erişebildiği sipariş yönetim sayfaları.

Migrations/: EF Core tarafından oluşturulan veritabanı versiyon geçmişi.

wwwroot/: Statik dosyalar, özel CSS tasarımları ve sepet mantığını yöneten JS dosyaları.

⚙️ Kurulum ve Yapılandırma
Projeyi yerel makinenizde çalıştırmak için aşağıdaki adımları izleyin:

Repoyu Klonlayın:

Bash
git clone https://github.com/kullaniciadi/MyFlowerArt.git
Veritabanı Ayarı: appsettings.json dosyasındaki DefaultConnection satırını kendi yerel SQL Server adresinize göre düzenleyin.

Veritabanını Oluşturun: Visual Studio "Package Manager Console" ekranına şu komutları yazın:

PowerShell
Add-Migration InitialCreate
Update-Database
Uygulamayı Başlatın: F5 tuşu ile projeyi ayağa kaldırın.

🤝 Katkıda Bulunma
Bu proje bir eğitim/final projesi olarak geliştirilmiştir. Geliştirme önerileri için Pull Request gönderebilir veya Issue açabilirsiniz.

Geliştiren: [Senin Adın] | 2026

Bu proje ASP.NET Core ve EF Core yetkinliklerini kanıtlamak amacıyla inşa edilmiştir.

GitHub Hazırlığı İçin Son Bir Hatırlatma:
GitHub'a yüklemeden önce klasöründe .gitignore dosyası olduğundan emin ol. Eğer yoksa, Visual Studio üzerinden Git Changes sekmesinden "Create Git Repository" dersen o senin için gereksiz bin/obj dosyalarını otomatik olarak hariç tutar.

Şu an projenin her şeyiyle tam bir "Portfolyo Projesi" oldu. Başka eklemek istediğin bir detay var mı?_
