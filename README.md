# Porównanie modeli interpolacji wideo (Video Interpolation Models Comparison - VIMC)

To repozytorium zawiera porównanie czterech popularnych modeli interpolacji wideo: RIFE, DAIN, XVFI oraz FLAVR. Wszystkie testy zostały przeprowadzone z następującymi parametrami:
- Mnożnik klatek: x2
- Docelowa liczba klatek: 60 FPS
- Precyzja: pełna

Użyto [Flowframes GUI dla Windows](https://github.com/n00mkrad/flowframes)

### Original input video


https://github.com/user-attachments/assets/c621fb7c-cb8e-4772-908b-2431c304202f




## RIFE (Recursive Frame Interpolation)

### RIFE v3.0



https://github.com/user-attachments/assets/2cb04fac-67ba-4388-b26d-252e8b2cd76c



### RIFE v4.0



https://github.com/user-attachments/assets/1c37abed-8c47-4f88-a14f-1967638305d9



## DAIN (Depth-Aware Video Frame Interpolation)



https://github.com/user-attachments/assets/1c2623e8-1b78-4864-9a77-f980b95ae690



## XVFI (X-Video Frame Interpolation)

### XVFI - trenowany na Vimeo90K



https://github.com/user-attachments/assets/dd378596-099c-48cf-a16e-4dc9d16b6b1c



### XVFI - trenowany na X4K1000



https://github.com/user-attachments/assets/a9693e36-594f-489a-9377-a40cbe29e37b



## FLAVR (Flow-Agnostic Video Representations)



https://github.com/user-attachments/assets/62d6e33c-20d7-4fbe-80e7-214b9549d036



## Szczegóły techniczne

Każdy z modeli ma swoje unikalne podejście do interpolacji:

### RIFE
- Wykorzystuje rekurencyjne podejście do interpolacji
- v3.0 wprowadził ulepszoną stabilność
- v4.0 oferuje lepszą wydajność i dokładność

### DAIN
- Wykorzystuje mapy głębi do lepszego przewidywania ruchu
- Szczególnie skuteczny w scenach z różnymi planami głębi

### XVFI
- Wersja Vimeo90K zoptymalizowana pod kątem typowych scenariuszy wideo
- Wersja X4K1000 specjalnie dostosowana do materiałów w wysokiej rozdzielczości

### FLAVR
- Nie polega na jawnej estymacji przepływu optycznego
- Wykorzystuje reprezentacje czasowo-przestrzenne

## Instrukcje

Aby użyć odpowiednich modeli, zastąp znaczniki [video_*] właściwymi plikami wideo przedstawiającymi wyniki interpolacji. Zalecane jest użycie tego samego materiału źródłowego dla wszystkich modeli, aby zapewnić uczciwe porównanie.

## Uwagi

- Wszystkie testy zostały przeprowadzone na tym samym sprzęcie
- Zachowano identyczne parametry interpolacji dla wszystkich modeli
- Materiał źródłowy był ten sam dla wszystkich testów

## Citations

```bibtex
@inproceedings{huang2022rife,
  title={Real-Time Intermediate Flow Estimation for Video Frame Interpolation},
  author={Huang, Zhewei and Zhang, Tianyuan and Heng, Wen and Shi, Boxin and Zhou, Shuchang},
  booktitle={Proceedings of the European Conference on Computer Vision (ECCV)},
  year={2022}
}
```
```bibtex
@article{ma2024latte,
  title={Latte: Latent Diffusion Transformer for Video Generation},
  author={Ma, Xin and Wang, Yaohui and Jia, Gengyun and Chen, Xinyuan and Liu, Ziwei and Li, Yuan-Fang and Chen, Cunjian and Qiao, Yu},
  journal={arXiv preprint arXiv:2401.03048},
  year={2024}
}
```
```bibtex
@inproceedings{DAIN,
    author    = {Bao, Wenbo and Lai, Wei-Sheng and Ma, Chao and Zhang, Xiaoyun and Gao, Zhiyong and Yang, Ming-Hsuan}, 
    title     = {Depth-Aware Video Frame Interpolation}, 
    booktitle = {IEEE Conference on Computer Vision and Pattern Recognition},
    year      = {2019}
}
```
```bibtex
@inproceedings{sim2021xvfi,
  title={XVFI: eXtreme Video Frame Interpolation},
  author={Sim, Hyeonjun and Oh, Jihyong and Kim, Munchurl},
  booktitle={Proceedings of the IEEE International Conference on Computer Vision (ICCV)},
  year={2021}
}
```
```bibtex
@article{kalluri2023flavr,
  title={FLAVR: Flow-Agnostic Video Representations for Fast Frame Interpolation},
  author={Kalluri, Tarun and Pathak, Deepak and Chandraker, Manmohan and Tran, Du},
  booktitle={WACV},
  year={2023}
}
```
---

*Uwaga: To porównanie służy celom edukacyjnym i badawczym.
