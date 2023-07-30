# Archlinux-dots

Welcome to try out my configs that i use on Arch linux. 

My custom kernels are compiled on a intel nuc 13 1340 i5.
And are trimmed from modules with the help of modprobed-db
to get high responsiveness.

With graysky patch(raptorlake) compile times.
real    4m50.813s
user    56m28.817s
sys     5m5.505s

I also testing clang compiler with polly and openMP.
Linux-clear is a good package to test on.
Download the package and run makepkg-clang.conf with
"makepkg  /etc/makepkg-clang.conf" or 

Install LLVM
git clone https://aur.archlinux.org/llvm-git
cd llvm-git
makepkg -sric --config /etc/makepkg-clang.conf
