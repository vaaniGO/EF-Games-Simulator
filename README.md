I was studying a little bit of FOL and a little bit of Descriptive Complexity, which led me to FOL with Least Fixed Points. Now, to show that a property is definable in FOL is fairly straightforward – we can give the sentence. But, to show that a sentence is *not* definable in FOL seems more challenging. For that, we have Ehrenfeucht-Fraïssé games. Similarly, for showing non-expressibility of a property in L^k∞ω: infinitary logic, we have pebble games. 

A resource I liked for 
1. EF-Games: https://pi.math.cornell.edu/~mec/Summer2009/Raluca/lesson1.html
2. Pebble Games: https://www.youtube.com/watch?v=IMsxnPnylSw&t=1543s

The site is live at https://vaanigo.github.io/EF-Games-Simulator/

## To run locally

Open `index.html` in a browser. To serve it the same way GitHub Pages does:

```bash
python3 -m http.server 8000
```

Then visit http://localhost:8000.

## Credits

The overview of EF games on the page is adapted from the [Cornell Math Explorers' Club lesson on Ehrenfeucht–Fraïssé games](https://pi.math.cornell.edu/~mec/Summer2009/Raluca/lesson1.html).
