# Masaüstü Dosya Araçları

Günlük ofis işlerinde zaman kazandıran iki küçük Python aracı. Her ikisi de hem grafik arayüzle hem komut satırından çalışır.

> Bu depo bir proje vitrinidir. Kaynak kod paylaşılmamaktadır.

## 1. macOS Artık Dosya Temizleyici

macOS'tan kopyalanan klasörlerde oluşan `._dosya` (AppleDouble), `.DS_Store`, `__MACOSX`, `Thumbs.db` gibi gereksiz dosyaları bulur ve siler.

- `._` ile başlayan dosyalar **dosya imzasıyla (magic bytes)** doğrulanır, böylece gerçek dosyalar yanlışlıkla silinmez
- Önce deneme modunda listeler, onaydan sonra siler
- Arka plan iş parçacığı sayesinde arayüz donmaz

## 2. Belge İçinde Metin Arama

Bir klasör ağacındaki tüm belgelerin **içinde** metin arar.

- Düz metin dosyalarının yanında `.docx`, `.xlsx`, `.pptx`, `.odt` ve `.ods` dosyalarını açmadan tarar (ZIP + XML okuma)
- Büyük/küçük harf duyarlı veya duyarsız arama
- Hangi dosyada ve hangi bölümde bulunduğunu raporlar

## Teknolojiler

`Python` · `Tkinter` · `zipfile` · `threading`
