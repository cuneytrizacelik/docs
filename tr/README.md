#[flexible.gs](http://flexible.gs)

Flexible Grid System bir Responsive CSS Framework'üdür.

Kuruluma başlamadan önce **HTML**, **CSS** veya **Sass**, **LESS** yada **Stylus** bilmeniz gerekmektedir.

Öğrenmeye başlamadan önce ise **Grid System** ve **Responive Design** hakkında birazcık bilgi sahibi olmanız yeterlidir.

##Kurulum

Flexible Grid System ile kod yazmanın iki yöntemi bulunmaktadır. Bunlar Statik ve Dinamik olmak üzere ikiye ayrılır. İki yöntemi aynı anda yada ayrı ayrı kullanmanız mümkündür.

###Statik
Statik yönetimi tercih ederseniz Flexible Grid System'in **CSS** ile hazırlanmış sabit classlarını kullanarak **HTML** kısmında kodlama yapabilirsiniz.
- [CSS](#css-kurulumu)

###Dinamik
Dinamik yöntemi tercih ederseniz Flexible Grid System'in **Sass**, **LESS** veya **Stylus** ile hazırlanmış mixinlerini kullanarak **CSS** kısmında kodlama yapabilirsiniz.
- [Sass](#sass-kurulumu)
- [LESS](#less-kurulumu)
- [Stylus](#stylus-kurulumu)

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

[Dosyaları indirin](https://github.com/flexiblegs/flexiblegs/archive/3.0.2.zip) ve kullanmak istediğiniz format doğrultusunda stil dosyalarınız arasına ekleyin.

####Responsive
Flexible Grid System'in responsive olarak kullanılmasını istiyorsanız `<head>` tagleri arasına aşağıdaki şekilde bir ekleme yapmanız yeterli olacaktır.
```html
<head>
  <meta name="viewport" content="width=device-width, initial-scale=1">
</head>
```

###[CSS Kurulumu](https://github.com/flexiblegs/flexiblegs/tree/master/static/css/flexiblegs)

#####Kaynak Kodu
```
css/
└── flexiblegs/
    ├── flexiblegs.css
    └── flexiblegs.min.css
```
Kaynak kodunu [görüntüleyin.](https://github.com/flexiblegs/flexiblegs/tree/master/static/css/flexiblegs)

####Kurulum
CSS kurulumu için `<head>` tagleri arasına aşağıdaki şekilde ekleme yapmanız yeterli olacaktır.
```html
<head>
  <link rel="stylesheet" href="flexiblegs/flexiblegs.min.css">
</head>
```

###[Sass Kurulumu](https://github.com/flexiblegs/flexiblegs/tree/master/dynamic/sass)

#####Kaynak Kodu
```
sass/
├── flexiblegs/
│   ├── _flexiblegs.sass
│   └── flexiblegs/
│       ├── _layout.sass
│       ├── _mixins.sass
│       └── mixins/
│           ├── _container.sass
│           ├── _wrap.sass
│           ├── _flexbox.sass
│           ├── _col.sass
│           ├── _gutter.sass
│           └── _align.sass
scss/
└── flexiblegs/
    ├── _flexiblegs.scss
    └── flexiblegs/
        ├── _layout.scss
        ├── _mixins.scss
        └── mixins/
            ├── _container.scss
            ├── _wrap.scss
            ├── _flexbox.scss
            ├── _col.scss
            ├── _gutter.scss
            └── _align.scss
```
Kaynak kodunu [görüntüleyin.](https://github.com/flexiblegs/flexiblegs/tree/master/dynamic/sass)

####Kurulum
Sass kurulumu için `scss` veya `sass` uzantılı stil dosyanız içerisine aşağıdaki şekilde ekleme yapmanız yeterli olacaktır.

```scss
// scss
@import "flexiblegs/flexiblegs";
```
```sass
// sass
@import "flexiblegs/flexiblegs"
```

###[LESS Kurulumu](https://github.com/flexiblegs/flexiblegs/tree/master/dynamic/less/flexiblegs)
#####Kaynak Kodu
```
less/
└── flexiblegs/
    ├── flexiblegs.less
    └── flexiblegs/
        ├── layout.less
        ├── mixins.less
        └── mixins/
            ├── container.less
            ├── wrap.less
            ├── flexbox.less
            ├── col.less
            ├── gutter.less
            └── align.less
```
Kaynak kodunu [görüntüleyin.](https://github.com/flexiblegs/flexiblegs/tree/master/dynamic/less/flexiblegs)

####Kurulum
LESS kurulumu için `less` uzantılı stil dosyanız içerisine aşağıdaki şekilde ekleme yapmanız yeterli olacaktır.

```less
@import "flexiblegs/flexiblegs.less";
```

###[Stylus Kurulumu](https://github.com/flexiblegs/flexiblegs/tree/master/dynamic/stylus/flexiblegs)
#####Kaynak Kodu
```
stylus/
└── flexiblegs/
    ├── flexiblegs.styl
    └── flexiblegs/
        ├── layout.styl
        ├── mixins.styl
        └── mixins/
            ├── container.styl
            ├── wrap.styl
            ├── flexbox.styl
            ├── col.styl
            ├── gutter.styl
            └── align.styl
```
Kaynak kodunu [görüntüleyin.](https://github.com/flexiblegs/flexiblegs/tree/master/dynamic/stylus/flexiblegs)

####Kurulum
Stylus kurulumu için `styl` uzantılı stil dosyanız içerisine aşağıdaki şekilde ekleme yapmanız yeterli olacaktır.

```styl
@import "flexiblegs/flexiblegs"
```

###[Ruby on Rails Kurulumu](https://github.com/flexiblegs/flexiblegs-rails)

Kaynak kodunu [görüntüleyin.](https://github.com/flexiblegs/flexiblegs-rails)

##Lisans
- Flexible Grid System MIT Lisansı altında lisanslanmıştır.
  - [http://opensource.org/licenses/MIT](http://opensource.org/licenses/MIT)
- Flexible Grid System dökümantasyonu Creative Commons Attribution 4.0 International Lisansı altında lisanslanmıştır.
  - [http://creativecommons.org/licenses/by/4.0](http://creativecommons.org/licenses/by/4.0)
