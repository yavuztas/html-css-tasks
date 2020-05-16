# Task 3 - HTML araştıması

Bu görevde bazı HTML taglarının her browser da desteklenmediğini ve hatta browserların versiyonlarına göre de çalışmayabileceğini belirttikten sonra bizden aşağıda verilen `<details>` ve `<keygen>` HTML taglarını araştırmamızı istiyor. Bize verdiği browserların bazı versiyonları için (`Chrome 81`, `Safari 13`, `Firefox 75`, `Internet Explorer 11`, `Edge 81` ve `Opera Browser 68`) bir tablo hazırlamamızı istiyor.

Hangi tagların hangi browserlar ve hangi versiyonlarında çalıştığını [https://developer.mozilla.org/] sitesinden bakabiliriz.
 - `<details>`: [https://developer.mozilla.org/en-US/docs/Web/HTML/Element/details](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/details)
 - `<keygen>`: [https://developer.mozilla.org/en-US/docs/Web/HTML/Element/keygen](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/keygen)
 
Bu sayfalarda belirtilen tagın ne işe yaradığı ve nasıl kullanılabileceği örnekler ile anlatılıyor. Sayfaların en alt kısmında da browser lara göre destekleyip desteklemediği ile ilgili bir tablo mevcut.

İlgili tablolardan sırayla aradağımız browser ve versiyonu için bakıp, bizde bu tablonun daha basitini aşağıdaki şekilde yapabiliriz:
<table>
  <tr>
    <th></th>
    <th>Chrome 81</th>
    <th>Safari 13</th>
    <th>Firefox 75</th>
    <th>Internet Explorer 11</th>
    <th>Edge 81</th>
    <th>Opera Browser 68</th>
  </tr>
  <tr>
    <td>details</td>
    <td>√</td>
    <td>√</td>
    <td>√</td>
    <td>×</td>
    <td>√</td>
    <td>√</td>
  </tr>
  <tr>
    <td>keygen</td>
    <td>×</td>
    <td>√</td>
    <td>×</td>
    <td>×</td>
    <td>×</td>
    <td>√</td>
  </tr>
</table>

Bu tablonun HTML kodu aşağıdaki şekilde olacak:
```html
<table>
  <tr>
    <th></th>
    <th>Chrome 81</th>
    <th>Safari 13</th>
    <th>Firefox 75</th>
    <th>Internet Explorer 11</th>
    <th>Edge 81</th>
    <th>Opera Browser 68</th>
  </tr>
  <tr>
    <td>details</td>
    <td>√</td>
    <td>√</td>
    <td>√</td>
    <td>×</td>
    <td>√</td>
    <td>√</td>
  </tr>
  <tr>
    <td>keygen</td>
    <td>×</td>
    <td>√</td>
    <td>×</td>
    <td>×</td>
    <td>×</td>
    <td>√</td>
  </tr>
</table>
```
**NOT:** Ayrıca `<keygen>` tagının deprecated olduğu yani artık kullanılmayacağıda sitede belirtiliyor. Zamanla destekleyen `Opera` ve `Safari` de de kaldırılabilir demek bu. Bunu da belirtmek faydalı olabilir.

# Task 4 - Impl HTML & CSS Uygulama

Burada about sayfasına resim ve video şu şekilde koyabilirsin:
```html
<p>İşte bizim muhteşem ekibimiz durmak bilmeden çalışmaya devam ediyor:</p>
<img width="600" src="https://blog.dacadoo.com/wp-content/uploads/2014/10/800x799/14107236.jpg" />
<p>Ayrıca size son çalışmamızdan bazı görüntüler sunmak isteriz:</p>
<video width="600" controls poster="http://media.w3.org/2010/05/sintel/poster.png">
  <source src="http://media.w3.org/2010/05/sintel/trailer.mp4" type="video/mp4">
</video>
```
Bunları hizalamak için genellikle CSS kullanman gerekir. Hızlı bir çözüm olarak tavsiyem ayrı bir `<div>` tagı içine alıp hepsini ortalamak için stil olarak `text-align: center;` vermen kolay olacaktır:
```html
<div style="text-align: center;">
  ... 
</div>
```
Üzerinde oynamak ve denemek istersen aşağıdaki codepen linkinden yapabilirsin:

[https://codepen.io/justintc/pen/KKdGoym](https://codepen.io/justintc/pen/KKdGoym)

# Task 5 - CSS Selectorlar

Bu kısımda sadece CSS selector için hangi kaynaklardan çalışabilirsin onların linkini vermiş. En basit anlamda bir CSS selector a örnek verelim. Aşağıdaki şekilde bir HTML yapımız olsun:
```html
<div>
  <p>başlık 1<p>
  <p>başlık 2<p>
</div>
```
Burada `<div>` tagının altındaki tüm `<p>` taglarını select etmek için şu CSS selector ifadesini kullanmalıyız:
```css
div > p {
  color: red;  
}
```
`div > p` selector ı sonucunda uyguladığımız stil ile `<div>` tagı altındaki tüm başlıkları kırmızı renke çevirmiş olduk.

Verilen örneklerden [https://flukeout.github.io/](https://flukeout.github.io/) hem eğlenceli hem de interaktif olarak çalışmak için çok güzel duruyor. Tavsiye ederim.
