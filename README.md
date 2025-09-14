tsv-web
=======

[![hugo-deploy](https://github.com/langchr86/tsv-web/actions/workflows/hugo-deploy.yml/badge.svg)](https://github.com/langchr86/tsv-web/actions/workflows/hugo-deploy.yml)

Das ist das [Hugo](https://gohugo.io)-Projekt für den Webauftritt des TSV Mettauertal.

Der Webauftritt ist erreichbar unter: [tsvmettauertal.ch](https://tsvmettauertal.ch).


Entwicklung
-----------

Installier Hugo z.B. unter Windows mit [Chocolatey](https://chocolatey.org/):

~~~~~~
choco install -y hugo-extended --version 0.148.2 --pin
~~~~~~

Die genau Version, welche zwingend verwendet werden muss, wird durch die Github Action definiert in:
[hugo-deploy.yml](.github/workflows/hugo-deploy.yml).

Nun kann lokal gearbeitet werden und mittels `hugo server` eine Server-Instanz gestartet werden,
die unter [localhost:1313](http://localhost:1313) erreichbar ist.
Diese aktualisiert sich bei den meisten Änderungen im Projekt automatisch.

Dokumentation:

* https://blowfish.page/docs/homepage-layout/
* https://blowfish.page/docs/shortcodes/
* https://bootstrapshuffle.com/de/classes


Deployment
----------

Das Deployment auf den echten Web-Server passiert automatisch bei einem Push auf den `main`-Branch
durch die Github-Action: [hugo-deploy.yml](.github/workflows/hugo-deploy.yml)


Photo-Galerie
-------------

Die ausgiebige Fotosammlung wird in einem separaten Tool unter:
[gallery.tsvmettauertal.ch](https://gallery.tsvmettauertal.ch) verwaltet.
Dazu wird [Piwigo](https://piwigo.org) selber gehostet.

Um Galerien in der Homepage einzubeten wird eine angepasste Version von
[piwigo-random](https://github.com/moy/piwigo-random) verwendet.

Die angepassten Dateien, welche auf `gallery.tsvmettauertal.ch/piwigo-random/` verfügbar sein müssen, findet ihr hier:
[piwigo-random](/piwigo-random/).
