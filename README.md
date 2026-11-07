# minitalk

![C](https://img.shields.io/badge/C-A8B9CC?style=flat-square&logo=c&logoColor=white) ![UNIX signals](https://img.shields.io/badge/UNIX_signals-555555?style=flat-square) ![42 Roma Luiss](https://img.shields.io/badge/42_Roma_Luiss-000000?style=flat-square&logo=42&logoColor=white)

A client and server that talk using only two UNIX signals. The client sends each character bit by bit, with `SIGUSR1` for 0 and `SIGUSR2` for 1. The server puts the bits back together and prints the message.

## Build & run

```bash
make
./server                 # prints its PID
./client <PID> "Hello from minitalk"
```

Built on `sigaction`, `kill` and my own [`ft_printf`](https://github.com/Fbiondo00/printf).

---

<sub>Part of my 42 Roma Luiss curriculum · [more projects](https://github.com/Fbiondo00) · MIT License</sub>
