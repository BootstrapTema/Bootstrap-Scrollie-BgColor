# Bootstrap-Scrollie-BgColor
Изменение цвета фона страницы при скроллинге
## Подключение
<pre>
&lt;script&gt;
$(window).ready(function() {
  
    var wHeight = $(window).height();

    $('.row')
      .height(wHeight)
      .scrollie({
        scrollOffset : -50,
        scrollingInView : function(elem) {
                   
          var bgColor = elem.data('background');
          
          $('body').css('background-color', bgColor);
          
        }
      });

  });
&lt;/script&gt;
</pre>
