# Crypto - Caesar Salads (100 points)
## Writeup Author: GameIsOn
---

### Task
Every CTF needs an introductory crypto. I found a roman emperor that made this super cool cipher. Can you decrypt this for me?

Attached files:
```
-- output.txt
```

**output.txt**:
```
Ciphertext: xlmdp{ryzo_drsc_gkcxd_dyy_rkbn_yp_k_cdkbd}
```
---
### Solution

'A roman emperor', which was mentioned in the task, is Julius Caesar. The ciphertext is encoded with the Caesar cipher, which was named after him. Placing the ciphertext in the Cyberchef with the decryption settings _ROT13 (Amount = 16)_ will result in our flag.

---
### Flag

```
nbctf{hope_this_wasnt_too_hard_of_a_start}
```
