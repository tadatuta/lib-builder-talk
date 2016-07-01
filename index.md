---

layout: default

---

# Яндекс

## **{{ site.presentation.title }}** {#cover}

<div class="s">
    <div class="service">{{ site.presentation.service }}</div>
</div>

{% if site.presentation.nda %}
<div class="nda"></div>
{% endif %}

<div class="info">
	<p class="author">{{ site.author.name }}, <br/> {{ site.author.position }}</p>
</div>

## **![](pictures/no-docs.gif)**

## **Документация — это хорошо**

## **Автогенерируемая документация — лучше!**

## **Что есть**

## Что есть
* [Сайт Лего](https://lego.yandex-team.ru/libs/islands/v3.8.0/desktop/button2/)
* ...[bem.info](https://ru.bem.info/libs/bem-components/v2.4.0/showcase/)
* ...[bem-site-engine](https://github.com/bem/bem-site-engine/)

## Что еще
* [bem-site](https://github.com/bem-site)
* ...bem-data-source
* ...provider
* ...bse-admin
* ...mds-wrapper
* ...builder-libraries
* ...snapshot-master
* ...builder-sitemap-xml

## Что еще
* dependency-updater
* ...snapshot-cleaner
* ...bem-md-renderer
* ...и так далее...

## **![](pictures/vegas.jpg)**

## **Что появилось**

## **[bem-lib-site](#)**

## **Как устроено**

## Как устроено
* bem-lib-site
    * ...bem-lib-site-data
    * ...bem-lib-site-view

## bem-lib-site-data
* Ставит зависимости
* ...Собирает интроспекцию о всех БЭМ-сущностях
    * ...Пути к исходным файлам блоков со всех уровней
    * ...Пути к кастомным файлам примеров

## bem-lib-site-data
* Ставит зависимости
* Собирает интроспекцию о всех БЭМ-сущностях
* Собирает документацию
    * ...block.{lang}.md (с учетом инлайновых примеров)
    * ...JSDoc


## bem-lib-site-data
* Ставит зависимости
* Собирает интроспекцию о всех БЭМ-сущностях
* Собирает документацию
* Собирает примеры
    * ...Живые, в iframe
    * ...HTML
    * ...BEMJSON
    * ...deps

## bem-lib-site-data
* Ставит зависимости
* Собирает интроспекцию о всех БЭМ-сущностях
* Собирает документацию
* Собирает примеры
* Общие readme, migration, changelog
* ...На выходе JSON и файлы примеров

## Структура данных
~~~
library
    version
        gh: '',
        readme: '',
        changelog: ''
        migration: ''
        sets
            desktop
                button
                    docs: ''
                    jsdoc: ''
                    examples: ''
                    sources: ''
~~~

## bem-lib-site-view
* Типичный БЭМ-проект
* ...Можно использовать как уровень переопределения
* ...Можно запилить свой
* ...На вход результат работы bem-lib-site-data
* ...На выходе статичный сайт

## **![](pictures/howto.gif)**

## **Как использовать**

## Как использовать
~~~
npm i bem-lib-site
bem-lib-site path/to/my/lib
~~~

## Конфигурация
~~~
'bem-lib-site-data': {
    tempFolder: 'tmp',
    outputFolder: 'output',
    platforms: { desktop: ['common', 'deskpad', 'desktop'] },
    libs: {
        'bem-components': {
            langs: ['ru', 'en'],
            github: {
                url: 'github.com', user: 'bem', repo: 'bem-components', defaultBranch: 'v3'
            }
        }
    }
}
~~~

## **![](pictures/engino.png)**

## **![](pictures/horse.gif)**

## Планы на будущее
* Внедрить в bem.info
* ...Внедрить в сайт Лего
* ...Поддержать инкрементальную сборку
* ...Написать тестов, наконец!

## **Ваши вопросы!**

## **Контакты** {#contacts}

<div class="info">
<p class="author">{{ site.author.name }}</p>
<p class="position">{{ site.author.position }}</p>

    <div class="contacts">
        <p class="contacts-left contacts-top">bem.info</p>
        <p class="contacts-left mail">info@bem.info</p>
        <p class="contacts-right twitter">bem_ru #b_</p>
        <!-- <p class="contacts-right contacts-bottom vk">vk</p> -->
        <!-- <p class="contacts-right facebook">facebook</p> -->
    </div>
</div>
