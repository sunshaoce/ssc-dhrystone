# benchmark-dhrystone
"DHRYSTONE" Benchmark Program by  Reinhold P. Weicker

## RUN

On RISC-V CPU:
```shell
CC=clang CFLAGS=-march=rv64gcv make run
```

On X86 cross-compile:
```shell
CC=riscv64-unknown-linux-gnu-clang CFLAGS=-march=rv64gcv make
qemu-riscv64 -L $RISCV_LINUX/sysroot ./dhrystone
```
