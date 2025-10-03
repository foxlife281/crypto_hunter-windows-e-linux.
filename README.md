
 # 🧠 Crypto Hunter – Windows e Linux

Ferramenta para busca de chaves e endereços Bitcoin por força bruta utilizando modos **address** e **BSGS**.

---

## 📦 Windows – Exemplos de uso

```bash
crypto_hunter -m address -f tests/71.txt -t 24 -l compress -6 -S -e -r 400000000000000000:7fffffffffffffffff -n 1024

crypto_hunter -m bsgs -t 24 -f tests/135.txt -k 4096 -6 -S -e 4000000000000000000000000000000000:7fffffffffffffffffffffffffffffffff

./crypto_hunter -m address -f tests/71.txt -t 24 -l compress -6 -S -e -r 400000000000000000:7fffffffffffffffff -n 1024

./crypto_hunter -m bsgs -t 24 -f tests/135.txt -k 4096 -6 -S -e 4000000000000000000000000000000000:7fffffffffffffffffffffffffffffffff

| RAM    | Parâmetros recomendados        |
| ------ | ------------------------------ |
| 2 GB   | `-k 128`                       |
| 4 GB   | `-k 256`                       |
| 8 GB   | `-k 512`                       |
| 16 GB  | `-k 1024`                      |
| 32 GB  | `-k 2048`                      |
| 64 GB  | `-n 0x100000000000 -k 4096`    |
| 128 GB | `-n 0x400000000000 -k 4096`    |
| 256 GB | `-n 0x400000000000 -k 8192`    |
| 512 GB | `-n 0x1000000000000 -k 8192`   |
| 1 TB   | `-n 0x1000000000000 -k 16384`  |
| 2 TB   | `-n 0x4000000000000 -k 16384`  |
| 4 TB   | `-n 0x4000000000000 -k 32768`  |
| 8 TB   | `-n 0x10000000000000 -k 32768` |
