# LaTex Vorlage für Abschlussarbeiten am rtm

Diese Vorlage enhält ein paar nützliche Pakete und typische Elemente und Umgebungen um den Einstieg ins schreiben wissenschatlicher Arbeiten in LaTex zu erleichtern. Sie nutzt das offizielle LaTex-Paket der Technischen Universität Darmstadt *tuda-ci*, das in allen aktuellen LaTex-Distributionen verfügbar ist.

Dieses Dokument baut auf tuda-ci_vorlage auf.

Verwandte Projekte
- [tuda-ci_vorlage](https://git.rtm.e-technik.tu-darmstadt.de/tuda-ci_templates/tuda-ci_vorlage): die Minimalbasis für Dokumente am rtm. Enthält im Wesentlichen die Konfiguration des TU-Designs (rtm Farbe und Logo)
- [tuda-ci_thesisinfo](https://git.rtm.e-technik.tu-darmstadt.de/tuda-ci_templates/tuda-ci_thesisinfo): ein Dokument mit vielen Tipps und Informationen zum schreiben einer Abschlussarbeit


# Infos für Maintainer

Änderungen, die alle Projekte gleichermaßen betreffen (z.B. Titelseite, Layout, Literaturverzeichnis) sollten zuerst in ``tuda-ci_vorlage`` eingepflegt werden und anschließend nicht manuell, sondern durch einen Merge in die ``tuda-ci_thesisinfo`` und ``tuda-ci_useful-packages`` übernommen werden.

Für den Merge erstellt man z.B. eine Mergerequest im ``_vorlage``-Projekt mit Quelle ``_vorlage:master`` und Ziel ``_useful-packages:master``.  Der Request taucht dann automatisch im Zielprojekt auf und kann dort gemerged werden.

Alternativ für lokalen merge das _vorlage- Repo als remote einbinden
```
git remote add upstream 'https://git.rtm.e-technik.tu-darmstadt.de/tuda-ci_templates/tuda-ci_vorlage.git'
git fetch upstream
git branch -a  (prüfen, ob upstream branches geladen wurden)
git merge upstream/fix/ultimativeLoesung
git push
(git remote remove upstream)
```