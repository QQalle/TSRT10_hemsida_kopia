---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---
# Projekthemsida

I år hostas och utvecklas projekthemsidorna med hjälp av GitLab Pages
hostat av [gitlab.liu.se](https://gitlab.liu.se).  Mer om GitLab Pages
och hur ni gör er hemsida kan ni läsa här:
[GitLab Pages](https://docs.gitlab.com/ee/user/project/pages/).

GitLab Pages är begränsade till statiska hemsidor, men det är enkelt
att integrera olika SSG ramverk.

Under kursens gång kommer er hemsida vara tillgänglig från:

	https://tsrt10.gitlab-pages.liu.se/<YYYY>/<projektnamn>

där *&lt;YYYY&gt;* är året kursen går och *&lt;projektnamn&gt;* är det kortnamn
ert gitlab-projekt har.  Endast de som har access till ert projekt i
gitlab har access till sidan. I samband med leverans av projektet
kommer hemsidan att göra publikt tillgänglig.

Vi kommer, precis som föreslås på
[Exploring GitLab Pages](https://docs.gitlab.com/ee/user/project/pages/introduction.html),
kräva att ni separerar er hemsida i en branch helt separat från övrig
utveckling.  Vi kommer att exportera hemsidan till en extern webserver
automatiskt, det är alltså viktigt att ni använder rätt
branch. Branchen ska heta **pages**, och kan skapas på följande sätt:

	git checkout --orphan pages && git reset --hard

När det är gjort är det bara att jobba på branchen som vanligt.
Notera att för att hemsidan ska dyka upp behöver ni skapa filen
*.gitlab-ci.yml* med rätt innhåll, se
[GitLab Pages](https://docs.gitlab.com/ee/user/project/pages/) för detaljer.


Den här hemsidan är skapad med GitLab Pages och
[Jekyll](https://jekyllrb.com/),
och använder pages branchen på samma sätt som er hemsida ska.  Ta
gärna en titt i det här projektet för att en idé om hur man kan
göra:
[tsrt10-pages-ex](https://gitlab.liu.se/hendeby-public/tsrt10-pages-ex)
