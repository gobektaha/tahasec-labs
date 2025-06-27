# Mini XSS Lab

Bu küçük HTML uygulaması, **Stored veya Reflected XSS** değil, basit bir **DOM-Based XSS** örneğidir.

## XSS Nedir?

**Cross-Site Scripting**, bir uygulamanın kullanıcıdan gelen girdiyi doğru şekilde filtrelememesi sonucu, zararlı JavaScript kodlarının çalıştırılmasına olanak tanır.

## Bu Projede Ne Oluyor?

- Kullanıcıdan bir girdi alınıyor
- Bu girdi DOM’a `innerHTML` ile direkt yazılıyor
- Filtreleme yapılmadığı için `<script>` etiketi dahil her şey çalışıyor

## Dene:

```html
<script>alert("XSS by tahasec-labs")</script>
