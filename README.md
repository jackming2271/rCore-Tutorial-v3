通过了lab3 的test_case
输出如下:



(rustup target list | grep "riscv64gc-unknown-none-elf (installed)") || rustup target add riscv64gc-unknown-none-elf
riscv64gc-unknown-none-elf (installed)
cargo install cargo-binutils
rustup component add rust-src
rustup component add llvm-tools-preview
[build.py] application 00power_3 start with address 0x80400000
[build.py] application 01power_5 start with address 0x80420000
[build.py] application 02power_7 start with address 0x80440000
[build.py] application 03sleep start with address 0x80460000
[build.py] application 04ch3_0_sleep start with address 0x80480000
[build.py] application 05ch3_0_sleep1 start with address 0x804a0000
[build.py] application 06ch3_1_yield0 start with address 0x804c0000
[build.py] application 07ch3_1_yield1 start with address 0x804e0000
[build.py] application 08ch3_1_yield2 start with address 0x80500000
[build.py] application 09ch3_0_setprio start with address 0x80520000
[build.py] application 10ch3t_deadloop start with address 0x80540000
[build.py] application 11ch3_2_stride0 start with address 0x80560000
[build.py] application 12ch3_2_stride1 start with address 0x80580000
[build.py] application 13ch3_2_stride2 start with address 0x805a0000
[build.py] application 14ch3_2_stride3 start with address 0x805c0000
[build.py] application 15ch3_2_stride4 start with address 0x805e0000
[build.py] application 16ch3_2_stride5 start with address 0x80600000
rust-objcopy --binary-architecture=riscv64 target/riscv64gc-unknown-none-elf/release/00power_3 --strip-all -O binary  target/riscv64gc-unknown-none-elf/release/00power_3.bin;  rust-objcopy --binary-architecture=riscv64 target/riscv64gc-unknown-none-elf/release/01power_5 --strip-all -O binary  target/riscv64gc-unknown-none-elf/release/01power_5.bin;  rust-objcopy --binary-architecture=riscv64 target/riscv64gc-unknown-none-elf/release/02power_7 --strip-all -O binary  target/riscv64gc-unknown-none-elf/release/02power_7.bin;  rust-objcopy --binary-architecture=riscv64 target/riscv64gc-unknown-none-elf/release/03sleep --strip-all -O binary  target/riscv64gc-unknown-none-elf/release/03sleep.bin;  rust-objcopy --binary-architecture=riscv64 target/riscv64gc-unknown-none-elf/release/04ch3_0_sleep --strip-all -O binary  target/riscv64gc-unknown-none-elf/release/04ch3_0_sleep.bin;  rust-objcopy --binary-architecture=riscv64 target/riscv64gc-unknown-none-elf/release/05ch3_0_sleep1 --strip-all -O binary  target/riscv64gc-unknown-none-elf/release/05ch3_0_sleep1.bin;  rust-objcopy --binary-architecture=riscv64 target/riscv64gc-unknown-none-elf/release/06ch3_1_yield0 --strip-all -O binary  target/riscv64gc-unknown-none-elf/release/06ch3_1_yield0.bin;  rust-objcopy --binary-architecture=riscv64 target/riscv64gc-unknown-none-elf/release/07ch3_1_yield1 --strip-all -O binary  target/riscv64gc-unknown-none-elf/release/07ch3_1_yield1.bin;  rust-objcopy --binary-architecture=riscv64 target/riscv64gc-unknown-none-elf/release/08ch3_1_yield2 --strip-all -O binary  target/riscv64gc-unknown-none-elf/release/08ch3_1_yield2.bin;  rust-objcopy --binary-architecture=riscv64 target/riscv64gc-unknown-none-elf/release/09ch3_0_setprio --strip-all -O binary  target/riscv64gc-unknown-none-elf/release/09ch3_0_setprio.bin;  rust-objcopy --binary-architecture=riscv64 target/riscv64gc-unknown-none-elf/release/10ch3t_deadloop --strip-all -O binary  target/riscv64gc-unknown-none-elf/release/10ch3t_deadloop.bin;  rust-objcopy --binary-architecture=riscv64 target/riscv64gc-unknown-none-elf/release/11ch3_2_stride0 --strip-all -O binary  target/riscv64gc-unknown-none-elf/release/11ch3_2_stride0.bin;  rust-objcopy --binary-architecture=riscv64 target/riscv64gc-unknown-none-elf/release/12ch3_2_stride1 --strip-all -O binary  target/riscv64gc-unknown-none-elf/release/12ch3_2_stride1.bin;  rust-objcopy --binary-architecture=riscv64 target/riscv64gc-unknown-none-elf/release/13ch3_2_stride2 --strip-all -O binary  target/riscv64gc-unknown-none-elf/release/13ch3_2_stride2.bin;  rust-objcopy --binary-architecture=riscv64 target/riscv64gc-unknown-none-elf/release/14ch3_2_stride3 --strip-all -O binary  target/riscv64gc-unknown-none-elf/release/14ch3_2_stride3.bin;  rust-objcopy --binary-architecture=riscv64 target/riscv64gc-unknown-none-elf/release/15ch3_2_stride4 --strip-all -O binary  target/riscv64gc-unknown-none-elf/release/15ch3_2_stride4.bin;  rust-objcopy --binary-architecture=riscv64 target/riscv64gc-unknown-none-elf/release/16ch3_2_stride5 --strip-all -O binary  target/riscv64gc-unknown-none-elf/release/16ch3_2_stride5.bin;
Platform: qemu
[rustsbi] RustSBI version 0.2.0-alpha.1
.______       __    __      _______.___________.  _______..______   __
|   _  \     |  |  |  |    /       |           | /       ||   _  \ |  |
|  |_)  |    |  |  |  |   |   (----`---|  |----`|   (----`|  |_)  ||  |
|      /     |  |  |  |    \   \       |  |      \   \    |   _  < |  |
|  |\  \----.|  `--'  |.----)   |      |  |  .----)   |   |  |_)  ||  |
| _| `._____| \______/ |_______/       |__|  |_______/    |______/ |__|

[rustsbi] Platform: QEMU (Version 0.2.0)
[rustsbi] misa: RV64ACDFIMSU
[rustsbi] mideleg: 0x222
[rustsbi] medeleg: 0xb1ab
[rustsbi-dtb] Hart count: cluster0 with 1 cores
[rustsbi] Kernel entry: 0x80200000
[kernel] Hello, world!
power_3 [10000/200000]
power_3 [20000/200000]
power_3 [30000/200000]
power_3 [40000/200000]
power_3 [50000/200000]
power_3 [60000/200000]
power_3 [70000/200000]
power_3 [80000/200000]
power_3 [90000/200000]
power_3 [100000/200000]
power_3 [110000/200000]
power_3 [120000/200000]
power_3 [130000/200000]
power_3 [140000/200000]
power_3 [150000/200000]
power_3 [160000/200000]
power_3 [170000/200000]
power_3 [180000/200000]
power_3 [190000/200000]
power_3 [200000/200000]
3^200000 = 871008973
Test power_3 OK!
[kernel] Application exited with code 0
power_5 [10000/140000]
power_5 [20000/140000]
power_5 [30000/140000]
power_5 [40000/140000]
power_5 [50000/140000]
power_5 [60000/140000]
power_5 [70000/140000]
power_5 [80000/140000]
power_5 [90000/140000]
power_5 [100000/140000]
power_5 [110000/140000]
power_5 [120000/140000]
power_5 [130000/140000]
power_5 [140000/140000]
5^140000 = 386471875
Test power_5 OK!
[kernel] Application exited with code 0
power_7 [10000/160000]
power_7 [20000/160000]
power_7 [30000/160000]
power_7 [40000/160000]
power_7 [50000/160000]
power_7 [60000/160000]
power_7 [70000/160000]
power_7 [80000/160000]
power_7 [90000/160000]
power_7 [100000/160000]
power_7 [110000/160000]
power_7 [120000/160000]
power_7 [130000/160000]
power_7 [140000/160000]
power_7 [150000/160000]
power_7 [160000/160000]
7^160000 = 667897727
Test power_7 OK!
[kernel] Application exited with code 0
get_time OK! 50
current time_msec = 51
AAAAAAAAAA [1/5]
AAAAAAAAAA [2/5]
BBBBBBBBBB [1/5]
BBBBBBBBBB [2/5]
CCCCCCCCCC [1/5]
SET priority : before[16] , after[10000]
SET priority : before[10000] , after[0]
Test set_priority OK!
[kernel] Application exited with code 0
[kernel] Application exited with code -2141974672
~~~~~~~~~~~~~~~~~~~~~~~~~
SET priority : before[16] , after[20000]
SET priority : before[16] , after[16666]
SET priority : before[16] , after[14285]
SET priority : before[16] , after[12500]
SET priority : before[16] , after[11111]
SET priority : before[16] , after[10000]
time_msec = 194 after sleeping 100 ticks, delta = 143ms!
Test sleep1 passed!
[kernel] Application exited with code 0
AAAAAAAAAA [3/5]
AAAAAAAAAA [4/5]
BBBBBBBBBB [3/5]
BBBBBBBBBB [4/5]
CCCCCCCCCC [2/5]
CCCCCCCCCC [3/5]
CCCCCCCCCC [4/5]
AAAAAAAAAA [5/5]
Test write A OK!
[kernel] Application exited with code 0
BBBBBBBBBB [5/5]
Test write B OK!
[kernel] Application exited with code 0
CCCCCCCCCC [5/5]
Test write C OK!
[kernel] Application exited with code 0
priority = 5, exitcode = 2118400
[kernel] Application exited with code 0
priority = 6, exitcode = 2898800
[kernel] Application exited with code 0
priority = 7, exitcode = 3416000
[kernel] Application exited with code 0
priority = 8, exitcode = 3854400
[kernel] Application exited with code 0
priority = 9, exitcode = 4866400
[kernel] Application exited with code 0
priority = 10, exitcode = 5954400
[kernel] Application exited with code 0
Test sleep OK!
[kernel] Application exited with code 0
Test sleep OK!
[kernel] Application exited with code 0
[kernel] Panicked at src/task/mod.rs:138 All applications completed!
