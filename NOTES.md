* Okay! I want to plot this awesome Roadster orbit
* So I go to HORIZONS and query for the data
* "Ecliptic and Mean Equinox of Reference Epoch" WHAT DOES THIS EVEN MEAN
* There are two ecliptic frames in Astropy, and both are TrueEcliptic
  - It depends on how you compute the rotation matrix -- should be easy right? RIGHT??
  - What's the difference? SCREENSHOT https://github.com/astropy/astropy/pull/6508#issue-139054262
* "Obliquity of 84381.448" sounds great, but life isn't easy!
  - ecliptic-no-comments.dat
* So we have to support both Mean and True ecliptic...
  - with several different obliquity values...
  - (or even arbitrary ones)...
  - Geocentric, Heliocentric, and Barycentric...
  - This amounts to _at least_ 12 different reference frames!
* Some of this reference frames are only theoretical and we have
  no evidence of people actually using them
* So... PLIZ HALP

jupyter nbconvert "file.ipynb" --to slides --reveal-prefix "https://cdnjs.cloudflare.com/ajax/libs/reveal.js/3.5.0"
