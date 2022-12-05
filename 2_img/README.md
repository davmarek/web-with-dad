# Obrázky na webu
- tag `<img>`
  - neukončuje se
  - **musí** mít atribut `src` = cesta k obrázku
  - **měl by** mít atribut `alt` = název obrázku, který se zobrazí pokud se obrázek nenačte

```html
<img src="cesta/k/obrazku.jpg">
```

# Cesta k obrázku
- v jaké složce je umístěn, relativně k aktuálnímu souboru html + název obrázku

## Jak určit cestu
Řekněme, že ve složce s naším projektem máme soubor `index.html` a složku `obrazky`.

V souboru `index.html` chceme zobrazit obrázek `pes.jpg`, který je ve složce `obrazky`.

Cesta bude vypadat následovně:
```
obrazky/pes.jpg
```
Celý `img` tag bude vypadat takto:
```html
<img src="obrazky/pes.jpg" alt="pes">
```
## Hloubější cesty
Cesta může být i mnohem složitější a jít do více složek:
```
slozka/obrazky/zvirata/pes.jpg
```

## Cesty ven ze složky
Pokud máme soubor v nějaké složkce a chceme odkázat na soubor, který se nachází v nadřazené složce, použijeme `..` abychom se _"dostali z aktuální složky"_.

```
../obrazky/pes.jpg
```