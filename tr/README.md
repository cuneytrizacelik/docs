#[flexible.gs](http://flexible.gs)

Flexible Grid System bir Responsive CSS Framework'üdür.

Kuruluma başlamadan önce **HTML**, **CSS** veya **Sass**, **LESS** yada **Stylus** bilmeniz gerekmektedir.

Öğrenmeye başlamadan önce ise **Grid System** ve **Responive Design** hakkında birazcık bilgi sahibi olmanız yeterlidir.

##Kurulum

Flexible Grid System'in responsive olarak kullanılması için `<head>` tagleri arasına aşağıdaki şekilde bir ekleme yapmanız yeterli olacaktır.
```html
<head>
  <meta name="viewport" content="width=device-width, initial-scale=1">
</head>
```

Flexible Grid System ile kod yazmanın iki yöntemi bulunmaktadır. Bunlar Statik ve Dinamik olmak üzere ikiye ayrılır. İki yöntemi aynı anda yada ayrı ayrı kullanmanız mümkündür.

####Statik
Statik yönetimi tercih ederseniz flexiblegs sabit class'larını kullanarak **HTML kısmında** kodlama yapabilirsiniz.
- CSS

####Dinamik
Dinamik yöntemi tercih ederseniz flexiblegs mixin'lerini kullanarak **CSS kısmında** kodlama yapabilirsiniz.
- Sass
- LESS
- Stylus

####Klasör Yapısı
```
static/
├── css/
dynamic/
├── sass/
│   ├── sass/
│   └── scss/
├── less/
└── stylus/
```

##Lisans
- Flexible Grid System MIT Lisansı altında lisanslanmıştır.
  - [http://opensource.org/licenses/MIT](http://opensource.org/licenses/MIT)
- Flexible Grid System dökümantasyonu Creative Commons Attribution 4.0 International Lisansı altında lisanslanmıştır.
  - [http://creativecommons.org/licenses/by/4.0](http://creativecommons.org/licenses/by/4.0)
