## CARA GIT BASH KE REPO GITHUB dalam bentuk folder
- git init (kalo foldernya blm pernah di bash)
- git remote add origin (link repo GitHub)  [kalo salah bisa hapus (git remote remove origin])
- git pull origin MASUKIN NAMA BRANCHnya misal main --allow-unrelated-histories (misal nama pathnya masih [master] bisa pake git checkout (nama branch yang mau dipake)
- git add .
- git commit -m "bebas diisi apa sesuaiin aja" (copy key, commit message)
- git push -u origin main (nama branch)


## hapus git init
rm -rf .git

## Cara biar folder env ga ikut ke bash
- buat file .gitignore
- isi filenya dengan nama folder env, misal env_ml
- save deh, nanti pas ke bash file .gitignorenya juga ke up tapi folder env_ml nya engga.

## Cara lain
### First bash
- git init
- git remote add origin [link repo]
- git add .
- git commit -m "first commit"
- git branch -M main (misal nama branchnya beda [master] jadi ganti dulu ke main)
- git push -u origin main

### Bash ketika upload file baru
- git add .
- git commit -m "Memperbaiki bug di file X"
- git push
