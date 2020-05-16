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
