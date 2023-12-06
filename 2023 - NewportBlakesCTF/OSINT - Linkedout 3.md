# OSINT - Linkedout 3 (420 points)
## Writeup Author: n0vac
---

### Task

Lets see your linkedin experience. There's another flag hidden somewhere, lets see if you can find it.

---
### Solution

This was referring to the profile found on Linkedout 1. I was confused at first and wondering where the flag is.
Then I looked at the link of the profile and it looked a little odd. It had hex.
```
6e626374667b4431645f7930755f537030745f31743f7d
```

I went to CyberChef, set the recipe to From Hex and put the hex as the input. And there was the flag!

---
### Flag

```
nbctf{D1d_y0u_Sp0t_1t?}
```