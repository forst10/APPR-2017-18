# Analiza podatkov s programom R, 2017/18

Repozitorij z gradivi pri predmetu APPR v študijskem letu 2017/18

## Analiza donosnosti investicij v ICO-te

Za projekt sem si izbral analizo donosnosti investicij v ICO-te. 

"ICO" (initial coin offering) oz. "TGE" (token generation event) oz. "TDE"" (token distribution event) oz. "TS"" (token sale) pomeni prvo ponudbo prodaje kriptokovancev oziroma kriptožetonov. Gre za način množičnega financiranja, ki zagonskim podjetjem zagotovi financiranje - podjetje izda svoj kriptožeton (token) v zameno za plačilo s kriptovaluto. ICO-ti v zadnjem času rastejo kot gobe po dežju, v letu 2017 je bilo na ta način zbranih že več kot 3,5 miljarde ameriških dolarjev. Zaradi opevanih visokih donosnosti ICO-ti privabljajo ogromno investitorjev (tudi neizkušenih), ki mnogokrat na slepo vložijo svoj denar in večinoma tudi dobro zaslužijo. Zato sem se odločil, da raziščem to področje in analiziram, kakšne so možnosti za zaslužek, kolikšna je donosnost v povprečju, itd.

Izbral si bom neko borzo s kriptožetoni (npr. HitBTC) in pridobil podatke o cenah v določenih obdobjih, te pa bom primerjal s ceno žetona, po kateri ga je pridobil investitor v času ICO-ta in tako dobil razliko (zaslužek/izgubo).

## Program

Glavni program in poročilo se nahajata v datoteki `projekt.Rmd`. Ko ga prevedemo,
se izvedejo programi, ki ustrezajo drugi, tretji in četrti fazi projekta:

* obdelava, uvoz in čiščenje podatkov: `uvoz/uvoz.r`
* analiza in vizualizacija podatkov: `vizualizacija/vizualizacija.r`
* napredna analiza podatkov: `analiza/analiza.r`

Vnaprej pripravljene funkcije se nahajajo v datotekah v mapi `lib/`. Podatkovni
viri so v mapi `podatki/`. Zemljevidi v obliki SHP, ki jih program pobere, se
shranijo v mapo `../zemljevidi/` (torej izven mape projekta).

## Potrebni paketi za R

Za zagon tega vzorca je potrebno namestiti sledeče pakete za R:

* `knitr` - za izdelovanje poročila
* `rmarkdown` - za prevajanje poročila v obliki RMarkdown
* `shiny` - za prikaz spletnega vmesnika
* `DT` - za prikaz interaktivne tabele
* `maptools` - za uvoz zemljevidov
* `sp` - za delo z zemljevidi
* `digest` - za zgoščevalne funkcije (uporabljajo se za shranjevanje zemljevidov)
* `readr` - za branje podatkov
* `rvest` - za pobiranje spletnih strani
* `reshape2` - za preoblikovanje podatkov v obliko *tidy data*
* `dplyr` - za delo s podatki
* `gsubfn` - za delo z nizi (čiščenje podatkov)
* `ggplot2` - za izrisovanje grafov
* `extrafont` - za pravilen prikaz šumnikov (neobvezno)
