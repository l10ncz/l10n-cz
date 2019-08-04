# L10N.cz

[![Build Status](https://api.travis-ci.com/l10ncz/l10ncz.svg?branch=master)](https://travis-ci.com/l10ncz/l10ncz)

Repositář pro web L10N.cz. Web používá generátor statických stránek [Jekyll](https://jekyllrb.com/).

## Úpravy obsahu

### Šablona
Web používá šablonu [ttskch/jekyll-ttskch-theme](https://github.com/ttskch/jekyll-ttskch-theme). Některé změny oproti ní se nachází v adresářích `_layouts`, `_pages`, `_sass` a `assets`.

### Obsah
Obsah všech stránek je v adresáři `_pages` a je psaný v HTML nebo Markdownu. Analogicky příspěvky na blog jsou v adresáři `_posts`. Pár stránek o Markdownu:
- [Mastering Markdown - GitHub Guides](https://guides.github.com/features/mastering-markdown/)
- [Basic writing and formatting syntax - User Documentation](https://help.github.com/articles/basic-writing-and-formatting-syntax/)
- [Syntax | kramdown](https://kramdown.gettalong.org/syntax.html)

### Příprava
Abyste byli schopni spustit níže uvedené příkazy, je nutné mít nainstalované [Ruby](https://www.ruby-lang.org/en/documentation/installation/) a [Bundler](https://bundler.io/#getting-started).

Před prvním zobrazením (nebo po změně souboru `Gemfile`) je potřeba stáhnout potřebné závislosti.
```
$ bundle install --path vendor/bundle
```

### Náhled
Při úpravách vzhledu i obsahu je dobré rovnou se podívat na výsledek. Níže uvedený příkaz sestaví obsah repositáře a zpřístupní ho na lokální adrese http://localhost:4000/.
```
$ bundle exec jekyll serve
```
Příkaz stačí spustit jednou v samostatném terminálu a nechat běžet. Pokud pak ve zdrojových souborech provedete nějakou změnu, Jekyll sestaví stránky znovu. Pro zobrazení efektu změn stačí obnovit načtenou stránku v prohlížeči (*F5*).

## Sestavení statické verze
Pro sestavení webu slouží tento příkaz.
```
$ bundle exec jekyll build
```
Statická verze stránek je vygenerovaná do adresáře `_site`. Pro nasazení stačí jeho obsah nahrát na server třeba přes FTP.
