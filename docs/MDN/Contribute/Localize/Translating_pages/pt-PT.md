---
version: prototype1
revision_id: 1319549
locale: pt-PT
slug: MDN/Contribute/Localize/Translating_pages
tags: "Tradução" "Localização" "Tradução de Página"
title: Traduzir páginas da MDN
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: True
table_of_contents_depth: 1
based_on: None
---
<p>Este artigo é um guia básico para traduzir o conteúdo na MDN, incluindo a mecânica do trabalho de tradução e as dicas de maneira adequada para lidar com os vários tipos de conteúdo.</p>

<h2 id="Começar_uma_nova_página_de_tradução">Começar uma nova página de tradução</h2>

<p>Quando encontra uma página que gostaria de traduzir o seu idioma, siga estes passos:</p>

<ol>
 <li>Clique no ícone dos Idiomas ({{FontAwesomeIcon("icon-language")}}) para abrir o menu dos <strong>Idiomas</strong>, e clique em <strong>Adicionar uma Tradução</strong>. A página dos Idiomas Selecionados aparece.</li>
 <li>Clique no idioma que deseja utilizar na tradução da página. A visualização de Traduzir Artigo abre com o texto do idioma original exibido no lado esquerdo da visualização.</li>
 <li>Sob a <strong>Descrição de Tradução</strong>, pode traduzir o título e opcionalmente a peneira rotativa para a linguagem selecionada. A "slug" é a última parte do URL de uma página (por exemplo, "Páginas de tradução" para este artigo.) Algumas comunidades de linguagens não traduzem a "slug", mantendo a mesma em Inglês. Compare com outros artigos na sua lingua, para determinar a prática comum. Pode clicar o sinal menos (-) ao lado da <strong>Descrição de Tradução</strong> para esconder esta informação quando terminar, para criar mais espaço para a seção <strong>Conteúdo de Tradução.</strong></li>
 <li>Sob <strong>Conteúdo de Tradução</strong>, traduza o corpo da página.</li>
 <li>Preencha pelo menos uma <strong>etiqueta</strong> para a página.</li>
 <li>Clique <strong>Guardar Alterações</strong> quando terminar.</li>
</ol>

<div class="note"><strong>Nota:</strong> Os elementos da interface do utilizador da visualização do Artigo de Tradução são mostrados inicialmente em Inglês. Em visitas subsequentes para traduzir um artigo em particular, a interface do utilizador (IU) é exibida na linguagem apropriada se a localização da RDM está disponível para tal idioma. A interface do utilizador da RDM pode ser localizada ao usar <a href="https://localize.mozilla.org/projects/mdn/" title="https://localize.mozilla.org/projects/mdn/">Pontoon.</a><br />
Veja <a href="/pt-PT/docs/Mozilla/Localization/Localização_com_Pontoon" title="/en-US/docs/Mozilla/Localization/Localizing_with_Verbatim">Localizar com Pontoon</a> para detalhes em como usar esta ferramenta.</div>

<h2 id="Editar_uma_página_traduzida">Editar uma página traduzida</h2>

<ul>
 <li>Em uma página traduzida, clique no botão <strong>Editar</strong> (por vezes rotulado no idioma-alvo). A visualização do Artigo de Tradução abre.</li>
</ul>

<p>Se a versão Inglesa foi alterada desde a última atualização de tradução, a visualização do Artigo de Tradução mostra um "diff" de nível de origem das alterações na versão Inglesa. Isto ajuda a ver o que precisa de ser atualizado na tradução.</p>

<h2 id="Etiquetar_tradução">Etiquetar tradução</h2>

<p>É importante que cada página seja etiquetada pelo menos com uma etiqueta ou "tag".<br />
 Mesmo que isto seja tradução.</p>

<p>Algumas etiquetas são utilizadas para filtros de procura, ou como convenções entre colaboradores. Estas não devem ser traduzidas. Para conhecer estas etiquetas, leia as <a href="/pt-PT/docs/MDN/Contribute/Localize/Projetos_localização">Normas de Etiquetagem</a>. É livre de criar etiquetas traduzidas para o conteúdo de grupo, se isto não estiver coberto por uma das normas de etiquetas.</p>

<h2 id="Dicas_para_os_novos_tradutores">Dicas para os novos tradutores</h2>

<p>Se não possui&nbsp;experiência&nbsp;em&nbsp;localização na&nbsp;MDN, aqui estão algumas sugestões:</p>

<ul>
 <li>Os artigos no <a href="/pt-PT/docs/Glossário">Glossário</a> são excelentes serem traduzidos por principiantes, porque estes são curtos e simples.</li>
 <li>Os&nbsp;artigos que estão etiquetados <a href="/en-US/docs/tag/l10n%3Apriority">"l10n:priority"</a>&nbsp;são considerados de alta prioridade para tradução.</li>
 <li>Se ver um texto entre chaves duplas, como por exemplo <code>\{{some-text("more text")}}</code>,&nbsp; deixe-o não traduzido, e não modifique&nbsp;os caracteres de&nbsp;pontuação. Isto é um&nbsp;<a href="/en-US/docs/MDN/Contribute/Structures/Macros">macro</a>, que provavelmente cria uma estructura na página, ou tem qualquer outra função útil. É provável que veja textos não traduzidos producidos por um macro; não se preocupe com isso até que adquira mais experiência&nbsp;com a&nbsp;MDN. (Mudar este texto requere <a href="/en-US/docs/MDN/Contribute/Tools/Template_editing">privilégios</a>&nbsp;<a href="/en-US/docs/MDN/Contribute/Tools/Template_editing">especiais</a>&nbsp;porque os macros podem ser muito poderosos.)&nbsp;Se estiver curioso, dê uma olhada aos&nbsp;<a href="/en-US/docs/MDN/Contribute/Structures/Macros/Commonly-used_macros">macros&nbsp;mais utilizados</a>&nbsp;e verifique os que os macros são capazes de fazer.</li>
 <li>Consulte a página de <a href="/pt-PT/docs/MDN/Contribute/Localize/Projetos_localização">Projetos de Localização</a> para saber mais sobre a localização para o seu idioma.</li>
</ul>

<p>&nbsp;</p>

