## Dal (Branch) İsimleri
- feature/<ozellik>   : Yeni özellikler
- hotfix/<duzeltme>   : Acil düzeltmeler (yayınlanan sürüm için)
- docs/<icerik>       : Belgelendirme değişiklikleri
- chore/<is>          : Bağımlılık, araç, yapılandırma vb.

## Commit Stili — Conventional Commits
- feat: yeni, geriye uyumlu özellik
- fix: hata düzeltmesi
- docs: dokümantasyon
- chore: araç/bağımlılık/temizlik
- refactor: davranışı değiştirmeden kod düzeni
Örnek: `feat(notes): add category template`

## Sürümleme — SemVer
- Etiket biçimi: vMAJOR.MINOR.PATCH (örn. v0.1.0, v0.1.1)
- Yayınlar için **annotated tag** kullanın.

## Basit Yayın Akışı
`git tag -a v0.1.1 -m "v0.1.1: hotfix README typo + guide reference"
git push origin main
git push origin v0.1.1
`
Yukarıdaki basit bit tag commitlemesi bulunuyor. İşlemlerini bu şekilde sürdür.