# Amaç
MLOps entegrasyonlu CIFAR-10 Görüntü Sınıflandırma Projesi

# Kurulum
## Sanal Ortamın Kurulumu
- `venv` python sanal ortamını kullandım.
- `python -m venv .venv` komutu ile `.venv` adında bir sanal ortam oluşturdum.
- `.venv\Scripts\activate` komutu ile sanal ortamı aktif hale getirdim.
- Terminalden sanal ortamın aktif olup olmadığını kontrol etmek için kullanabileceğin komutlar:
    - Linux/macOS (bash/zsh):
        - `echo $VIRTUAL_ENV`
    - Windows PowerShell:
        - `echo $env:VIRTUAL_ENV`
    - Windows CMD:
        - `echo %VIRTUAL_ENV%`


# Teknoloji Yığını
- Python 3.12.7

# Dizin Yapısı
`configs`: Konfigürasyon parametrelerinin bulunduğu dizindir.

`data`: Ham ve işlenmiş verilerin bulunduğu dizindir.

`experiments`: Yapılan deneylerin çıktılarının bulunduğu dizindir.

`notebooks`: Keşif amaçlı ve ön çalışmaların bulunduğu dizindir.

`reports`: Sonuç rapor ve görsellerinin bulunduğu dizindir.

`src`: Projenin ana kaynak dosyalarının bulunduğu bölümdür.

`requirements.txt`: Projenin bağımlılıklarının bulunduğu dosyadır.