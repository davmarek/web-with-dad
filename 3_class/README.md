
# Třídy (class)
Třídy slouží k označení HTML prvku, aby jsme mohli jednomu typu tagu (např. `<p>` jako paragraf) nastavovat různé styly, podle toho do jaké třídy patří.

**Každý prvek/tag v HTML může mít vlastnost `class`.**

## Jednu třídu může mít hodně prvků

```html
<p class="modra">Tento text je modry</p>

<h1 class="modra">Tento nadpis je modry</h1>
```

## Jeden prvek může mít hodně tříd
Musíme je akorát oddělit mezerami.
```html
<p class="modra cervena">Text s třídama: modra cervena</p>
```

> ❗️ Název třídy nemůže obsahovat mezery. Místo mezer použijeme třeba pomlku. (`nazev-dlouhe-tridy`)


# Stylování třídy v CSS
Když chceme nastavit nějaké styly vybrané třídě (např. `modra`), napíšeme před její název tečku.

```css
.modra {
  color: blue;
}
```

Pokud chceme vybrat pouze nadpisy s touto třídou:
```css
h1.modra {
  color: blue;
}
```

Pokud chceme vybrat nadpisy a paragrafy s touto třídou (oddělujeme čárkou):
```css
h1.modra,
p.modra {
  color: blue;
}
```