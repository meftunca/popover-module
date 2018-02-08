## PopOver modül kullanımı
Açıklamaya başlamadan önce projenin şuanda alpha aşamasında olduğu söylemek isterim. projenin daha da gelişebilmesi için zamana ihtiyacı var. İlk önce kullanılabilir attr(özniteliklere örn(class,id vs)) değinmek isterim...
- `data-title` > popOver için başlık yazmanızı sağlar
- `data-content` > popOver için içerik(text) yazmanızı sağlar
- `data-footer` > popOver için alt alan oluşturmanızı sağlar

### Örnek
Aşağıda popOver için örnek tetikleyici(trigger) yapıyı görebilirsiniz
```html
<a class="btn" role="button" data-arrow="top" data-toggle="popover"
   data-title="popover" data-content="Lorem ipsum dolor sit amet, consectetur adipisicing elit."
   data-footer="popover footer">popover top</a>

<a class="btn" role="button" data-arrow="left" data-toggle="popover"
   data-title="popover" data-content="Lorem ipsum dolor sit amet, consectetur adipisicing elit."
   data-footer="popover footer">popover left</a>

<a class="btn" role="button" data-arrow="right" data-toggle="popover"
   data-title="popover" data-content="Lorem ipsum dolor sit amet, consectetur adipisicing elit."
   data-footer="popover footer">popover right</a>

<a class="btn" role="button" data-arrow="bottom" data-toggle="popover"
   data-title="popover" data-content="Lorem ipsum dolor sit amet, consectetur adipisicing elit."
   data-footer="popover footer">popover bottom</a>

```
#### Tetikleyici sonrası body tagi içindeki çıktısı...
> PopOver öğeleri body içinde en alta atanır. Tetikleyicinin görevi Öğeleri oluşturmak,kaldırmak ve gerekli verileri sağlamaktır.

```html
<div class="popover-content arrow-top show">
   <div class="popover-header">popover</div>
   <div class="popover-body">
   Lorem ipsum dolor sit amet, consectetur adipisicing elit.
   </div>
   <div class="popover-footer">popover footer</div>
</div>
```

#### Eklenecek özellikler
1. Json verilerinizi belirli content alanı içinde popover nesnesi ile görüntü alma
2. Anlık görsel görüntüleme...
3. ... (###### önerilerinizi bekliyorum)

###### [Codepen linki](https://codepen.io/by-Meftunca/pen/aqpoeO)
