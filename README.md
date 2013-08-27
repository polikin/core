compass_mixins
==============

Here's some mixins that I created or integrate from other people. It's very useful!
Obviously, you can add or modified those mixins for your own code.    

Now with:    
- Susy Responsive Grid (http://susy.oddbird.net/)    
- Ceaser CSS3 Animations (https://github.com/jhardy/compass-ceaser-easing)    
- GetSkeleton Grid (https://github.com/theresponsiveness/GetSkeleton1200-or-960 & http://getskeleton.com/)    

No need to install any gems.

#####Usage (Compass is needed)
---
`@import "_charcoal-core"` - everything (GetSkeleton Grid, Susy Grid, Ceaser, Custom mixins)    
`@import "_charcoal-core/src/_susy"` - Susy grid only    
`@import "_charcoal-core/src/_ceaser"` - CSS3 easing animations only    
`@import "_charcoal-core/src/_responsive-grid"` - GetSkeleton Grid only (Refer to https://github.com/theresponsiveness/GetSkeleton1200-or-960)    

---


#####Type of mixins: | file: _core-functions.scss
---
`media-query`    
`image size`    
`image height`    
`image width`    
`background-image`    
`center absolute`    
`prefix, suffix, prefix & suffix`    
`keyframes`    
`debug`    
`font-face`    
`triangle`    
`circle`    
`placeholder color`  

---

#####How to use Ceaser mixins
---

`@include ceaser-transition(all, 800ms, $easeInQuad);`

---

#####How to use Susy
---

The only thing you have to do is to create susy variables and you're good to go!    

---

#####How to use Animate.sass
---

`@import "animate/_shared";`    
`@import "animate/_animations";`    

then    

`@include animations(fading-entrances);` - entrances animations family    
or    
`@include animations(fading-entrances/fadeInRight);` - specific animation     

reference: https://github.com/theresponsiveness/animate.sass