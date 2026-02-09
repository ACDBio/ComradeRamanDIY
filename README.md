# ComradeRamanDIY
A DIY 3D printed Raman system with a CCD spectrometer using based on 90° scattering geometry and 780 nm laser. Adjustment-free.

This repository documents the physical Raman system: overview, .stl and FreeCad files for 3d printing, bill of materials, and examples of the acquired spectra.
Software used only for calibration, data acquisition, processing, visualization, and search in reference databases is available [here](https://github.com/ACDBio/raman-open-forge-imai).
---

## About the system

ComradeRamanDIY is a Raman setup built from commercially available components and custom 3D-printed mechanics.

Key design choices:

- 90° collection geometry   
- external TEC cooling of the CCD spectrometer  
- stack of budget filters for effective filtration of the laser line

The system was designed for stable measurement of liquid samples in cuvettes.
---

## Current system performance
Comparison of the DMSO spectra obtained with the system and the mprofessional probe after Raman shift [software](https://github.com/ACDBio/raman-open-forge-imai) calibration. 
![DMSO spectra comparison](https://github.com/ACDBio/ComradeRamanDIY/blob/main/Screenshot%20from%202026-02-09%2009-05-09.png)

After system calibration with [YM_RPL_785_500](https://aliexpress.ru/item/1005010193725685.html?spm=a2g2w.orderdetail.0.0.20384aa6LKfzBg&sku_id=12000051478540187&_ga=2.6013747.1429933141.1770309479-1631170546.1742897773), DIY spectra peak positions match the reference database spectra (from ramanbase.org) without re-calibration.
E.g. for isopropyl alcohol:
![Isopropyl alcohol](https://github.com/ACDBio/ComradeRamanDIY/blob/main/Screenshot%20from%202026-02-09%2009-01-47.png)

---

## BILL OF MATERIALS
Total cost (with a new CCD spectromter): ~1800 USD
1. PETG 3d printing filament for printing the .stl
2. 800 nm long-pass filters 4-14 pieces (the current system uses 14 pieces but the quality of spectra don't change substantially from 4 pieces). We used 5.9x5.9 mm IR camera filters from [this shop](https://aliexpress.ru/store/911601353?spm=a2g2w.orderdetail.0.0.18794aa6WkrNWx&page=3) for ~ 2$. 1-2 filters from [here](https://aliexpress.ru/item/1005009606845139.html?spm=a2g2w.orderdetail.0.0.10bb4aa6kRWllm&sku_id=12000049611215568&_ga=2.133597321.606840197.1770619478-1631170546.1742897773) also work, but you will need to adjust the cuvette holder.
4. [NF780 Narrow Band filter](https://aliexpress.ru/item/1005008883212898.html?spm=a2g2w.orderdetail.0.0.d7e94aa6Bp8xzT&sku_id=12000047075793792&_ga=2.26257338.606840197.1770619478-1631170546.1742897773) for laser cleaning.
5. [15 degree LED lens](https://aliexpress.ru/item/32820431045.html?spm=a2g2w.orderdetail.0.0.75834aa6qalnJD&sku_id=64707315106&_ga=2.189769388.606840197.1770619478-1631170546.1742897773) for light collection (is inserted in the cuvette holder)
6. [Quartz cuvette](https://aliexpress.ru/item/32793982308.html?spm=a2g2w.orderdetail.0.0.2bdd4aa6R19moS&sku_id=63840647083&_ga=2.17671998.606840197.1770619478-1631170546.1742897773) 10 mm light path
7. [IRM785 CCD spectrometer](https://aliexpress.ru/item/1005009187077048.html?spm=a2g2w.orderdetail.0.0.671d4aa6tsgBNN&sku_id=12000048233983566&_ga=2.33651750.606840197.1770619478-1631170546.1742897773)
8. [SZMCTV 1/2 Microscope Camera Adapter](https://aliexpress.ru/item/32855848880.html?spm=a2g2w.favourites.0.0.778e4aa6S5wLJN&sku_id=10000001989770343) for laser focusing
9. [TEC1-12715](https://aliexpress.ru/item/1005003070412441.html?shpMethod=CAINIAO_ECONOMY&sku_id=12000023786453944&spm=a2g2w.productlist.search_results.5.53b447bfnGnVcq) for CCD spectrometer cooling with the radiator (here - a 7х8 cm copper one was used) and a fan.

# Acknowledgments
Special thanks to [Imai Optics](http://www.imaioptics.com/) for supporting the project by providing a discount on [YM_RPL_785_500](https://aliexpress.ru/item/1005010193725685.html?spm=a2g2w.orderdetail.0.0.20384aa6LKfzBg&sku_id=12000051478540187&_ga=2.6013747.1429933141.1770309479-1631170546.1742897773), which was instrumental in testing the setup during development.
Also thyanks to [ramanbase.org](https://ramanbase.org/) developers and contributors and ramanspy developers.

The cuvette holder provided here can also be used with [Imai Optics](http://www.imaioptics.com/) probe [YM_RPL_785_500](https://aliexpress.ru/item/1005010193725685.html?spm=a2g2w.orderdetail.0.0.20384aa6LKfzBg&sku_id=12000051478540187&_ga=2.6013747.1429933141.1770309479-1631170546.1742897773).

