<p align="center"><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/logo.svg"/></a><br/><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/xxai.svg"/></a></p><p align="center"><a href="https://github.com/xxai-art/doc#readme"><img alt="I18N" src="https://cdn.jsdelivr.net/gh/wactax/img/t.svg"/></a>　<a href="https://groups.google.com/u/0/g/xxai-art"><img alt="Google Groups" src="https://cdn.jsdelivr.net/gh/wactax/img/g-groups.svg"/></a></p>

# xxAI.art

Вебсайттын кодунун бир бөлүгү ачык булак болуп саналат, котормону оптималдаштырууга кош келиңиз.

## алдыңкы код

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
