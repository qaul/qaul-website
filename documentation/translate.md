# Translate the qaul.net Web Site

**The [qaul.net] web site is multilingual and can be translated into any language.**

## Translating a Content Page

Each page can be translated into any other Language.
To add a new language do the following things:

1. Add the new language to the configuration file `config.toml`. Add the new language to the existing configuration:

```
[languages]
  [languages.en]
    weight = 1
    LanguageName = "English"
  [languages.de]
    weight = 3
    LanguageName = "Deutsch"
  [languages.ar]
    weight = 2
    LanguageName = "العربية"
    rtl = true
```

2. Create a language specific CSS file in the folder `themes/hugo-theme-qaul/static/css/` (e.g. `themes/hugo-theme-qaul/static/css/fr.css` for French).
  * This file contains language specific configuration and will be mostly empty.
  * For right-to-left written languages copy the file for arabic 'ar.css'.

3. Translate the web site menu items. The web site menu items can be found in the folder `themes/hugo-theme-qaul/i18n`. There is a file for each language.
  * Copy the file `en.toml` and rename it according to your language.
  * Translate each sentence or word in `other = "TRANSLATE THIS PART"`.

4. Translate the content markdown files. The markdown files are in the `content` folder.
    * Copy 
    * Try to at least to translate the start page. The following files need to be translate for the start page:
        * `content/_index.md`
        * all files in the folder `content/home`

[qaul.net]: https://qaul.net
