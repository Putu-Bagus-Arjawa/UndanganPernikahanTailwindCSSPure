# Set nama (sesuai nama GitHub)
git config --global user.name "NamaKamu"

# Set email (pakai email GitHub)
git config --global user.email "emailkamu@example.com"

# Cek udah bener belum
git config --list

buat folder baru, buka di vscode, lalu buka git bash

# Clone repo 
git clone https://github.com/Putu-Bagus-Arjawa/UndanganPernikahanTailwindCSSPure.git

# Install dependency
npm install

# Pastikan mulai dari branch development
git checkout development

# Update branch local
git pull origin development

# Buat branch baru (ganti 'nama-page' sesuai halaman)
git checkout -b page/nama-page

# Jalanin tailwindcss
npx @tailwindcss/cli -i ./src/input.css -o ./src/output.css --watch
# pas sudah buat dan mau ngirim

# Cek perubahan apa aja yang belum di-add 
git status

# Tambahkan semua file yang diubah
git add .

# Atau tambahkan file spesifik 
git add nama-file.html

# Commit perubahan (deskripsi harus jelas perubahannya apa) 
git commit -m "feat: add homepage layout"

# Push branch pertama kali
git push -u origin page/nama-page

# Kalau udah pernah push sebelumnya
git push