# Diapositiba elebakar paraleloak

[Hau](https://juanabasolo.github.io/ehu-revealjs/elebakarparaleloak/) egiteko erabili dudan kodea.

## Azalpen laburra

1. Konpilatzean fitxategi bi sortzen ditu, batak agintzen du eta besteak aginduak jaso.
1. Hori gertatzeko revealjs-k erabili behar du Multiplex gehigarria eta horri pasatu behar zaizkio `secret` eta `sockedID` aldagaietako balioak. 
1. Fitxategi bakarra sortu beharrean, hizkuntzako bat sortu behar da aldagai berberak erabilita.
1. Agindu behar ez duten fitxategiak, jaurti (nire kasuan, euskara bantuaz ez dauden fitxategi agintari guztiak)
1. Eroan webgunera
1. Pasa esteka(k) audientziari.
1. Egin aurkezpena

## Kasu zehatz honetakoak

### kontuan izatekoak

* Nik Quarto darabilt 
* EHUko itxurako txantiloiak darabiltzat
* Dena fitxategi bakarrean sortzea eskatzen diot, errazago erabiltzeko
* Irtera karpeta bat zehaztu dot html-ak horra sortzeko (eta gitpagesen argitaratzeko), baina horra ez dau sortzen berez fitxategi agintaria.

Quarton sortzen dituen fitxategiak dira:

+ fitxategia.html audientziarako
+ fitxategia-speaker.html hizlariarentzat

Zehatzako ikus daiteke kodean nik zelan egin dodan, honelako burua behar luke estandar parebatek

```yaml
title: "Izenburua"
subtitle: Azpi izenburua
author: "Hizlariaren izen-abizenak-edo"
date: today
format: 
    revealjs:
        embed-resources: true # Fitxategi bakarrean nahi bada
        multiplex: 
            id: 'x0x0x0x0x0x0x' # eGokitu zurearekin
            secret: 'asdasdfasdfasdfa' # egokitu zurearekin
```

`id` eta `secret` aldagaietarako balioak nik hemen sortu ditut: https://reveal-multiplex.glitch.me/  
Hor Multiplex-ekoek zerbitzari bat dutelako erabilera publikorako prest. Baina norberarena ere sor omen daiteke. Berez, gorago aipatutako `secret` eta `sockedID` aldagaiak dira

Quartoko webgunean [horren gaineko informazioa](https://quarto.org/docs/presentations/revealjs/presenting.html#multiplex)
