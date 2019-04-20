nyc-subway-icons
================

SVG icons based on current New York City MTA subway lines.

<p>
<img src="https://unpkg.com/nyc-subway-icons@0.4.0/svg/1.svg" alt="1" width="48">
<img src="https://unpkg.com/nyc-subway-icons@0.4.0/svg/2.svg" alt="2" width="48">
<img src="https://unpkg.com/nyc-subway-icons@0.4.0/svg/3.svg" alt="3" width="48">
<img src="https://unpkg.com/nyc-subway-icons@0.4.0/svg/4.svg" alt="4" width="48">
<img src="https://unpkg.com/nyc-subway-icons@0.4.0/svg/5.svg" alt="5" width="48">
<img src="https://unpkg.com/nyc-subway-icons@0.4.0/svg/6.svg" alt="6" width="48">
<img src="https://unpkg.com/nyc-subway-icons@0.4.0/svg/6d.svg" alt="6d" width="48">
<img src="https://unpkg.com/nyc-subway-icons@0.4.0/svg/7.svg" alt="7" width="48">
<img src="https://unpkg.com/nyc-subway-icons@0.4.0/svg/7d.svg" alt="7d" width="48">
<img src="https://unpkg.com/nyc-subway-icons@0.4.0/svg/a.svg" alt="a" width="48">
<img src="https://unpkg.com/nyc-subway-icons@0.4.0/svg/c.svg" alt="c" width="48">
<img src="https://unpkg.com/nyc-subway-icons@0.4.0/svg/e.svg" alt="e" width="48">
<img src="https://unpkg.com/nyc-subway-icons@0.4.0/svg/l.svg" alt="l" width="48">
<img src="https://unpkg.com/nyc-subway-icons@0.4.0/svg/s.svg" alt="s" width="48">
<img src="https://unpkg.com/nyc-subway-icons@0.4.0/svg/b.svg" alt="b" width="48">
<img src="https://unpkg.com/nyc-subway-icons@0.4.0/svg/d.svg" alt="d" width="48">
<img src="https://unpkg.com/nyc-subway-icons@0.4.0/svg/f.svg" alt="f" width="48">
<img src="https://unpkg.com/nyc-subway-icons@0.4.0/svg/m.svg" alt="m" width="48">
<img src="https://unpkg.com/nyc-subway-icons@0.4.0/svg/n.svg" alt="n" width="48">
<img src="https://unpkg.com/nyc-subway-icons@0.4.0/svg/q.svg" alt="q" width="48">
<img src="https://unpkg.com/nyc-subway-icons@0.4.0/svg/r.svg" alt="r" width="48">
<img src="https://unpkg.com/nyc-subway-icons@0.4.0/svg/w.svg" alt="w" width="48">
<img src="https://unpkg.com/nyc-subway-icons@0.4.0/svg/j.svg" alt="j" width="48">
<img src="https://unpkg.com/nyc-subway-icons@0.4.0/svg/z.svg" alt="z" width="48">
<img src="https://unpkg.com/nyc-subway-icons@0.4.0/svg/g.svg" alt="g" width="48">
<img src="https://unpkg.com/nyc-subway-icons@0.4.0/svg/sir.svg" alt="sir" width="48">
<img src="https://unpkg.com/nyc-subway-icons@0.4.0/svg/h.svg" alt="h" width="48">
<img src="https://unpkg.com/nyc-subway-icons@0.4.0/svg/t.svg" alt="t" width="48">
</p>

## Some notes

* Uses the [official MTA colors](http://web.mta.info/developers/resources/line_colors.htm).
* __Note:__ There's no official color for the SIR (Staten Island Railway) line; this is approximated from the MTA website's low-resolution imagery. It doesn't look like the SIR icon is really used anywhere except for the MTA website.
* A good resource for SVG icons exist in the public domain on [Wikipedia](http://commons.wikimedia.org/wiki/New_York_City_Subway_bullets), which includes historical lines. I referred to these for guidance, but created my own from scratch. In comparison, I increased the X-height of each letter in relationship to the circle in my version. This allows each bullet to "read" better when used as part of inline text, such as in MTA status alerts.

### Examples of usage in the wild

* The [MTA Weekender Unofficial HD Remaster](https://weekender.netlify.com/), my update of the [MTA's Weekender](http://web.mta.info/weekender/servicestatus.html). ([GitHub](https://github.com/louh/weekender))


## Technocery

You can install this in a Node project with a package manager, e.g.

```sh
npm install nyc-subway-icons
```

or

```sh
yarn add nyc-subway-icons
```


### To convert SVG to PNG

Get `librsvg` for your system, e.g.

```sh
brew install librsvg
```

Then:

```sh
for svg in ./svg/*.svg; do rsvg-convert -o "${svg%.svg}".png "$svg"; done
```


## License

I claim no ownership or rights over this work.

[CC0](http://creativecommons.org/publicdomain/zero/1.0/).
