# mezzio-static-pages

[![Build Status](https://github.com/mezzio/mezzio-static-pages/actions/workflows/continuous-integration.yml/badge.svg)](https://github.com/mezzio/mezzio-static-pages/actions/workflows/continuous-integration.yml)

> ## 🇷🇺 Русским гражданам
>
> Мы, участники Laminas, родились и живем в разных странах. У многих из нас есть друзья, родственники и коллеги как в России, так и в Украине. Некоторые из нас родились в России. Некоторые из нас живут в России. У некоторых бабушки и дедушки сражались с фашистами во Второй мировой войне. Здесь никто не поддерживает фашизм.
>
> У одного из нас есть украинская родственница, которая спаслась из дома вместе с сыном. Поезд задержался из-за бомбежки на дороге впереди. У нас есть друзья, которые прячутся в бомбоубежищах. Мы с тревогой ждем весточки от них после воздушных налетов, которые беспорядочно наносят удары и попадают по больницам, школам, детским садам и домам. Мы не берем это из каких-либо СМИ. Мы наблюдаем это напрямую.
>
> Вы доверяете нам достаточно, чтоб использовать наши программы, и мы просим вас довериться нам вновь. Мы нуждаемся в помощи. Выходите и протестуйте против этой бесполезной войны. Остановите кровопролитие. Скажите "Нет войне!"
>
> ## 🇺🇸 To Citizens of Russia
>
> We at Laminas come from all over the world. Many of us have friends, family and colleagues in both Russia and Ukraine. Some of us were born in Russia. Some of us currently live in Russia. Some have grandparents who fought Nazis in World War II. Nobody here supports fascism.
>
> One team member has a Ukrainian relative who fled her home with her son. The train was delayed due to bombing on the road ahead. We have friends who are hiding in bomb shelters. We anxiously follow up on them after the air raids, which indiscriminately fire at hospitals, schools, kindergartens and houses. We're not taking this from any media. These are our actual experiences.
>
> You trust us enough to use our software. We ask that you trust us to say the truth on this. We need your help. Go out and protest this unnecessary war. Stop the bloodshed. Say "stop the war!"

This library simplifies rendering static pages in [Mezzio](https://docs.mezzio.dev/mezzio/) applications.

> [!IMPORTANT]
> This module **does not** support laminas-mvc applications.

## Installation

Run the following to install this library:

```bash
$ composer require mezzio/mezzio-static-pages
```

If you want to automate the enabling of the module when running `composer require/install/update`, then your project needs to use https://github.com/laminas/laminas-component-installer[laminas/laminas-component-installer].
If it does, when the package is installed you'll be asked if you want to enable its [ConfigProvider](https://docs.laminas.dev/laminas-config-aggregator/config-providers/).
Answer with `Y` and the package will be ready to use.

If you don't use laminas-component-installer, or for some reason or other can't, then ensure that `\StaticPages\ConfigProvider::class,` is in the `ConfigAggregator` list in `config/config.php`, as in the example below.

```php
$aggregator = new ConfigAggregator(
    [
        \StaticPages\ConfigProvider::class,
    ]
);
```

## Documentation

Browse the documentation online at https://docs.mezzio.dev/mezzio-static-pages/

## Support

* [Issues](https://github.com/mezzio/mezzio-static-pages/issues/)
* [Forum](https://discourse.laminas.dev/)
