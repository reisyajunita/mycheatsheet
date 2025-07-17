## CARA GIT BASH KE REPO GITHUB dalam bentuk folder
- git init (kalo foldernya blm pernah di bash)
- git remote add origin (link repo GitHub)  [kalo salah bisa hapus (git remote remove origin])
- git pull origin MASUKIN NAMA BRANCHnya misal main --allow-unrelated-histories (misal nama pathnya masih [master] bisa pake git checkout (nama branch yang mau dipake)
- git add .
- git commit -m "bebas diisi apa sesuaiin aja" (copy key, commit message)
- git push -u origin main (nama branch)


## hapus git init
rm -rf .git
