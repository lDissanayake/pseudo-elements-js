# pseudo-elements-js
Way to modify CSS of pseudo-elements with animeJS

##Anime JS animate pseudo-elements
```
var st = document.createElement('style');
document.querySelector('head').append(st);

var fo = { background: '#444', width: 0 }; // animejs will animate this object

anime( {
      targets: fo,
      duration: 6000,
      width: ['0','200%'],
      background: ['#333', 'rgb(0,255,0)'],
      update: function() {
          st.innerText = '.invt-blog-post_meta:after{ background:' + fo.background  + '; width:' + fo.width + ';}'
      },
} );
```
