# Lezione 1

Utilizzeremo HTML, CSS, e JavaScript per creare un Design System minimale utilizzando SASS. Prima di iniziare assicuratevi di aver installato sul vostro sistema operativo l'ultima release LTS di Node.js.

## Installazione di Node.js

Vai sul [sito di Nodejs](https://nodejs.org/en/) e scarica la versione LTS (attualmente la 16.x.x). Se sei un utente Windows o Mac avrai a disposizione un installer guidato per il tuo sistema operativo. Con pochi click riuscirai ad installare Node.js correttamente.

## SASS

Sass preprocessore CSS. Ti consente di utilizzare variabili, regole nidificate, mixin, funzioni e altro, il tutto con una sintassi completamente compatibile con i CSS. Sass aiuta a mantenere i fogli di stile di grandi dimensioni ben organizzati e semplifica la condivisione del design all'interno e tra i progetti.

Dai uno sguardo alla [documentazione ufficiale](https://sass-lang.com/) per maggiori dettagli :smile:

### Installare SASS 

Per installare SASS sulla vostra macchina basta digitare dalla linea di comando quanto segue

```
$ npm install -g sass
```

Se tutto è andato a buon fine digitando il comando `sass` dal terminale dovrebbe apparire quanto segue:

```
$ sass

Usage: sass <input.scss> [output.css]
       sass <input.scss>:<output.css> <input/>:<output/> <dir/>

━━━ Input and Output ━━━━━━━━━━━━━━━━━━━
    --[no-]stdin               Read the stylesheet from stdin.
    --[no-]indented            Use the indented syntax for input from stdin.
-I, --load-path=<PATH>         A path to use when resolving imports.
                               May be passed multiple times.
-s, --style=<NAME>             Output style.
                               [expanded (default), compressed]
    --[no-]charset             Emit a @charset or BOM for CSS with non-ASCII characters.
                               (defaults to on)
    --[no-]error-css           When an error occurs, emit a stylesheet describing it.
                               Defaults to true when compiling to a file.
    --update                   Only compile out-of-date stylesheets.

━━━ Source Maps ━━━━━━━━━━━━━━━━━━━━━━━━
    --[no-]source-map          Whether to generate source maps.
                               (defaults to on)
    --source-map-urls          How to link from source maps to source files.
                               [relative (default), absolute]
    --[no-]embed-sources       Embed source file contents in source maps.
    --[no-]embed-source-map    Embed source map contents in CSS.

━━━ Other ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
-w, --watch                    Watch stylesheets and recompile when they change.
    --[no-]poll                Manually check for changes rather than using a native watcher.
                               Only valid with --watch.
    --[no-]stop-on-error       Don't compile more files once an error is encountered.
-i, --interactive              Run an interactive SassScript shell.
-c, --[no-]color               Whether to use terminal colors for messages.
    --[no-]unicode             Whether to use Unicode characters for messages.
-q, --[no-]quiet               Don't print warnings.
    --[no-]quiet-deps          Don't print compiler warnings from dependencies.
                               Stylesheets imported through load paths count as dependencies.
    --[no-]verbose             Print all deprecation warnings even when they're repetitive.
    --[no-]trace               Print full Dart stack traces for exceptions.
-h, --help                     Print this usage information.
    --version                  Print the version of Dart Sass.
```

### Come utilizzare SASS in questo progetto

Dalla directory principale del progetto eseguite questo comando:

```
sass --watch ./ui-kit/sass/ui-kit.scss:./ui-kit/css/ui-kit.css
```

Da questo momento in poi ogni volta che un file `.scss` verrà modificato SASS si preoccuperà di trasformare il codice in puro CSS. Trovate il codice css generato nella directory `ui-kit/css/ui-kit.css`.


## Obiettivo della lezione

Utilizzando SASS e JavaScript bisogna realizzare i seguenti componenti per il nostro UI Kit:

- [ ] Typography
- [ ] Spacing utilities
- [ ] Alerts
- [ ] Badges
- [ ] Buttons
- [ ] Button Groups
- [ ] Cards
- [ ] Forms
- [ ] Navs & Tabs
- [ ] Navbar
- [ ] Grid System
