# Coder Swag App

UIKit storyboard örneği. Uygulama, yazılımcı swag’i için **Shop By Category** ekranıyla açılır: şapkalar, hoodieler, tişörtler ve dijital ürünler.

## Teknoloji

- Swift 5
- UIKit ve storyboard
- Dağıtım hedefi: iOS 16
- Xcode 16 veya üzeri

## Gereksinimler

- macOS üzerinde Xcode 16 veya üzeri
- iOS 16 veya üzeri bir simülatör

## Çalıştırma

1. Depoyu klonlayın.
2. `CoderSwagApp.xcodeproj` dosyasını açın.
3. Bir simülatör seçin.
4. Run ile çalıştırın.

## Proje düzeni

```
CoderSwagApp.xcodeproj/
CoderSwagApp/
  AppDelegate.swift
  Info.plist
  Controller/
    ViewController.swift
  View/
    CategoryCell.swift
  Base.lproj/
    Main.storyboard
    LaunchScreen.storyboard
  Assets.xcassets/
    hats, hoodies, shirts, digital
    hat01–hat04, hoodie01–hoodie04, shirt01–shirt05
    AppIcon.appiconset
```

`Main.storyboard` bir navigasyon denetleyicisiyle başlar. Kök sahnenin başlığı Coder Swag’tir. Ekranda Shop By Category etiketi ve `categoryTable` çıkışına bağlı bir tablo vardır. Prototip hücre `CategoryCell`’dir; `categoryImage` ve `categoryTitle` bağlıdır. Hücredeki yer tutucu görsel `digital`, yer tutucu başlık HOODIES’tir.

`LaunchScreen.storyboard` boş bir açılış ekranıdır. Varlık kataloğunda kategori görselleri (`hats`, `hoodies`, `shirts`, `digital`) ve ürün görselleri (`hat01`–`hat04`, `hoodie01`–`hoodie04`, `shirt01`–`shirt05`) vardır. `AppIcon.appiconset` yalnızca yuva tanımları içerir; ikon dosyası yoktur.

## Durum

Kategori tablosu ve `CategoryCell` vardır. Tabloya veri kaynağı bağlanmamıştır. `ViewController` veri kaynağı veya delege uygulamaz. Ürün akışı yazılmamıştır.

## Yazar

Halil Özel
