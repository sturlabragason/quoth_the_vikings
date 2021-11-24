# quoth_the_vikings
The quoth_the_vikings action is an action that plucks a random sentence from one the Icelandic Sagas.

[![Quoth The Vikings](https://github.com/sturlabragason/quoth_the_vikings/actions/workflows/quoth.yml/badge.svg)](https://github.com/sturlabragason/quoth_the_vikings/actions/workflows/quoth.yml)
`#actionshackathon21`

The [`sturlabragason/quoth_the_vikings`](https://github.com/sturlabragason/quoth_the_vikings) action is a composite action that grabs a random line in a random language from one of the Icelandic sagas. It incorporates the action: [`actions/checkout@v2`](https://github.com/actions/checkout).

## 🪓🛡️ What this action does: (in old norse) 🪓🛡️

> Úr brunni Mímis, erut sagnir allar fengnar!
> Galdur magnast enn, ok á skjánum þulu myndar!
> Eigi erut rúnir ristar úr letri Væringja!
> Gerit menn þá allir, sem þeir skyldu met þulu þessa, gerist glaðir, ellegar notið til níðs!

## :rocket: What this action does (in plain english): :rocket:

- 🛠️ First off, it downloads ALL of the icelandic sagas from [`sturlabragason/quoth_the_vikings`](https://github.com/sturlabragason/quoth_the_vikings)!
- It then picks a random sentence from a random saga, in a random language!
- It then replaces all letters of the latin alphabet with the ELDER FUTHARK! 
- Voila, use the output as you please: they make great automated commit messages, git tags or anything at all!


## Usage

```yaml
jobs:
  quoth_the_vikings_job:
    name: Using quoth_the_vikings action
    steps:
      - id: quoth_the_vikings
        uses: sturlabragason/quoth_the_vikings@main
      - name: Use the quote
        shell: pwsh
        run: echo ${{ steps.quoth_the_vikings.outputs.quote }}
```

## License

[GNU General Public License v3.0](https://github.com/sturlabragason/quoth_the_vikings/blob/main/LICENSE)