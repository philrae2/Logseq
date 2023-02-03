---
title: roam/css
---

- 
```css
@import url('https://rcvd.github.io/roam-css-system/themes/bear.css');
::-webkit-scrollbar {
    width: 7px;
}


/* this code hides all block tags */
[data-tag^="chld:"],
[data-tag^="blck-chld:"],
[data-tag^="blck:"] {
display:none;
}

[data-page-links*="blck:grey"] > .rm-block-main,
[data-page-links*="blck-chld:grey"],
[data-page-links*="chld:grey"] > .rm-block-children
{
    /* color: #383d41; */
    background-color: #40454F;
    border: 1px solid #40454F; 
    margin-bottom: 5px;
}

[data-page-links*="blck:blue"] > .rm-block-main,
[data-page-links*="blck-chld:blue"],
[data-page-links*="chld:blue"] > .rm-block-children
{
 /*	 color: #004085;*/
    background-color: #0C5B7C;
    /*border-color: #b8daff;*/
  border: solid 1px #0C5B7C;
  /*border-color: #80BDFF;*/
    margin-bottom: 5px;
}
[data-page-links*="blck:green"] > .rm-block-main,
[data-page-links*="blck-chld:green"],
[data-page-links*="chld:green"] > .rm-block-children
{
 
  /*   color: #155724; */
    background-color: #094D19;
    border: 1px solid #094D19;
  
    margin-bottom: 5px;
}

[data-page-links*="blck:red"] > .rm-block-main,
[data-page-links*="blck-chld:red"],
[data-page-links*="chld:red"] > .rm-block-children
{
 
  /*   color: #721c24;*/
    background-color: #7D373D;
    border: 1px solid #7D373D;
  
    margin-bottom: 5px;
}

[data-page-links*="blck:yellow"] > .rm-block-main,
[data-page-links*="blck-chld:yellow"],
[data-page-links*="chld:yellow"] > .rm-block-children
{
 
 /*  color: #856404; */
    background-color: #52451A;
    
  border: 1px solid #52451A;
 
    margin-bottom: 5px;
}
```
