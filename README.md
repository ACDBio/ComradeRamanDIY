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

The cuvette holder provided here can also be used with [Imai Optics](http://www.imaioptics.com/) probe [YM_RPL_785_500](https://aliexpress.ru/item/1005010193725685.html?spm=a2g2w.orderdetail.0.0.20384aa6LKfzBg&sku_id=12000051478540187&_ga=2.6013747.1429933141.1770309479-1631170546.1742897773).

---

## Current system performance
Comparison of the DMSO spectra obtained with the system and the mprofessional probe after Raman shift [software](https://github.com/ACDBio/raman-open-forge-imai) calibration. 
![DMSO spectra comparison](https://github.com/ACDBio/ComradeRamanDIY/blob/main/Screenshot%20from%202026-02-09%2009-05-09.png)

After system calibration with [YM_RPL_785_500](https://aliexpress.ru/item/1005010193725685.html?spm=a2g2w.orderdetail.0.0.20384aa6LKfzBg&sku_id=12000051478540187&_ga=2.6013747.1429933141.1770309479-1631170546.1742897773), DIY spectra peak positions match the reference database spectra (from ramanbase.org) without re-calibration.
E.g. for isopropyl alcohol:
![Isopropyl alcohol](https://github.com/ACDBio/ComradeRamanDIY/blob/main/Screenshot%20from%202026-02-09%2009-01-47.png)
