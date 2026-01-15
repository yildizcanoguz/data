HM_APP (Hakediş & Maliyet) - Kurulum

1) Klasör yapısı:
hm_app/
  index.html
  data/
    jobs.json
    machines.json

2) Çalıştırma:
- En sorunsuz: klasörde terminal aç ->  python3 -m http.server 8000
  sonra tarayıcı: http://localhost:8000/hm_app/index.html

- Alternatif: sadece çift tıkla açacaksan (file://):
  İlk açılışta JSON fetch çalışmayabilir. Bu durumda sayfada:
  "Excel’den Güncelle" butonuyla Excel dosyanı seç, data lokal cache’e kaydolur.

3) Excel Import:
- Mevcut Excel dosyandaki 'Base_de_donnée' sheet'i otomatik okunur.
- Makine listesini Excel’den de almak istersen, 'Machines' adında yeni bir sheet aç:
  Kolonlar: name | daily
  Örnek satır: Ekskavatör | 40000

4) Export:
- Gelir CSV / Excel (CSV) / JSON butonları ile indir.
