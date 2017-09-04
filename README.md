ch.08# Head-First-HTML-CSS

This is my learning-record and codes.


## Note

**ch.03**  
1. void elements: < br >, < img >, < link >  

**ch.05**  
1. How to choose image format:  
  lots of colors: JPEG or PNG;  
  lots of continuous colors: JPEG;  
  simple logo and icon with slightly geometric: PNG or GIF;  
  transparency: PNG, GIF(limited);  

**ch.06 industry standard HTML**  
1. HTML5 doctype: <!doctype html>  
2. Adding a meta tag to specify the character encoding (after HTML5): < meta charset="utf-8" >  
3. W3C validator: http://validator.w3.org  

**ch.07 CSS**  
1. How to use external stylesheet to add CSS-Style:  
  < link type="text/css" rel="stylesheet" href="???.css" >
  **p.s. External Stylesheet makes it easier if you want to do some adjustments for style.**  
2. Specificity grade of CSS (bottom is specificer than upper):  
  body {}  
  other_element {}  
  .class {}  
  other_element.class {}  
3. By equal specificity the last CSS wins.  
4. We can make an element belonged to many classes, like this:  
  < p class="tea cafe cocktails" >  
  But only the the class selector in ???.css works.(NOT means the last classname in < p > element)  
5. W3C CSS validator: http://jigsaw.w3.org/css-validator/  

**ch.08 CSS: font**  
1. Customize the fonts with font-family property:  
  example: body { font-family: Verdana, Geneva, Arial, sans-serif; }  
  explain: element { font-family: "alternative font A", "alternative font B", "alternative font C", "fontfamilyname"}  
  There are 5 font families: **sans-serif**, **serif**, **monospace**, **cursive** and **fantasy**.  
2. Using **@font-face** to load the fonts:  
  .woff is a font format, which is accepted for most modern browsers.  
  example:  
    @font-face {  
       font-family: "Emblema One";  
       src: url("http://wickedlysmart.com/hfhtmlcss/chapter8/journal/EmblemaOne-Regular.woff");  
    }  
  explain:  
    i. @font-face is NOT a ordinary CSS selector rule, it's kind of special rule and should be wrote above the body selector rule;  
    ii. use { font-family: "???"; } to give this font-family a name;  
    iii. src can use full url on Internet or from local data.  
3. Fontsize:  
  absolute: { font-size: ??px; }  
  relative to inherited size: { font-size: ??%; } or { font-size: ??em; }  
  keywords: { font-size: small; }  
  **p.s. Relative-Size makes it easier than all in pixels if you want to do some adjustments for font size.**  
4. Default sizes of font:  
  default font-size: 16px;  
  < h1 >: 200% of default font-size;  
  < h2 >: 150% of default font-size;  
  < h3 >: 120% of default font-size;  
  < h4 >: 100% of default font-size;  
  **p.s. If you don't use absolute but relative font-size in body CSS selector, then it will be relative to the default value.**  



