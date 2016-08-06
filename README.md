# jquery_gototop
This is simple and useful go to top jquery with full example. All you have to do is adding jquery library via CDN (google apis) and
start writing some code

This is the full source code looks like

```javascript
<!DOCTYPE HTML>
<html>
 <head>
  <title></title>
 </head>
 <body>
  <a href='#home' tile="Go to top">
   <div class="arrowup">
    <img src="/path/of/image/">
   </div>
  </a>
 </body>
 <script type="https://ajax.googleapis.com/ajax/libs/jquery/1.12.4/jquery.min.js">
 <script>
  $(document).ready(function(){
    $(windows).scroll(function(){
      if($(this).scrollTop() > 500){
        $(".arrowup").fadeIn(100);
      }
      else {
        $(".arrowup").fadeOut(400);
      }

     });

     $(".arrowup").click(function(){
      $("html, body").animate({scrollTop:0}, 800);
     });
  });
 <script>
</html>
```
Just make a div class as a selector (arrowup) and modify it with jquery instantly

