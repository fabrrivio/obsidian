<h1>Version de NodeJs</h1>
La version en générale a utiliser est la: **node_14** et pas la node_16

<h1>Communiquer nuxt avec l'aio locale</h1>
- changer la config [[Docker]] dans docker-compose.yaml
  extra_hosts:
      - "back.aio-prm.aio:${DOCKER_HOST_IP}"
* changer le .env du projet
  AIO_API_BASE_URL=https://back.aio-prm.aio
  SITE_HOSTNAME=https://back.aio-prm.aio
* redemarrer docker

<h1>Problème affichage d'image sur le front</h1>
* Si les images ne s'affichent pas sur les sites déployés via le manager, il faut contrôler:
1. Désactiver la config proxy côté front: (mettre à false)
      ![[Pasted image 20221228092854.png]]
2. Se connecter en SSH et faire un symlink du dossier media (ln -s /home/clients/{clientid}/{aio_directory}/shared/public/media media) à voir doc https://github.com/iomediacommunication/documentation/blob/main/infrastructure/index.md
3. Modifier la configuration sur le [[Manager]]: mettre media dans dossier partagé

<h1>Recaptcha</h1>
https://developers.google.com/recaptcha/docs/faq#id-like-to-run-automated-tests-with-recaptcha.-what-should-i-do
https://iomedia.slack.com/archives/C04GB1STYR3/p1673963132928619

