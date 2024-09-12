# sectorlisp fork for kvm

Fork of sectorlisp with minor adjustments to allow easy use with KVM. Specifically:

- IO via BIOS functions (`int 0x10 and int 0x16`) are replaced with IO over an IO port.
- Paritition table is removed

This allows kvm to interact with a sectorlisp loaded into a specific location in memory without including a BIOS.

For more information, see the [description of sectorlisp](https://github.com/jart/sectorlisp) at the original repo.
For context, see [kvm_sectorlisp](https://github.com/BolunThompson/kvm_sectorlisp).
