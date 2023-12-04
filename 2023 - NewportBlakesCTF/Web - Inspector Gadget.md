# Web - Inspector Gadget (130 points)
## Writeup Author: GameIsOn

---

### Task
While snooping around this website, inspector gadet lost parts of his flag. Can you help him find it?

inspector-gadget.chal.nbctf.com

---

### Solution

The flag on this website is split into 4 parts.

#### Flag Part 1/4

This part can be found in the title of the 'About Gadget Magnifying Glass' page.
```html
<title>Flag Part 1/4:nbctf{G00d_</title>
```

### Flag Part 2/4

On the main page there is a script tag, which holds the redirection functions, written in JS.

```html
<script>
        function openotherpage(){
            window.location.href = "Page1.html";
        }
        function opengadgetarms(){
            window.location.href = "gadgetarms.html";
        }
        function opengadgetcoat(){
            window.location.href = "gadgetcoat.html";
        }
        function opengadgethat(){
            window.location.href = "gadgethat.html";
        }
        function opengadgetskates(){
            window.location.href = "gadgetskates.html"
        }
        function opengadgetcopter(){
            window.location.href = "gadgetcopter.html"
        }
        function opengadgetmangifyingglass(){
            window.location.href="gadgetmag.html"
        }
        function opengadgetphone(){
            window.location.href="gadgetphone.html"
        }
        function getflag(){
            window.location.href="supersecrettopsecret.txt"
        }
    </script>
```

The last function looks pretty strange. Adding the /supersecrettopsecret.txt at the end of the URL:

**https://inspector-gadget.chal.nbctf.com/supersecrettopsecret.txt**

```
Flag Part 2/4:
J06_
```

---

#### Flag Part 3/4

Looking at the img tag on the main page, we can see, that attribute alt holds our part.

```html
<img src="Krooter Gadget.jpg" alt="Flag Part 3/4: D3tect1v3_">
```

#### Flag Part 4/4

One of the first things, that I checked, was the robots.txt file, which holds parts of the site, that Google can't show on the search page.

**https://inspector-gadget.chal.nbctf.com/robots.txt**

```
User-agent: *
Disallow: /mysecretfiles.html
```

Bingo!

**https://inspector-gadget.chal.nbctf.com/mysecretfiles.html**

```
You found my secret page!
Here's part of the flag for your troubles, part 4/4 G4dg3t352}
```

---

### Flag

```
nbctf{G00d_J06_D3tect1v3_G4dg3t352}
```

