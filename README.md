<p align="center"><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/logo.svg"/></a><br/><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/xxai.svg"/></a></p><p align="center"><a href="https://github.com/xxai-art/doc#readme"><img alt="I18N" src="https://cdn.jsdelivr.net/gh/wactax/img/t.svg"/></a>　<a href="https://groups.google.com/u/0/g/xxai-art"><img alt="Google Groups" src="https://cdn.jsdelivr.net/gh/wactax/img/g-groups.svg"/></a></p>

Каталогго киргенден кийин адегенде nodejs, [direnv](https://direnv.net) , [bun](https://github.com/oven-sh/bun) орнотуу сунушталат, андан кийин `direnv allow` ( [.envrc](https://github.com/xxai-art/doc/blob/main/.envrc) каталогго киргенден кийин автоматтык түрдө аткарылат).

Мааниси: кытай тилинен жапон, корей, англис, англис тилинен башка бардык тилдерге котормо. Эгер сиз кытай жана англис тилин гана колдогуңуз келсе, `zh: en` деп жазсаңыз болот.

Мааниси: кытай тилинен жапон, корей, англис, англис тилинен башка бардык тилдерге котормо. Эгер сиз кытай жана англис тилин гана колдогуңуз келсе, `zh: en` деп жазсаңыз болот.

* [алдыңкы код](https://github.com/xxai-art/web)
* [Бүтүндөй сайт үчүн тил пакеттери](https://github.com/xxai-art/web/tree/main/i18n)
* [Кирүү модулдары үчүн тил пакеттери](https://github.com/wacpkg/user/tree/main/ui.i18n)
* [Вебсайттын көп тилдүү документтери](https://github.com/xxai-doc)

Алдын ала программалоо тили [@w5/coffee_plus](http://npmjs.com/@w5/coffee_plus) , ал кофескрипт синтаксисинин негизинде кээ бир функцияларды кошот, караңыз [./coffee_plus.md](./coffee_plus.md) .

## Веб-сайттарды жана документтерди интернационалдаштыруу

Төмөнкү 3 долбоордун үстүнөн куруңуз

* [@w5/mdt](https://www.npmjs.com/package/@w5/mdt)

  Суффикс `.mdt` , сиз тышкы файлдарга кайрылуу үчүн `<+ ./coffee_plus/import.js>` окшош синтаксисин колдоно аласыз жана `.md` суффикси менен белгилерди түзө аласыз.

* [@w5/trmd](https://www.npmjs.com/package/@w5/trmd)

  Markdown котормосу коддорду жана шилтемелерди которбойт жана которулган сүйлөмдөрдү кэштейт. Эгерде котормо өзгөртүлсө, бирок түпнуска текст өзгөртүлбөсө, аны кайра аткаруу котормодогу өзгөртүүнү кайра жазбайт.

* [@w5/i18n](https://www.npmjs.com/package/@w5/i18n)

  `yaml` түзүлгөн веб-сайттарды которуу үчүн тил файлдары.

### Документти которууну автоматташтыруу боюнча нускамалар

[xxai-art/doc](https://github.com/xxai-art/doc) код репозиторийин караңыз

Каталогго киргенден кийин адегенде nodejs, [direnv](https://direnv.net) , [bun](https://github.com/oven-sh/bun) орнотуу сунушталат, андан кийин `direnv allow` ( [.envrc](https://github.com/xxai-art/doc/blob/main/.envrc) каталогго киргенден кийин автоматтык түрдө аткарылат).

Жүздөгөн тилдерге которулган чоң коддук базаны болтурбоо үчүн, мен ар бир тил үчүн өзүнчө код базасын түздүм жана код базасын сактоо үчүн уюм түздүм.

`GITHUB_ACCESS_TOKEN` чөйрө өзгөрмөсүн коюу жана андан кийин [create.github.coffee](https://github.com/xxai-art/doc/blob/main/create.github.coffee) иштетүү код репозиторийин автоматтык түрдө түзөт.

Албетте, сиз аны коддук базага да койсоңуз болот.

Котормо скриптинин шилтемеси [run.sh](https://github.com/xxai-art/doc/blob/main/run.sh)

Скрипт коду төмөнкүчө чечмеленет:

[bunx](https://bun.sh/docs/cli/bunx) тезирээк npx үчүн алмаштыруу болуп саналат. Албетте, сизде булочка орнотулган жок болсо, анын ордуна `npx` колдонсоңуз болот.

`bunx mdt zh` `.mdt` zh каталогунда `.md` катары көрсөтөт, төмөнкү шилтемеленген 2 файлды караңыз

* [coffee_plus.mdt](https://github.com/xxai-doc/zh/blob/main/coffee_plus.mdt)
* [coffee_plus.md](https://github.com/xxai-doc/zh/blob/main/coffee_plus.md)

`bunx i18n` котормонун негизги коду (эгерде сизде `nodejs` гана орнотулган болсо, бирок `bun` жана `direnv` орнотулбаса, которуу үчүн `npx i18n` да иштетсеңиз болот).

Ал [i18n.yml](https://github.com/xxai-art/doc/blob/main/i18n.yml) талдайт, бул документте `i18n.yml` конфигурациясы төмөнкүдөй:

```
en:
zh: ja ko en
```

Мааниси: кытай тилинен жапон, корей, англис, англис тилинен башка бардык тилдерге котормо. Эгер сиз кытай жана англис тилин гана колдогуңуз келсе, `zh: en` деп жазсаңыз болот.

Акыркысы [gen.README.coffee](https://github.com/xxai-art/doc/blob/main/gen.README.coffee) болуп саналат, ал `README.md` жазуусун түзүү үчүн ар бир тилдин `README.md` негизги аталышы менен биринчи субтитринин ортосундагы мазмунду чыгарат. Код абдан жөнөкөй, аны өзүңүз карасаңыз болот.

Google API акысыз которуу үчүн колдонулат. Эгер Google'га кире албасаңыз, проксиди конфигурациялап, орнотуңуз, мисалы:

```
export https_proxy=http://127.0.0.1:7890 http_proxy=http://127.0.0.1:7890 all_proxy=socks5://127.0.0.1:7890
```

Котормо скрипти `.i18n` каталогунда которулган кэшти жаратат, аны `git status` менен текшерип, кайталанма котормолорду болтурбоо үчүн код репозиторийине кошуңуз.

Кэшти жаңыртуу үчүн котормону өзгөрткөн сайын `bunx i18n` иштетиңиз.

Эгерде түпнуска текст менен котормо бир эле учурда өзгөртүлсө, кэш чаташып калат, андыктан сиз өзгөрткүңүз келсе, бирөөнү гана өзгөртүп, андан кийин кэшти жаңыртуу үчүн `bunx i18n` иштете аласыз.
