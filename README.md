# <a href="http://bootstraptema.ru/stuff/plugins_bootstrap/design/bootstrap_scrollie_bgcolor/13-1-0-1269">Bootstrap-Scrollie-BgColor</a>
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

#### По умолчанию используется свойство <code>background-color</code>
#### Комбинация цвета секции определяется атрибутом <code>data-background</code>
