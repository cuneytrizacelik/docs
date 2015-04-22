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

###[Dosyaları indirin](https://github.com/flexiblegs/flexiblegs/archive/4.0.0.zip)

[Dosyaları indirin](https://github.com/flexiblegs/flexiblegs/archive/4.0.0.zip) ve kullanmak istediğiniz format doğrultusunda stil dosyalarınız arasına ekleyin.

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

###Backend

Öncelikle Flexible Grid System altyapısı oluşurken kullanılan **CSS** kodlarını, neden kullanıldıklarını ve arkaplanda işlerin nasıl çalıştığıyla ilgili bilgi sahibi olmanız kullanım hakimiyetiniz açısından oldukça faydalı olacaktır. Kod parçalarında **CSS** kısmında sabit **Sass**, **LESS** veya **Stylus** kısmında dinamik olacak kısımlar **@degisken** şeklinde belirtilmektedir.

###.wrap

###.flexbox

###.col

###.gutter

###.align

##Tarayıcı Desteği

**Responsive Design** olarak kodlama yapıyorsanız **Media Queries** kullanımından kaynaklı **Internet Explorer 9 ve üzeri** versiyonları desteklemek zorunda kalıyoruz.

**Flexbox** özelliğini kullanıyorsak **Internet Explorer 10 ve üzeri** versiyonları desteklemek zorunda kalıyoruz. **Flexbox** özelliğini mobil cihazlardaki tasarım kontrolünü kolaylaştırmak için kullandığımızı düşünürsek **Flexbox** özelliğini kullandığımızda tarayıcı desteği mobil'e geçtiği için otomatikman tarayıcı desteğinide sağlamış oluyoruz.

Yukarıdaki iki durum dışında tüm masaüstü ve mobil tarayıcılara destek sağlanmaktadır.

###CodePen

- Flexible Grid System [CSS](http://codepen.io/dnomak/pen/KwWJpm)
- Flexible Grid System [Sass](http://codepen.io/dnomak/pen/wBzdzj)
- Flexible Grid System [LESS](http://codepen.io/dnomak/pen/yyVXQa)
- Flexible Grid System [Stylus](http://codepen.io/dnomak/pen/EaZPYw)


##Motivasyon

Projeye dört elle sarılmamı sağlayan bazı linkler :)

- [http://designinstruct.com/web-design/flexible-grid-system](http://designinstruct.com/web-design/flexible-grid-system)
- [https://rschu.me/the-history-of-a-nifty-css-flexible-grid-system](https://rschu.me/the-history-of-a-nifty-css-flexible-grid-system)
- [http://webbox5.webbox.io/2014/07/25/004](http://webbox5.webbox.io/2014/07/25/004)
- [https://github.com/showcases/design-essentials](https://github.com/showcases/design-essentials)
- [http://coliss.com/articles/build-websites/operation/css/css-flexible-grid-system-flexiblegs.html](http://coliss.com/articles/build-websites/operation/css/css-flexible-grid-system-flexiblegs.html)
- [http://www.mserdark.com/haftanin-ozeti-4](http://www.mserdark.com/haftanin-ozeti-4)
- [http://www.ozgurwebgunleri.org.tr/2014/etkinlik-programi-2](http://www.ozgurwebgunleri.org.tr/2014/etkinlik-programi-2)
- [http://sass-lang.com/community](http://sass-lang.com/community)
- [http://lesscss.org/usage/#frameworks-using-less-grid-systems](http://lesscss.org/usage/#frameworks-using-less-grid-systems)
- [https://github.com/stylus/stylus/wiki](https://github.com/stylus/stylus/wiki)
- [http://sassbreak.com/resources](http://sassbreak.com/resources)
- [http://www.moongift.jp/2015/04/flexible-gs-レスポンシブ対応のグリッドレイアウトフレ](http://www.moongift.jp/2015/04/flexible-gs-レスポンシブ対応のグリッドレイアウトフレ)

##Gelecek

- Flexible Grid System Yeni Websitesi · [Kaynak kodunu görüntüleyin.](https://github.com/flexiblegs/website)
  - Kurulum · [Kurulum kısmını görüntüleyin.](https://github.com/flexiblegs/docs/tree/master/tr/#kurulum)
  - Öğrenme · [Öğrenme kısmını görüntüleyin.](https://github.com/flexiblegs/docs/tree/master/tr/#Öğrenme)
  - Kütüphane
    - Flexible Breakpoints · [Kaynak kodunu görüntüleyin.](https://github.com/flexiblegs/breakpoints)
    - Flexible Tools · [Kaynak kodunu görüntüleyin.](https://github.com/flexiblegs/tools)
    - Flexible Styles · [Kaynak kodunu görüntüleyin.](https://github.com/flexiblegs/styles)
    - Flexible Colors
    - Flexible Fonticons
    - Flexible Navbar
    - Flexible Tabs · [Kaynak kodunu görüntüleyin.](https://github.com/flexiblegs/tabs)
    - Flexible Slider ve daha fazlası :)
  - Formül · [Tweet linkini görüntüleyin.](https://twitter.com/flexiblegs/status/550265997639573504)
  - Responsive Test
  - Özelleştirme · [Kaynak kodunu görüntüleyin.](https://github.com/flexiblegs/website/blob/master/app/models/customization.rb)
- Flexible Grid Builder · [Kaynak kodunu görüntüleyin.](https://github.com/flexiblegs/gridbuilder)
- Flexible Frontend Editor
- Flexible Shop
  - Mug
  - Shirt
  - Sticker ve daha fazlası :)
- Flexible Workspace & Cafe
  - Kahve (Flexible Blend)
  - Havuçlu Kek (Flexible Grid System logolu kek kalıbında) ve daha fazlası :P

##Sunumlar

- [ODTÜ Halıcı Kuluçka Merkezi 2014](https://speakerdeck.com/dnomak/flexible-project-odtu-2014)
- [Özgür Web Teknolojileri Günleri 2014](https://speakerdeck.com/dnomak/flexible-grid-system-owtg-2014)

##Lisans

- Flexible Grid System MIT Lisansı altında lisanslanmıştır.
  - [http://opensource.org/licenses/MIT](http://opensource.org/licenses/MIT)
- Flexible Grid System dökümantasyonu Creative Commons Attribution 4.0 International Lisansı altında lisanslanmıştır.
  - [http://creativecommons.org/licenses/by/4.0](http://creativecommons.org/licenses/by/4.0)

##PayPal

PayPal aracılığıyla bağış yapabilirsiniz :) `me@dnomak.com`

***NOT :*** *Dökümantasyonu yazmaya devam ediyorum* ***[@dnomak](https://github.com/dnomak)*** *adresinden beni takip edebilirsiniz.*