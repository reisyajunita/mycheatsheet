# Cara membuat virtual environment
1. Buka folder yang mau ditambahkan venvnya, contoh cd /d/Users/Reisya/Documents/environment
2. Kalau udah masukan code ini ke terminal (python -m venv env)
3. Lalu aktifkan venv-nya, kalo langsung di vs code cek dia pakai git bash atau apa. disini aku pake git bash, ini codenya (source env_bike_sharing/Scripts/activate)


Kalo misalnya env-nya bekas yang sebelumnya trs bingung mau pindah ke venv baru caranya gini, Jika masalah masih ada, coba pastikan VS Code menggunakan interpreter yang benar:

1. Tekan Ctrl + Shift + P
2. Ketik Python: Select Interpreter
3. Pilih interpreter dari environment yang kamu buat (env/.../python.exe).
4. Restart VS Code.

# Cara bikin requirements
Pastikan kamu sudah berada di environment yang benar, lalu jalankan:
1. Pake freeze (pip freeze > requirements.txt)
2. Kalau mau ngambil package yang lagi digunain di notebook itu, bisa pake pipreqs, caranya:
	1. pip install pipreqs
	2. pipreqs . --force

P.s: Kalo isinya ga ada alias kosong berarti itu belum ada file .py jadi convert dulu file .ipynb nya jadi .py

- Caranya gini (jupyter nbconvert --to script nama_file.ipynb)

- Kalo masih error, contohnya ini: Error ini terjadi karena pipreqs mengalami masalah dengan encoding saat membaca file di folder proyek. Biasanya ini karena ada karakter yang tidak bisa diproses oleh encoding default (cp1252). Caranya gini:
(pipreqs . --force --encoding=utf8)


# Menginstall package requirements
caranya: pip install -r requirements.txt

# Cara upgrade requirements.txt
cara 1: Buka requirements.txt dan tambahkan baris berikut:
		streamlit
	Lalu jalankan:
		pip install -r requirements.txt
Cara 2: pip install --upgrade -r requirements.txt

P.s: Coba salah satu cara di atas tergantung kebutuhan kamu. Kalau mau tetap pakai versi lama tapi tambah streamlit, cara 1 lebih aman.
