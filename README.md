# Hinweise für Forschungsberichte und quantitative empirische Abschlussarbeiten

![](UNI_Kassel_FB_Gesellschaftswissenschaften_Farbe_klein.png)

Dieses Template beinhaltet die [Hinweise für das Verfassen von Forschungsberichten und quantitativen empirische Abschlussarbeiten](https://www.uni-kassel.de/fb05/index.php?eID=dumpFile&t=f&f=476&token=1ae8c6038ddadd3c07822dded7cc19b0223a195a) von
[Frau Dr. Manuela Pötschke FB 05 Universität Kassel](https://www.uni-kassel.de/fb05/fachgruppen-und-institute/soziologie/fachgebiete/angewandte-statistik/team/dr-manuela-poetschke).

Diese Vorlage soll als Stütze dienen, um mit R und R-Studio einen Forschungsbericht zu erstellen.

Grundkenntnisse in R, sowie das Arbeiten mit Markdown-Dateien werden vorausgesetzt. Als Einstiegsliteratur wird [R Markdown Cookbook: Yihui Xie, Christophe Dervieux, Emily Riederer (2021)](https://bookdown.org/yihui/rmarkdown-cookbook/) empfohlen

[Markdown Cheat Sheet](https://www.markdownguide.org/cheat-sheet/)

# Installationsanleitung

Follgende Programme werden benötigt um das Skript zum laufen zu bringen.

[LaTeX](https://www.latex-project.org/get/)

[R](https://cran.r-project.org/mirrors.html)

[R-Studio](https://www.rstudio.com/products/rstudio/download/#download) oder eine beliebig andere IDE

## Installation via [homebrew](https://formulae.brew.sh/)

```{bash}
# latex
brew install --cask basictex
brew install texlive

# r + rstudio
brew install r
brew install --cask rstudio
```

## Installation via [pacman](https://wiki.archlinux.org/title/pacman)

```{bash}
sudo pacman -S texinfo texlive-core texlive-latexextra texlive-science r
```

Sowie das Paket [markdown](https://cran.r-project.org/web/packages/markdown/index.html)

```{r}
install.packages("rmarkdown")
```

---

## Allgemeine Hinweise

Allgemeine Hinweise zu Forschungsberichten aus Empiriepraktika (BA, Modul 6), empirischen Seminaren (MA, Modul 3) oder für empirische Abschlussarbeiten (BA, MA):
Der Umfang des Berichts im Empiriepraktikum ergibt sich aus der Fragestellung und den verwendeten Analyseverfahren. Wenn die Seitenzahl vorgegeben oder vereinbart ist und nicht ausreicht, ist die Forschungsfrage nicht präzise genug formuliert.

Es gibt keine allgemein gültigen Regeln für das Abfassen von Forschungsberichten, außer:

- Die Arbeit beginnt mit einem Deckblatt, das mindestens den (prägnanten) Titel der Arbeit, den Namen des Schreibenden, die Matrikelnummer, eine E-Mail-Adresse und den Bezug (also den Titel der Lehrveranstaltung und ihre Leitung) enthalten soll.

- Die Arbeit muss ein Inhaltsverzeichnis und ein Literaturverzeichnis enthalten.

- Beachten Sie die formalen Regeln für die Zitation! Zitationen sollen den Lesenden das Ver- ständnis erleichtern und die Lesenden sollen die Quellen Ihrer Argumentation leicht nachvoll-
ziehen können, ohne dass der Lesefluss unterbrochen wird.

- Erstellen Sie ein vollständiges und übersichtliches Literaturverzeichnis!

- Die Arbeit kann ein Abbildungs- und ein Tabellenverzeichnis sowie einen Anhang enthalten. Die Seitennummerierung der Arbeit bezieht den Anhang nicht mit ein.

- Gliedern Sie Ihre Arbeit nach nachvollziehbaren Kriterien mit verschiedenen Abstraktionsni- veaus! Machen Sie es den Lesenden leicht, Ihren Argumenten zu folgen und bereiten Sie den
Lesenden durch einen präzisen und interessanten Schreibstil ein Lesevergnügen.

- Der Argumentationsgang muss immer auf die Forschungsfrage bezogen sein. Er folgt einem klaren und durchgängigen „roten Faden“. Exkurse sind deutlich zu machen (z.B. mit spezifi- schem Titel, spezifischer Formatierung oder indem die entsprechenden Passagen in Fußnoten geschrieben werden).

<br/>
<br/>

# Bewertungsschema für empirische Haus- und Abschlussarbeiten

<table class="tg">
<thead>
  <tr>
    <th class="tg-0pky">Gewichtung Beurteilungsgegenstand</th>
    <th class="tg-0pky">Bemerkungen</th>
    <th class="tg-0pky">Gewichtung</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">Formale Anforderungen</td>
    <td class="tg-0pky">korrektes Inhaltsverzeichnis (mit Gliederungsnummerierung);
korrekte Zitation im Text und vollständiges Literaturverzeichnis;
Deckblatt</td>
    <td class="tg-0pky">bei geringen Verstößen: 0,3 Noten Abzug;
bei groben Verstößen: 1 Note Abzug</td>
  </tr>
  <tr>
    <td class="tg-0pky">sprachliche Qualität</td>
    <td class="tg-0pky">grammatikalisch korrekte Sprache, keine Rechtschreibfehler;
Vermeidung von Bandwurmsätzen; klare, präzise Formulierungen; Verwendung angemessener Fachbegriffe</td>
    <td class="tg-0pky">bei geringen Verstößen: 0,3 Noten Abzug;
bei groben Verstößen: 1 Note Abzug</td>
  </tr>
  <tr>
    <td class="tg-0pky">klare Fragestellung</td>
    <td class="tg-0pky">In der Einleitung muss deutlich werden, wo- rum es in der Arbeit genau geht.</td>
    <td class="tg-0pky">bei unklarer Fragestellung muss die Arbeit überarbeitet werden</td>
  </tr>
    <tr>
    <td class="tg-0pky">klare und angemessene Struktur</td>
    <td class="tg-0pky">die Gliederung folgt der Logik zur Beantwortung der Frage;
eine Zusammenfassung der Ergebnisse oder ein Fazit schließen die Arbeit ab;
logisch und sachlich korrekte und empirisch begründete Argumentation in Bezug auf die Fragestellung/ Hypothese</td>
    <td class="tg-0pky">bei unklarer Struktur oder Argumentation Abzug bis zu einer Note;
bei fehlender Beantwortung der Frage muss die Arbeit überarbeitet werden</td>
  </tr>
    <tr>
    <td class="tg-0pky">Einleitung</td>
    <td class="tg-0pky">umfasst die Fragestellung mit Herleitung, Be- gründung ihrer Relevanz und die kurze Darstellung des Aufbaus der Arbeit</td>
    <td class="tg-0pky">bei fehlender Fragestellung muss die Arbeit überarbeitet werden</td>
  </tr>
    <tr>
    <td class="tg-0pky">Darstellung des theoretischen Hintergrundes</td>
    <td class="tg-0pky">Auswahl relevanter Literatur;
adäquate Darstellung der jeweiligen Argumente;
Vollständigkeit über das Feld (nicht über die Autoren)</td>
    <td class="tg-0pky">Bonus für die präzise Darstellung von Diskussionen mit Für und Wider-Argumenten bis zu einer Note
Abzug bis zu einer Note, wenn relevante Teile des Forschungsfeldes fehlen</td>
  </tr>
    <tr>
    <td class="tg-0pky">Hypothesen</td>
    <td class="tg-0pky">müssen aus der Theorie abgeleitet und empi- risch prüfbar sein</td>
    <td class="tg-0pky">Abzug bis zu einer Note</td>
  </tr>
    <tr>
    <td class="tg-0pky">Anwendung und Darstellung der verwendeten Methoden</td>
    <td class="tg-0pky">Begründung für die verwendete Methode;
je nach Schwerpunkt der Arbeit und Gebräuchlichkeit der Methode ausführliche Darstellung</td>
    <td class="tg-0pky">Abzug bis zu einer Note</td>
  </tr>
    <tr>
    <td class="tg-0pky">Darstellung empirischer Ergebnisse</td>
    <td class="tg-0pky">korrekte und anschauliche Beschreibung der Ergebnisse;
Unterstützung der Darstellung durch angemessene Grafiken, Tabellen und Abbildungen</td>
    <td class="tg-0pky">Abzug bis zu zwei Noten</td>
  </tr>
</tbody>
</table>


