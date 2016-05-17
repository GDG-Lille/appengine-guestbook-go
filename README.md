Ma première application sur la Google Cloud Platform avec Appengine & Go
===

Cette application est un exemple simplifié du [tutoriel officiel][0]

## Product & Language
- [App Engine][1]
- [Go][2]

## Démarrage
Faisons tout d'abord fonctionner cette application en local.

1. **Téléchargement du [SDK][3]**
2. **Lancement de l'application**
    * `/path/to/go_appengine/goapp serve helloworld/`
    * `curl http://localhost:8080`
    * :)

## Déploiement
Nous avons une application qui fonctionne, déployons là sur Google Appengine!

1. **Connexion à [la console][4] et création d'une application**
    * Nous nommerons par la suite l'identifiant de votre nouvelle application <ID_APPLICATION>
2. **Déploiement!**
    * `/path/to/go_appengine/appcfg.py -A <ID_APPLICATION> -V 1 update helloworld/`
    * `curl http://<ID_APPLICATION>.appspot.com`
    * :)

## Compléments
Google Appengine est une plateforme avec beaucoup de services disponibles. N'hésitez pas à regarder la
[documentation complète][5]. Les langages acceptés nativement sont Java, Python, Go, PHP,
mais il est aussi simple d'y faire tourner du Node ou du Ruby!

Appengine, en tant que "Platform as a Service", n'est qu'une petite partie des services fournis par la Google Cloud Platform.
Vous en trouverez un plus grand aperçu [ici][6].




[0]: https://cloud.google.com/appengine/docs/go/quickstart
[1]: https://developers.google.com/appengine
[2]: https://golang.org
[3]: https://cloud.google.com/appengine/downloads/#Google_App_Engine_SDK_for_Go
[4]: https://console.developers.google.com
[5]: https://cloud.google.com/appengine/docs
[6]: https://cloud.google.com/