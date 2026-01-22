GitHub'a Proje Yükleme Adımları

1. GitHub'da Yeni Repository Oluşturma

   - GitHub.com'a giriş yapın
   - Sağ üstteki "+" butonuna tıklayın
   - "New repository" seçin
   - Repository adı: "shadow_puzzle" (veya istediğiniz isim)
   - Public veya Private seçin
   - "Initialize this repository with a README" seçeneğini İŞARETLEMEYİN (zaten README var)
   - "Create repository" butonuna tıklayın

2. Terminal Komutları

   Proje klasöründe şu komutları sırayla çalıştırın:

   ```bash
   # Tüm dosyaları staging area'ya ekle
   git add .

   # İlk commit'i yap
   git commit -m "Initial commit: Shadow Puzzle Game"

   # GitHub repository URL'ini ekle (kendi URL'inizi kullanın)
   git remote add origin https://github.com/KULLANICI_ADINIZ/shadow_puzzle.git

   # Ana branch'i main olarak ayarla
   git branch -M main

   # GitHub'a yükle
   git push -u origin main
   ```

3. Alternatif: SSH Kullanımı

   Eğer SSH kullanıyorsanız:
   ```bash
   git remote add origin git@github.com:KULLANICI_ADINIZ/shadow_puzzle.git
   git push -u origin main
   ```

Notlar:
- KULLANICI_ADINIZ yerine kendi GitHub kullanıcı adınızı yazın
- İlk push'ta GitHub kullanıcı adı ve şifre (veya Personal Access Token) isteyebilir
- Eğer 2FA (Two-Factor Authentication) açıksa, Personal Access Token kullanmanız gerekir

