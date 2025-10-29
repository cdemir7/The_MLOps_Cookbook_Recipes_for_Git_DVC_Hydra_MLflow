# Genel Git Komutları
## Git (yerel) — “durum” ve “log”
- Durum (çalışma alanı / staging):
    - `git status`: okunabilir özet
    - `git status -sb`: kısa (branch + özet)`
    - `git diff`: henüz stage edilmemiş değişiklikler`
    - `git diff --staged`: stage edilmiş (commit’e gidecek) değişiklikler`

- Commit geçmişi (log):
    - `git log`: ayrıntılı geçmiş
    - `git log --oneline`: her commit tek satır
    - `git log --oneline --graph --decorate --all`: dalları grafikli göster
    - `git log -n 5`: son 5 commit
    - `git show`: son commit’in diff’i
    - `git show --stat`: son commit’in dosya istatistiği
    - `git log -p path/to/file`: belirli dosyada yapılan değişiklikler (patch ile)
    - `git log -- path/to/file`: belirli dosyanın geçmişi (diffsuz)

- Filtreler
    - `git log --author="Cihan" --since="2025-10-01" --until="2025-10-28"`
    - `git log --grep="fix|bug" -E`: mesajda regex eşleşen commitler

- Uzak repo ile fark (neyi push/pull edeceksin?):
    - `git fetch origin`
    - `git log --oneline origin/main..HEAD`: henüz push etmediklerin
    - `git log --oneline HEAD..origin/main`: uzakta olup sende olmayanlar
    - `git branch -vv`: her branch’in upstream durumu

- Kayıp commitleri bile kurtarmak için:
    - `git reflog`: HEAD’in geçmiş hareketleri (geri dönüş/kurtarma için altın değerinde)

## Yeni branch oluşturma ve yeni brach'i aktif etme
- `git fetch origin`
- `git switch main`: (eski gitlerde: git checkout main)
- `git pull --ff-only origin main`: main’i güncelle
- `git switch -c feature/cifar-aug`: yeni branch’i oluştur ve geç
- `git push -u origin feature/cifar-aug`: uzakta oluştur + upstream ayarla

## Sürümleme
- Sürümler SemVer ile etiketlenir (örn. `v0.1.0`, `v0.1.1`).
- Yayınlar annotated tag olarak işaretlenir.