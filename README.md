# :goberserk: quoth_the_vikings - ᚲᚢᛟᛏᚺ_ᛏᚺᛖ_ᚹᛁᚲᛁᚾᚷᛋ :goberserk:
:godmode: The quoth_the_vikings action is an action that plucks a random sentence from one the Icelandic Sagas. :godmode:

:suspect: [![Quoth The Vikings](https://github.com/sturlabragason/quoth_the_vikings/actions/workflows/quoth.yml/badge.svg)](https://github.com/sturlabragason/quoth_the_vikings/actions/workflows/quoth.yml)
 `#actionshackathon21` :suspect:

:rage1: The [`sturlabragason/quoth_the_vikings`](https://github.com/sturlabragason/quoth_the_vikings) action is a composite action that grabs a random line in a random language from one of the Icelandic sagas. It incorporates the action: [`actions/checkout@v2`](https://github.com/actions/checkout). :rage1:

## :hurtrealbad: What this action does: (in old norse) :goberserk:

> Úr brunni Mímis, erut sagnir allar fengnar!
> Galdur magnast enn, ok á skjánum þulu myndar!
> Eigi erut rúnir ristar úr letri Væringja!
> Gerit menn þá allir, sem þeir skyldu met þulu þessa, gerist glaðir, ellegar notið til níðs!

## :rage4: What this action does (in plain english): :rage3:

- :suspect: First off, it downloads ALL of the icelandic sagas from [`sturlabragason/quoth_the_vikings`](https://github.com/sturlabragason/quoth_the_vikings)! :suspect:
- :hurtrealbad: It then picks a random sentence from a random saga, in a random language! :hurtrealbad:
- :rage1: It then replaces all letters of the latin alphabet with the ELDER FUTHARK! :rage1:
- :goberserk: Voila, use the output as you please: they make great automated commit messages, git tags or anything at all! :goberserk:


## :rage4: Usage :rage4:

```yaml
    steps:
      - id: quoth_the_vikings
        uses: sturlabragason/quoth_the_vikings@main
```
:godmode: To [use the quote](https://docs.github.com/en/actions/learn-github-actions/workflow-syntax-for-github-actions#jobsjob_idoutputs): :godmode:        
```yaml
      - name: Use the quote
        shell: pwsh
        run: echo ${{ steps.quoth_the_vikings.outputs.quote }}
```

## License :finnadie:

[GNU General Public License v3.0](https://github.com/sturlabragason/quoth_the_vikings/blob/main/LICENSE)