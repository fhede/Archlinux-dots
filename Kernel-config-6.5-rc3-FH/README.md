Custom kernel slimmed from modules with modprobed-db and compiled against intel nuc 13 1340P i5.

No support for kvm,zen,qemu,multimedia,amd
Only support for intel nuc.

:Testing
Add CONFIG_PREEMPT_DYNAMIC: this in its current form adds the
preempt=none/voluntary/full boot options (default: full),
to allow distros to build a PREEMPT kernel but fall back to
close to PREEMPT_VOLUNTARY (or PREEMPT_NONE) runtime scheduling
behavior via a boot time selection.

grub_commandline preempt=full

sudo dmesg | grep Preempt
Dynamic Preempt: voluntary
rcu: Preemptible hierarchical RCU implementation.
Dynamic Preempt: full

system76-scheduler seems to enable same thing in the config
