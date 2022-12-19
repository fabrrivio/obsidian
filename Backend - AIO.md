<h1>Mettre à jour la version d'aio CMS</h1> Example avec version 1.7.*
https://documentation.iomedia.ch/doc/developpement/cms/aio2020/versions/index.md

1. Fixer la version (composer update aio-cms-bundle -W)
  "iomedia/aio-cms-bundle": "^1.7.*",
2. Lancer le CMS en local avec une db local et lancer les migrations
   php bin/console doctrine:schema:update --dump-sql


<h1>Mise en place </h1>

