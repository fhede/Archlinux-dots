Custom kernel 6.5.0-linux-FH slimmed from modules with modprobed-db and compiled against intel nuc 13 1340P i5.

Working for kvm,qemu,multimedia,intel.
Performance governor is set.
300 Hz timer x 16 cores

Testing the preempt that opensuse use with very high responsivness.
sudo dmesg | grep -i preempt
Linux version 6.5.0-linux-FH (fred@nuc13) (gcc (GCC) 13.2.1 20230801, GNU ld (GNU Binutils) 2.41.0) #8 SMP PREEMPT_DYNAMIC Thu Aug 31 16:56:07 CEST 2023
Dynamic Preempt: voluntary
rcu: Preemptible hierarchical RCU implementation.
Dynamic Preempt: full

Made for for intel nuc.

152 modules currently loaded per /proc/modules
167 modules are in /home/fred/.config/modprobed.db

With graysky patch(raptorlake) https://github.com/graysky2/kernel_compiler_patch compile times.
real 4m50.813s user 56m28.817s sys 5m5.505s

I also use system76cheduler from archlinux testing.

Fastest kernel ever for me with no glithces and very high responsivness.
