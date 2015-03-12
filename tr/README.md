#[flexible.gs](http://flexible.gs)

Flexible Grid System bir Responsive CSS Framework'üdür.

Kuruluma başlamadan önce **HTML**, **CSS** veya **Sass**, **LESS** yada **Stylus** bilmeniz gerekmektedir.

##Kurulum

Flexible Grid System ile kod yazmanın iki yöntemi bulunmaktadır. Bunlar Statik ve Dinamik olmak üzere ikiye ayrılır. İki yöntemi aynı anda yada ayrı ayrı kullanmanız mümkündür.

###Statik
Statik yönetimi tercih ederseniz Flexible Grid System'in **CSS** ile hazırlanmış sabit classlarını kullanarak **HTML** kısmında kodlama yapabilirsiniz.
- [CSS Kurulumu](#css-kurulumu)
- [Ruby on Rails Kurulumu](#ruby-on-rails-kurulumu)

###Dinamik
Dinamik yöntemi tercih ederseniz Flexible Grid System'in **Sass**, **LESS** veya **Stylus** ile hazırlanmış mixinlerini kullanarak **CSS** kısmında kodlama yapabilirsiniz.
- [Sass Kurulumu](#sass-kurulumu)
- [LESS Kurulumu](#less-kurulumu)
- [Stylus Kurulumu](#stylus-kurulumu)
- [Ruby on Rails Kurulumu](#ruby-on-rails-kurulumu)

###[Dosyaları indirin](https://github.com/flexiblegs/flexiblegs/archive/3.0.3.zip)

[Dosyaları indirin](https://github.com/flexiblegs/flexiblegs/archive/3.0.3.zip) ve kullanmak istediğiniz format doğrultusunda stil dosyalarınız arasına ekleyin.

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
└── sass/
    ├── flexiblegs/
    │   ├── _flexiblegs.sass
    │   └── flexiblegs/
    │       ├── _breakpoints.sass
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
            ├── _breakpoints.scss
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
        ├── breakpoints.less
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
        ├── breakpoints.styl
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

##Öğrenme

Öğrenmeye başlamadan önce **Grid System** ve **Responive Design** hakkında bilgi sahibi olmanız gerekmektedir.

####Responsive Meta
Flexible Grid System'in responsive olarak kullanılmasını istiyorsanız `<head>` tagleri arasına aşağıdaki şekilde ekleme yapmanız gerekmektedir.
```html
<head>
  <meta name="viewport" content="width=device-width, initial-scale=1">
</head>
```

###CSS Kodları

Öncelikle Flexible Grid System altyapısı oluşurken kullanılan **CSS** kodlarını, neden kullanıldıklarını ve arkaplanda işlerin nasıl çalıştığıyla ilgili bilgi sahibi olmanız kullanım hakimiyetiniz açısından oldukça faydalı olacaktır.

Örnek kodlarda CSS kısmında sabit Sass, LESS veya Stylus kısmında dinamik olacak kısımları @ işareti ile belirtilmektedir.

###.container

**CSS** kısmında **container** class genişliği `1140px` ile sınırlıdır. Değişiklik yapmanızda sakınca yoktur.

**Sass**, **LESS** veya **Stylus** kısmında **container** mixinini kullanırken istediğiniz genişliği dinamik olarak belirtmeniz mümkün olacaktır.

**container** class veya mixini eklenen elementin belirtilen genişlik kadar sayfada ortalı durmanısını sağlayan özellik ise `margin-left: auto;` ve `margin-right: auto;` kullanımıdır, ayrı olarak belirtilmesinin sebebi `margin-top` veya `margin-bottom` özelliği eklemesi yapıldığında belirttiğiniz değerin ezilmemesini sağlar. `max-width` kullanımı ise ekran boyutunuz daraldığında **container** ekli elementin `100%` olarak davranmasını sağlayacaktır.

```
max-width: @width;
margin-left: auto;
margin-right: auto;
```

###.wrap

###.flexbox

###.col

###.gutter

###.align

##Lisans
- Flexible Grid System MIT Lisansı altında lisanslanmıştır.
  - [http://opensource.org/licenses/MIT](http://opensource.org/licenses/MIT)
- Flexible Grid System dökümantasyonu Creative Commons Attribution 4.0 International Lisansı altında lisanslanmıştır.
  - [http://creativecommons.org/licenses/by/4.0](http://creativecommons.org/licenses/by/4.0)

##Gelecek

- Flexible Grid System Yeni Websitesi · [Geliştirme aşaması](https://github.com/flexiblegs/website)
  - Kurulum
  - Öğrenme
  - Kütüphane
    - Flexible Colors
    - Flexible Style
    - Flexible Fonticons
    - Flexible Navbar
    - Flexible Tabs
    - Flexible Slider ve daha fazlası :)
  - Flexible Formule · [Tweet linki](https://twitter.com/flexiblegs/status/550265997639573504)
  - Responsive Test
  - Customization · [Geliştirme aşaması](https://github.com/flexiblegs/website/blob/master/app/models/customization.rb)
  - Hikaye
- Flexible Grid Builder · [Geliştirme aşaması](https://github.com/flexiblegs/gridbuilder)
- Flexible Frontend Editor
- Flexible Shop
  - Mug
  - Shirt
  - Sticker ve daha fazlası :)
- Flexible Workspace & Cafe
  - Kahve (Flexible Blend)
  - Havuçlu Kek (flexible.gs logolu kek kalıbında :P) ve daha fazlası :)

##Bağış yapın

PayPal aracılığıyla bağış yapın :)

<form action="https://www.paypal.com/cgi-bin/webscr" method="post" target="_top">
<input type="hidden" name="cmd" value="_s-xclick">
<input type="hidden" name="hosted_button_id" value="NHEUHUB8863NS">
<input type="image" src="http://flexible.gs/svg/ppcom.svg" border="0" name="submit" alt="PayPal - The safer, easier way to pay online!">
<img alt="" border="0" src="https://www.paypalobjects.com/tr_TR/i/scr/pixel.gif" width="1" height="1" alt="PayPal">
</form>

*NOT : Dökümantasyonu yazmaya devam ediyorum [@dnomak](https://github.com/dnomak) adresinden beni takip edebilirsiniz.*