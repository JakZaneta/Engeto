# Postup, jak vyrobit CV

### 1. vyrobit html podklad (zatím bez formuláře dole)

### 2. v rámci ukázky css bylo přidáno:

```css
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

img {
  width: 150px;
  height: 150px;
  border-radius: 50%;
}

h1 {
  color: #333;
  margin-top: 30px;
  margin-bottom: 10px;
}

.footer-p {
  color: #666;
  margin-top: 20px;
}
```

### 3. přidání délkových měr

- celý kód obalit divem se třídou "container" a té nastavit maximální šířku na 800px (vlastnost `max-width`) a šířku na 90% (vlastnost `width`)
- třídě "container" dát vlastnost "vnitřní vycpávku" na 10px (vlastnost `padding`)
- třídu "container" vycentrovat - pomocí vlastnosti `margin: auto`
- všem nápisům h2 nastavit horní okraj a dolní okraj (`margin-top` a `margin-bottom`) na 30px a spodní padding nastavit na 5px (`padding-bottom`)

### 4. přidání barev

- nápisu "Frontend Developer" (těsně pod h1) přidat barvu "green"
- elementu h1 přidat barvu `#333`
- pozadí (tedy tagy body) přidat barvu se složkami red = 244, green = 244, blue = 244
- všechny barvy uložit do proměnných (barvu `#333`do proměnné `--main-color`, ostatní jakkoliv)
- `--main-color` přidat i nadpisům h2

### 5. jednotky délky a barvy

- všem tagům h2 přidat spodní ohraničení (vlastnost `border-bottom`) tak, aby byla 2px tlustá, nepřerušovaná a barva `var(--main-color)`
- třídě "container" přidat stín (vlastnost `box-shadow`, hodnoty: "posun dolů", "posun doleva", "velikost rozmazání", a "barva") - očekává tedy 3 délkové honodty a jednu barvu
- třídě "container" přidat zakulacení rohů (vlastnost `border-radius`) - hodnota např. px

### 6. vlastnosti textu

- přidat sekci "About me" a do ní přidat odstavec "Lorem Ipsum"
- textu v sekci about me nastavit zarování do bloku (vlstnost `text-align`)
- elementu h1 a odstavci pod ním nastavit zarovná na střed
- zarovnání na střed nastavit i obrázku
- všem seznamům odstranit tečky před itemy (vlastnost `list-style-type`)
- velikost písma "Fronted Developer" nastavit na 18px (vlastnost `font-size`)
- odkazy v textu napsat kurzívou, tučně a podtrženě(vlastnost `font-weight`, `font-style`, `text-decoration`)
- importovat font Ubuntu a pro celý html soubor nastavit font na něj (a kdybys se něco nepovedlo, tak sans-sarif) - vlastnost `font-family

### 7. přidání formuláře

- přidat formulář (tag `form`) a do něj jendotlivá okýnka - Jméno (`<input type="text">`), email (`<input type="email>`), vaše zpráva (`<textarea type="message">`),odeslat zprávu (`<input type="submit">`)
- všem přidat, že jsou povinné (atribut `required`)
- stylování: všechny inputy a textarea kromě submit dostanou šířku 100%, padding 10px, border-radius 5px, margin-bottom 10px, a border 1px solid --main-color
- stylování: submit: barva pozadí #4caf50, barva nápis bílá, padding 10px 20px, žádnou border, border-radius 5px
- submit po najetí myší: `cursor: pointer` a barva pozadí se změní na #45a049
