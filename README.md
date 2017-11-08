Scrap [Dofus][] [Treasure Hunter][].

[![][Illustration]][La chasse aux trésors]

Builds
------

- [Branch: build][]

Dependencies
------------

- [Puppeteer][]

Running
-------

Running [scrap](bin/scrap) launches [Puppeteer][] (the [head-less Chrome browser][Announcement])
and collects data from [Treasure Hunter][] to [dofus-treasure-hunter/](dofus-treasure-hunter).

Structure
---------

```
dofus-treasure-hunter
└── clues
   ├── names
   │  └── <language>.json
   └── positions
      └── <name>.json
```

The structure is a directory with the name of the visual clues – which are [JSON][] formatted.

Translations come from [Treasure Hunt][].

Usage
-----

```
scrap
```

Deploying
---------

```
deploy
```

Running [deploy](bin/deploy) deploys the collected data to the [build][Branch: build] branch.

[Announcement]: https://developers.google.com/web/updates/2017/04/headless-chrome
[Branch: build]: https://github.com/alexherbo2/dofus-treasure-hunter-scrap/tree/build
[Dofus]: http://dofus.com
[Illustration]: https://s.ankama.com/www/static.ankama.com/upload/backoffice/direct/2014-03-25/a5eb7605c4ed1c18376915ddb5506f09.jpg
[JSON]: https://json.org
[La chasse aux trésors]: http://dofus.com/fr/mmorpg/actualites/devblog/billets/417489-chasse-tresors
[Puppeteer]: https://github.com/GoogleChrome/puppeteer
[Treasure Hunter]: https://dofusama.fr/treasurehunt/rechercher-un-indice.html
[Treasure Hunt]: http://dofus-map.com/hunt
