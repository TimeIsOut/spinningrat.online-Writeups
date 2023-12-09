# Italian mails(Origins)
## Writeup Author - h1tok1r11

---

### Task

Enzo Tommasi was a YouTube "superstar" in Italy. He went viral with this video initially and then with many others. Can you find out where he was in this epic clip?
Video(https://www.youtube.com/watch?v=rNta7FLxq8s)
Flag format: hctf{street_name_number}

---

### Solution

The first thing that came to my mind was to type **Enzo Tommasi poste italiane** into Google. After this we can see the post on Reddit(https://www.reddit.com/r/copypastaitalia/comments/1251pyq/enzo_tomasi_alle_poste_lyrics/).

There are lyrics to video in which we can see **Ostia**, so we can suggest that the post office is located in Ostia. And if we type **ostia poste italiane** we will see several post offices one of which is the one we are looking for.
(../assets/adress.png)

---

### Flag

```
hctf{Via_Ferdinando_Acton_44}
```