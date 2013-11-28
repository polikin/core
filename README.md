#core

####twitter: @_polikin


#####* The docs will come soon!
==============
Every librairie is called by mixin. So, you can call `@import "_core"` and until you include a mixin, nothing will be output. No dependencies!

Now with:    
- Susy Responsive Grid (http://susy.oddbird.net/)    
- Ceaser CSS3 Animations (https://github.com/jhardy/compass-ceaser-easing)    
- Animate.sass (https://github.com/polikin/animate.sass)   
- GetSkeleton Grid (https://github.com/theresponsiveness/GetSkeleton1200-or-960 & http://getskeleton.com/)    
- Jacket Sass (https://github.com/Team-Sass/jacket/)    

No need to install any gems.

#####Available on Bower
```
bower install core
```
---
#####Why should I use Core?    

Well, the main idea here is that Core import some libs that we probably use everytime in our project. 
So, with Core you don't have to install any gems. Everything is up to date and ready to be import. 
Per example. You want to use Susy for your project. Then, your co-worker has need to work on the same project. 
Until Core, he should install the gem on his computer. 
If not, the compilation failed. With Core, you drop the folder `core` in your project and you're good to go.

---
#####Usage (Compass is needed)
---
`@import "_core"` - everything (GetSkeleton Grid, Susy Grid, Ceaser, Custom mixins)    
`@import "_core/src/_susy"` - Susy grid only    
`@import "_core/src/_ceaser"` - CSS3 easing animations only    
`@import "_core/src/_responsive-grid"` - GetSkeleton Grid only (Refer to https://github.com/theresponsiveness/GetSkeleton1200-or-960)    

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
`arrow`    
`circle`    
`placeholder color`  
`truncate`  

---

#####How to use Ceaser mixins
---

`@include ceaser-transition(all, 800ms, $easeInQuad);`    

reference: https://github.com/jhardy/compass-ceaser-easing

---

#####How to use Susy
---

The only thing you have to do is to create susy variables and you're good to go!    

http://susy.oddbird.net/

---

#####How to use Animate.sass
---

`@import "animate/_shared";`    
`@import "animate/_animations";`    

then    

`@include animations(fading-entrances);` - entrances animations family    
or    
`@include animations(fading-entrances/fadeInRight);` - specific animation     

reference: https://github.com/polikin/animate.sass
