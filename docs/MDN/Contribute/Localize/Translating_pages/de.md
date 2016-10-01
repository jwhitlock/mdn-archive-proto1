---
version: prototype1
revision_id: 1126151
locale: de
slug: MDN/Contribute/Localize/Translating_pages
tags: "MDN" "Guide" "Anfänger" "Beginner" "Übersetzung" "übersetzen" "Lokalisation" "Seite Übersetzen"
title: MDN Seiten übersetzen
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: True
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<p>Dieser Artikel ist eine Grundanleitung für die Übersetzung von Inhalten auf MDN. Er beinhaltet sowohl die Grundlagen Übersetzungsarbeit als auch Tipps für den richtigen Umgang mit den verschiedenen Arten von Inhalten.</p>

<h2 id="Übersetzung_einer_neuen_Seite_starten">Eine neue Übersetzung einer Seite starten</h2>

<p>Befolgen Sie diese Schritte, wenn Sie eine Seite in Ihre Sprache übersetzen möchten:</p>

<ol>
 <li>Klicken Sie auf das Sprachen-Symbol ({{FontAwesomeIcon("icon-language")}}) um das <strong>Sprachen</strong>-Menü zu öffnen und wählen Sie <strong>Übersetzung hinzufügen</strong>. Daraufhin erscheint die Auswahlseite der verfügbaren Sprachen.</li>
 <li>Wählen Sie die Sprache, in die Sie die Seite übersetzen möchten. Anschließend öffnet sich ein Editor, auf dessen linker Hälfte die originale Seite, auf der rechten die Vorschau der übersetzten Seite zu sehen ist.</li>
 <li>Unter <strong>Beschreibung übersetzen</strong> können Sie den Titel und optional den Adressnamen (Slug) in die Zielsprache übersetzen. Der Adressname ist der letzte Teil der URL einer Seite (zum Beispiel: "Translating_pages" für diesen Artikel.) Manche Sprachcommunities übersetzen den Adressnamen nicht und übernehmen den Englischen. Vergleichen Sie dazu am besten andere Artikel in Ihrer Sprache um die gängige Praxis zu ermitteln. Um mehr Platz für den Abschnitt <strong>Übersetzung in Deutsch</strong> zu erhalten, können Sie auf das Minus-Zeichen neben dem Abschnitt <strong>Beschreibung übersetzen</strong> klicken und ihn so ausblenden.</li>
 <li>Übersetzen Sie den Inhalt der Seite unter <strong>Übersetzung in Deutsch</strong>.</li>
 <li>Tragen Sie mindestens ein <strong>Schlagwort</strong> für die Seite ein.</li>
 <li>Drücken Sie<strong> Änderungen speichern</strong> wenn Sie fertig sind.</li>
</ol>

<div class="note"><strong>Hinweis:</strong> Die Benutzeroberfläche der "Artikel übersetzen"-Ansicht werden anfangs in Englisch angezeigt. Bei nachfolgenden Bearbeitungen eines bestimmten Artikels im Editor wird die Benutzeroberfläche in der jeweils passenden Sprache angezeigt, falls eine Lokalisierung für MDN in dieser Sprache verfügbar ist. Die MDN Benutzeroberfläche kann mit <a href="https://localize.mozilla.org/projects/mdn/" title="https://localize.mozilla.org/projects/mdn/">Pontoon</a> lokalisiert werden. Konsultieren Sie dazu <a href="/en-US/docs/Mozilla/Localization/Localizing_with_Verbatim" title="/en-US/docs/Mozilla/Localization/Localizing_with_Verbatim">Lokalisierung mit Pontoon</a> für Details zu dessen Benutzung.</div>

<h2 id="Eine_übersetzte_Seite_bearbeiten">Eine übersetzte Seite bearbeiten</h2>

<ul>
 <li>Drücken Sie auf einer übersetzten Seite den <strong>Bearbeiten</strong> Knopf (mitunter auch englisch: <strong>Edit</strong>). Die <strong>Artikel-Übersetzen</strong>-Ansicht öffnet sich.</li>
</ul>

<p>Wenn die englische Version seit der letzten Aktualisierung der Übersetzung verändert wurde, wird in der Artikel-Übersetzen-Ansicht die Quellebene "diff" mit den Änderungen der englischen Version angezeigt. Dies hilft Ihnen, Aktualisierungen schneller durchzuführen.</p>

<h2 id="Übersetzungs_Tags">Schlagwort-Übersetzungen</h2>

<p>Es ist wichtig, dass jede Seite mit mindestens einem Schlagwort getaggt wird, auch wenn es sich um eine Übersetzung handelt.</p>

<p>Manche Tags werden von Suchfiltern oder als Konventionen zwischen Beitragserstellern benutzt. Diese Schlagwörter sollten nicht übersetzt werden. Lesen Sie hierzu die <a href="/en-US/docs/Project:MDN/Contributing/Tagging_standards">Tagging Standards</a> um diese Schlagwörter zu erkennen.<br />
 Sie dürfen gern übersetzte Schlagwörter erstellen, um Inhalte zu gruppieren, wenn sie nicht von einem Standard-Schlagwort abgedeckt werden.</p>

<h2 id="Tipps_für_neue_Übersetzer">Tipps für neue Übersetzer</h2>

<p>Sie sind neu bei der Lokalisierung auf MDN? Dann sind hier ein paar Ratschläge:</p>

<ul>
 <li>Artikel im <a href="/de/docs/Glossary">Glossar</a> eignen sich hervorragend für Einsteiger, weil sie einfach und kurz sind.</li>
 <li>Artikel mit dem Schlagwort <a href="/en-US/docs/tag/l10n:priority">"l10n:priority"</a> werden beim Übersetzen mit einer hohen Priorität berücksichtigt.</li>
 <li>Wenn Text in doppelten geschweiften Klammern steht, wie <code>\{{some-text("more text")}}</code>, dann lassen Sie diesen unübersetzt, und ändern Sie die Satzzeichen nicht. Dies sind <a href="/en-US/docs/MDN/Contribute/Structures/Macros">Makros</a>, die Strukturen auf der Seite erstellen, oder andere nützliche Funktionen übernehmen. Es kann sein, dass das Makro unübersetzten Text erzeugt, machen Sie sich darüber keine Gedanken, bis Sie mehr Erfahrung mit MDN gewonnen haben (das Bearbeiten dieses Textes erfordert <a href="/en-US/docs/MDN/Contribute/Tools/Template_editing">spezielle Privilegien</a>, weil Makros sehr mächtige Werkzeuge sein können.) Wenn Sie neugierig sind, werfen Sie doch einen Blick auf die <a href="/en-US/docs/MDN/Contribute/Structures/Macros/Commonly-used_macros">Häufig verwendeten Makros</a>, um die Möglichkeiten der Makros zu verstehen.</li>
 <li>Schauen Sie auf die <a href="/en-US/docs/MDN/Contribute/Localize/Localization_projects">Lokalisations-Projektseite</a> um mehr über die Lokalisierung in ihre Sprache zu erfahren.</li>
</ul>

