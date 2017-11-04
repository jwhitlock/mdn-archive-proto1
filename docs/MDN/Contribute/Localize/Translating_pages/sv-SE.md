---
version: prototype1
revision_id: 1324584
locale: sv-SE
slug: MDN/Contribute/Localize/Translating_pages
tags: "Sidöversättning"
title: Översätta MDN-sidor
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: True
needs_localization: True
table_of_contents_depth: 1
based_on: None
---
<p>Denna artikel är en grundläggande guide för översättning av innehåll på MDN, som tar upp både tekniken&nbsp;kring översättningsarbetet och tips på det korrekta sättet att hantera olika typer av innehåll.</p>

<h2 id="Påbörja_översättning_av_en_sida"><span class="short_text" id="result_box" lang="sv"><span class="alt-edited">Påbörja översättning av en sida</span></span></h2>

<p>Följ de här stegen när du stöter på en sida som du skulle vilja översätta till ditt språk:</p>

<ol>
 <li>Klicka på Språk-ikonen ({{FontAwesomeIcon("icon-globe")}}) för att öppna menyn för <strong>Språk</strong> och klicka på <strong>Lägg till en översättning</strong>. Du hamnar då på sidan Välj Språk.</li>
 <li>Klicka på det språk&nbsp;som du vill översätta sidan till. Vyn Översätter artikel öppnas med originalspråkets text på vänster sida av vyn.</li>
 <li>Under <strong>Översätt beskrivning</strong>&nbsp;kan du översätta titeln och även sluggen (frivilligt), till målspråket. Sluggen är den sista delen av en sidas URL (till exempel "Translating_pages" för denna artikel.) Vissa språkgemenskaper översätter inte sluggen, utan låter den vara samma som på engelska.&nbsp;Jämför med andra artiklar på ditt språk för att avgöra vad som är praxis.&nbsp;Du kan klicka på minustecknet bredvid <strong>Översätt beskrivning</strong>&nbsp;för att dölja denna information när du är klar med den, för att göra mer plats för <strong>Översätt innehåll</strong>-sektionen.</li>
 <li>Översätt sidans innehåll under <strong>Översätt innehåll</strong>.</li>
 <li>Fyll i åtminstone en <strong>tagg</strong> för sidan.</li>
 <li>Klicka på <strong>Spara ändringar</strong> när du är färdig.</li>
</ol>

<div class="note"><strong>Note:</strong> The user interface elements of the Translating Article view are initially shown in English. On subsequent visits to translate a particular article, the UI is shown in the appropriate language if a localization of MDN is available for that language. The MDN user interface can be localized using <a href="https://localize.mozilla.org/projects/mdn/" title="https://localize.mozilla.org/projects/mdn/">Verbatim</a>. See <a href="/en-US/docs/Mozilla/Localization/Localizing_with_Verbatim" title="/en-US/docs/Mozilla/Localization/Localizing_with_Verbatim">Localizing with Verbatim</a> for details on how to use this tool.</div>

<h2 id="Redigera_en_sida_som_är_översatt">Redigera en sida&nbsp;som är översatt</h2>

<ul>
 <li>Klicka på <strong>Redigera</strong>-knappen på&nbsp;en redan översatt sida (ibland märkt på&nbsp;mål-språket). Vyn för Översätter artikel öppnas.</li>
</ul>

<p>Om den engelska versionen har ändrats sedan översättningen senast uppdaterades, kommer Översätter artikel-vyn att visa en källnivå-"diff" på&nbsp;ändringarna i den engelska versionen.&nbsp;Detta hjälper dig att se vad som behöver&nbsp;uppdateras i översättningen.</p>

<h2 id="Översätta_taggar">Översätta taggar</h2>

<p>Det är viktigt att varje sida är taggad med minst en tagg. Även om det&nbsp;är översättning. I regel är det en bra idé att använda samma taggar som originalartikeln.</p>

<p>Vissa taggar används för sökfilter, eller som sedvänja mellan bidragare. Dessa bör inte översättas. För att veta vilka dessa är, läs <a href="/en-US/docs/Project:MDN/Contributing/Tagging_standards">tagging standards</a>. Du kan också skapa översatta taggar för att gruppera innehåll, om detta&nbsp;inte täcks av någon av standardens taggar.</p>

<h2 id="Tips_för_nya_lokaliserare">Tips för&nbsp;nya lokaliserare</h2>

<p>Om du är nybörjare inom lokalisering på MDN kommer här några förslag:</p>

<ul>
 <li>Artiklar i <a href="https://developer.mozilla.org/sv-SE/docs/Glossary">Ordlista</a>&nbsp;är jättebra för nybörjare att översätta då de är korta och enkla.</li>
 <li>Artiklar som är taggade med <a href="https://developer.mozilla.org/en-US/docs/tag/l10n%3Apriority">"l10n:priority"</a>&nbsp;anses vara högprioriterade vad gäller översättning. Dessutom har&nbsp;tutorials och konceptuella artiklar generellt sett högre prioritet än referenssidor, då läsare har störst behov av översättningar när de lär sig nya koncept.</li>
 <li>Om du ser text mellan dubbla klammerparenteser, som t.ex. &nbsp;<code>\{{some-text("more text")}}</code>, lämna det oöversatt i artikeln, och ändra inte skiljetecknen. Detta är ett <a href="https://developer.mozilla.org/en-US/docs/MDN/Contribute/Structures/Macros">macro</a>, som antagligen skapar en struktur på sidan, eller gör något annat användbart.&nbsp;Du kan komma att se oöversatt text som genereras från ett macro; bry dig inte om det förrän du har mer erfarenhet av MDN. (Att ändra denna typ av text kräver&nbsp;<a href="https://developer.mozilla.org/en-US/docs/MDN/Contribute/Tools/Template_editing">särskilda behörigheter</a>&nbsp;eftersom macros kan vara väldigt kraftfulla.) Om du är nyfiken, titta på <a href="https://developer.mozilla.org/en-US/docs/MDN/Contribute/Structures/Macros/Commonly-used_macros">Commonly-used macros</a>&nbsp;för att se vilka typer av saker macros kan göra.</li>
 <li>Titta på sidan&nbsp;<a href="https://developer.mozilla.org/en-US/docs/MDN/Contribute/Localize/Localization_projects">Localization projects</a>&nbsp;för att veta mer om lokalisering för din "locale".</li>
</ul>

