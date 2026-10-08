# EcoProve AI

Çevresel verilerin kullanılmadan önce güvenilirliğini değerlendiren, şüpheli veriyi silmeden karantinaya alan ve kararların kaydını blokzincirde izlenebilir yapan bir güven katmanı.

Track: Climate Data & Environmental Monitoring (IEEE Global ClimateChain Hackathon 2026)

## Durum
- [x] Üç veri kaynağını ortak şemaya getirme (`birlestir.py`)
- [x] Kaynaklar arası sapma ve eksik gün analizi (`analiz_A.py`)
- [x] Registry contract taslağı (`contracts/EcoProveRegistry.sol`), henüz deploy edilmedi
- [ ] Tahmin modeli, Reliability Score, Adaptive Trust
- [ ] Sahte hata testi (precision/recall)
- [ ] Backend, dashboard, testnet deploy

## Veri kaynakları (Ankara, 2020-2025)
- NASA POWER (MERRA-2), günlük: https://power.larc.nasa.gov/
- Open-Meteo (ERA5 reanalysis): https://open-meteo.com/
- NOAA GHCN-Daily, istasyon TUM00017130: https://www.ncei.noaa.gov/

## Çalıştırma
CSV dosyalarıyla aynı klasörde:
```
pip install pandas numpy matplotlib
python birlestir.py
python analiz_A.py
```

## İlgili çalışma
Heston TF (2026). A proof-of-stake blockchain framework for transparent climate data verification. PLOS Climate 5(6): e0000764. https://doi.org/10.1371/journal.pclm.0000764
