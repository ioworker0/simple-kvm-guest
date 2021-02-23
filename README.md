# simple-kvm-guest
一个简单KVM用户空间实例

```sh
make -C guest
```

```sh
gcc kvm.c -o kvm
```

```sh
./kvm
```

```sh
pidstat -p `pidod kvm` 1
```

```sh
08:34:49 PM   UID       PID    %usr %system  %guest    %CPU   CPU  Command
08:34:50 PM     0      3655    0.00    0.00  100.00  100.00     1  kvm
08:34:51 PM     0      3655    0.00    0.00  100.00  100.00     1  kvm
08:34:52 PM     0      3655    0.00    0.00  100.00  100.00     1  kvm
```
