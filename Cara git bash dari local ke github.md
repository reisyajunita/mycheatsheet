## CARA GIT BASH KE REPO GITHUB dalam bentuk folder
- git init (kalo foldernya blm pernah di bash)
- git remote add origin (link repo GitHub)  [kalo salah bisa hapus (git remote remove origin])
- git pull origin MASUKIN NAMA BRANCHnya misal main --allow-unrelated-histories (misal nama pathnya masih [master] bisa pake git checkout (nama branch yang mau dipake)
- git add .
- git commit -m "bebas diisi apa sesuaiin aja" (copy key, commit message)
- git push -u origin main (nama branch)


## hapus git init
rm -rf .git

## Cara lain
- git init (Inisialisasi repositori)
- git add . (Pilih file yang mau disimpan)
- git commit -m "Pesan commit" (Simpan file tersebut dengan sebuah pesan)
- git branch -M main (Ubah nama branch)
- git remote add origin <URL> (Hubungkan ke GitHub)
- git push -u origin main (Kirim ke GitHub)

## Cara biar folder env ga ikut ke bash
- buat file .gitignore
- isi filenya dengan nama folder env, misal env_ml
- save deh, nanti pas ke bash file .gitignorenya juga ke up tapi folder env_ml nya engga.
