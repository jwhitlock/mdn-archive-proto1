---
version: prototype1
revision_id: 1275319
locale: pt-BR
slug: Mozilla/Add-ons
tags: "Add-ons" "TopicStub" "Precisa de Tradução"
title: Complementos
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div class="summary">Modifique e amplie os aplicativos da Mozilla</div>

<p><strong>Complementos</strong> acrescentam novas funcionalidades para os aplicativos baseados no <a href="/pt-BR/docs/Mozilla/Gecko" title="Informações do Gecko">Gecko</a> tais como Firefox, SeaMonkey e Thunderbird. Há dois tipos de complementos principais <a href="/pt-BR/docs/Mozilla/Add-ons/Gerenciador_de_Add-on#Extensoes">Extensões</a> adicionam novas características para o aplicativo, enquanto <a href="/pt-BR/docs/Mozilla/Add-ons/Temas">Temas</a> modificam a interface do aplicativo do usuário.</p>

<p>Para ambos, extensões e temas, a Mozilla opera o repositório em <a href="https://addons.mozilla.org" title="Ir para a página de Complementos">addons.mozilla.org</a>, também conhecido como AMO. Quando você <a href="/pt-BR/docs/Mozilla/Add-ons/Enviando-um-complemento-para-o-AMO" title="Enviando seu complemento">Envia complementos para o AMO</a> eles são revisados e depois de passados na revisão, são disponibilizados aos usuários. Você não tem que enviar complementos para AMO, mas se enviar, os usuários terão mais confiança no fato de que eles foram revisados, e você pode se beneficiar da visibilidade AMO como uma fonte confiável para complementos úteis.</p>

<p>O termo "complemento"(Add-ons) inclui plugins, extensões, temas, e plug-ins de mecanismos de busca (tal como google, bing, etc.).</p>

<p>O <a href="/pt-BR/docs/Mozilla/Add-ons/Gerenciador_de_Add-on" title="Addons/Add-on Manager">Gerenciador de complementos</a> pode afetar o comportamento do aplicativo que o hospeda. Nós desenvolvemos <a href="/pt-BR/docs/Mozilla/Add-ons/Orientacoes-de-complementos" title="/Add-ons/Orientacoes-de-complementos">orientações de complementos</a> para ajudar a garantir que eles proveriam uma boa experiência para os usuários. Estas orientações se aplicam em todos tipos de complementos, mesmo se eles são hospedados em <a href="https://addons.mozilla.org" title="Ir para a página de Complementos">addons.mozilla.org</a> ou não.</p>

<p>O <a href="/pt-BR/docs/Mozilla/Add-ons/Gerenciador_de_Add-on" title="Addons/Add-on Manager">Gerenciador de complementos</a> dá acesso aos complementos a fim de determinar o que está disponível, instalar, remover, desativar e atualizar.</p>

<hr />
<h2 id="Extensões_2"><a name="Extensões">Extensões</a></h2>

<p>Extensões adicionam novas funcionalidades para aplicativos da Mozilla como Firefox e Thunderbird. Eles podem adicionar novos recursos ao navegador, como um jeito diferente de gerenciar as abas, e eles podem modificar o conteúdo da web para aperfeiçoar a usabilidade ou segurança sites específicos.</p>

<p>Há três tipos de técnicas diferentes que você pode utilizar para construir uma extensão: Add-on baseado em extensões SDK, extensões <em>restartless</em> inicializadas manualmente e extensões overlay.</p>

<ul class="card-grid">
 <li>Desenvolva extensões que não requer a reinicialização do navegador utilizando um conjunto JavaScript APIs de alto nível.</li>
 <li><a href="https://developer.mozilla.org/en-US/Add-ons/Bootstrapped_extensions">Extensões <em>Restartless</em></a><br />
  Desenvolva extensões que não requer a reinicialização do navegador.</li>
 <li><a href="https://developer.mozilla.org/en-US/Add-ons/Overlay_Extensions"><span>Extensões Overlay</span></a><br />
  Extensões que requerem a reinicialização do navegador para instalar, geralmente usando <a href="https://developer.mozilla.org/pt-BR/docs/Mozilla/Tech/XUL/Overlays">overlays XUL</a>.</li>
</ul>

<p>Se você puder, é aconselhável utilizar o Add-on SDK, que usa o mecanismo de extensão restartless mas simplifica determinadas tarefas e limpa depois de si mesmo. Se o Add-on SDK não é suficiente para as suas necessidades, implemente uma extensão restartless manual no lugar.</p>

<p>Para obter mais informações sobre como escolher qual a técnica de usar, leia esta <a href="https://developer.mozilla.org/en-US/Add-ons/Comparing_Extension_Toolchains">comparação</a>.</p>

<div class="column-container">
<div class="column-half">
<h3 id="Práticas_Recomendadas">Práticas Recomendadas</h3>

<p>Não importa como você desenvolve uma extensão, existem algumas orientações que você pode seguir para ajudar a garantir que sua extensão fornece uma experiência tão boa para o usuário o quão possível.</p>

<dl>
 <dt><a href="https://developer.mozilla.org/en-US/Add-ons/Performance_best_practices_in_extensions">Desempenho</a></dt>
 <dd>Assegurando que sua extensão é rápida, responsiva e eficiente para a memória.</dd>
 <dt><a href="https://developer.mozilla.org/en-US/Add-ons/Security_best_practices_in_extensions">Segurança</a></dt>
 <dd>Assegurando que sua extensão não exponha o usuário para websites maliciosos.</dd>
 <dt><a href="https://developer.mozilla.org/en-US/Add-ons/Extension_etiquette">Etiqueta</a></dt>
 <dd>Assegurando que sua extensão funcione bem com outras extensões.</dd>
</dl>
</div>

<div class="column-half">
<h3 id="Aplicativo_específico">Aplicativo específico</h3>

<p>A maioria das documentações assume que você está desenvolvendo para o Firefox Desktop. Se você está desenvolvendo para algum outro aplicativo baseado no Gecko, há diferenças importantes que você precisa saber sobre.</p>

<dl>
 <dt><a href="https://developer.mozilla.org/en-US/Add-ons/Thunderbird">Thunderbird</a></dt>
 <dd>Desenvolvendo extensões para o Thunderbird mail client.</dd>
 <dt><a href="https://developer.mozilla.org/en-US/Add-ons/Firefox_for_Android">Firefox para Android</a></dt>
 <dd>Desenvolvendo extensões para Firefox para Android.</dd>
 <dt><a href="https://developer.mozilla.org/en-US/Add-ons/SeaMonkey_2">SeaMonkey</a></dt>
 <dd>Desenvolvendo extensões para <a href="http://www.seamonkey-project.org/">SeaMonkey</a> <span class="short_text" id="result_box" lang="pt"><span class="hps">suíte de</span> <span class="hps">software.</span></span></dd>
</dl>
</div>
</div>

<hr />
<h2 id="Temas"><a name="Themes">Temas</a></h2>

<p>Os temas são add-ons que personalizam a IU do aplicativo. Existem dois tipos de temas: temas leves e temas completos.</p>

<div class="column-container">
<div class="column-half">
<p><a href="https://addons.mozilla.org/en-US/developers/docs/themes">Temas Leves</a> são muito mais simples de implementar do que temas completos, mas fornece a personalização muito limitada.</p>
</div>

<div class="column-half">
<p><span id="result_box" lang="pt">Com <a href="https://developer.mozilla.org/en-US/docs/Themes">Temas Completos</a> você pode fazer modificações mais profundas na IU. A documentação para temas completos é fora da data, mas está ligada a aqui como uma possível base para a documentação atualizada.</span></p>
</div>
</div>

<hr />
<h2 id="Outros_tipos_de_complementos">Outros tipos de complementos</h2>

<p><span id="result_box" lang="pt"><a href="/pt-BR/docs/Mozilla/Add-ons/Creating_OpenSearch_plugins_for_Firefox">Plugins de Search Engine</a> são um tipo simples e muito específico de add-on: eles adicionam novos mecanismos de busca para barra de pesquisa do navegador.<br />
 <br />
 <a href="https://developer.mozilla.org/en-US/docs/Plugins">Plugins</a> ajuda a aplicação a entender o conteúdo web que não é suportado nativamente. Plugins NPAPI são uma tecnologia antiga  e os novos sites não devem usá-las. Em geral, os plugins não estão disponíveis na maioria dos sistemas móveis modernos, e os sites devem evitar usar plugins.</p>

<hr />
<h2 id="Mais_informações"><a name="Mais informações">Mais informações</a></h2>

<p>&nbsp;</p>

<table class="topicpage-table">
 <tbody>
  <tr>
   <td>
    <h2 class="Documentation" id="Documentation" name="Documentation">Documentação</h2>

    <dl>
     <dt><a href="/pt-BR/docs/Mozilla/Add-ons/Gerenciador_de_Add-on" title="Addons/Add-on Manager">Gerenciador de complementos (Gerenciador de Add-on)</a> {{gecko_minversion_inline("2.0")}}</dt>
     <dd>Usando o Gerenciador de Add-on.</dd>
     <dt><a href="/pt-BR/docs/Mozilla/Add-ons/Repositorio_Add-on" title="Addons/Add-on Repository">Repositório de Add-on</a> {{gecko_minversion_inline("2.0")}}</dt>
     <dd>O Repositório de Add-on é usado para encontrar add-ons disponíveis.</dd>
     <dt><a href="/pt-BR/docs/Mozilla/Add-ons/Interface-com-o-Repositorio_Add-on" title="Addons/Interfacing with the Add-on Repository">Interagindo com o Add-on Repository (Repositório de Add-on)</a> {{gecko_minversion_inline("2.0")}}</dt>
     <dd>Como usar o módulo <a href="/en-US/docs/Addons/Add-on_Repository" title="Addons/Add-on Repository"><code>AddonRepository.jsm</code></a> para interagir com o AMO.</dd>
     <dt><a href="/en-US/docs/Addons/Working_with_AMO" title="Addons/Working with AMO">Trabalhando com o AMO</a> {{gecko_minversion_inline("2.0")}}</dt>
     <dd>Dicas e sugestões de como fazer seu add-on funcionar com o repositório <a class="external" href="http://addons.mozilla.org" title="http://addons.mozilla.org/">addons.mozilla.org</a>.</dd>
     <dt><a href="/en-US/docs/Extensions" title="Extensions">Extensões</a></dt>
     <dd>Informação sobre como desenvolver extensões para os aplicativos Mozilla.</dd>
     <dt><a href="/en-US/docs/Addons/Add-on_guidelines" title="/en-US/docs/Addons/Add-on_guidelines">Diretrizes para Add-on</a></dt>
     <dd>Diretrizes para se criar ótimos add-ons com grandes chances de fazer sucesso!</dd>
     <dt><a href="/en-US/docs/Plugins" title="Plugins">Plugins</a></dt>
     <dd>Como desenvolver plugins.</dd>
     <dt><a href="/en-US/docs/Themes" title="Themes">Temas</a></dt>
     <dd>Desenvolver temas (ou skins (peles)) para os aplicativos Mozilla.</dd>
     <dt><a href="/en-US/docs/Creating_OpenSearch_plugins_for_Firefox" title="Creating OpenSearch plugins for Firefox">Criando plugins OpenSearch (Busca Aberta) para Firefox</a></dt>
     <dd>Como desenvolver plug-ins de busca para Firefox.</dd>
     <dt><a href="/en-US/docs/Performance" title="Performance">Desempenho</a></dt>
     <dd>Diretivas para desempenho e utilitáros para fazer seu add-on ter bom desempenho (e interagir bem com o dos outros).</dd>
    </dl>

    <p><span class="alllinks"><a href="/en-US/docs/tag/Add-ons" title="tag/Add-ons">Veja todas as páginas com o tag "Add-ons"...</a></span></p>
   </td>
   <td>
    <h2 class="Community" id="Community" name="Community">Comunidade</h2>

    <ul>
     <li>Veja os foruns sobre desenvolvimento de extensão para Mozilla... {{DiscussionList("dev-extensions", "mozilla.dev.extensions")}}</li>
     <li><a class="link-irc" href="irc://irc.mozilla.org/extdev">#extdev IRC channel</a></li>
     <li><a class="external" href="http://forums.mozillazine.org/?c=11">MozillaZine forum</a></li>
     <li><a class="external" href="/devnews/index.php/categories/about-addons" title="https://developer.mozilla.org/editor/fckeditor/core/editor/devnews/index.php/categories/about-addons/">about:addons newsletter</a></li>
     <li><a class="external" href="/web-tech" title="https://developer.mozilla.org/editor/fckeditor/core/editor/web-tech/">Mozilla's Web-Tech blog</a></li>
     <li><a class="external" href="http://mozdev.org/mailman/listinfo/project_owners">mozdev project owners</a></li>
     <li><a class="external" href="http://planet.mozilla.org/" title="http://planet.mozilla.org/">Planet Mozilla</a></li>
     <li><a href="/en-US/docs/Extensions/Community" title="Extensions/Community">Links para outras comunidades...</a></li>
    </ul>

    <h2 class="Tools" id="Tools" name="Tools">Ferramentas</h2>

    <ul>
     <li><a href="/en-US/docs/DOM_Inspector" title="DOM Inspector">DOM Inspector</a> - inspeciona o DOM, CSS, e XBL (Firefox e Thunderbird)</li>
     <li><a class="external" href="http://www.hacksrus.com/~ginda/venkman/" rel="external nofollow" title="http://www.hacksrus.com/~ginda/venkman/">Venkman</a>, um depurador de JavaScript (<a class="external" href="http://addons.mozilla.org/en-US/firefox/addon/216" rel="external nofollow" title="http://addons.mozilla.org/en-US/firefox/addon/216">Firefox</a>, <a class="external" href="http://addons.mozilla.org/en-US/thunderbird/addon/216" rel="external nofollow" title="http://addons.mozilla.org/en-US/thunderbird/addon/216">Thunderbird</a>)</li>
     <li><a class="link-https" href="https://builder.mozillalabs.com/" title="https://builder.mozillalabs.com/">Laboratório da Mozilla Construidora de Add-ons</a></li>
     <li><a class="link-https" href="https://addons.mozilla.org/en-US/firefox/addon/7434/" rel="external nofollow" title="https://addons.mozilla.org/en-US/firefox/addon/7434/">Extensão de Desenvolvimento de Extensão</a> um conjunto de ferramentas de desenvolvimento</li>
     <li><a class="external" href="http://www.gijsk.com/" rel="external nofollow" title="http://www.gijsk.com/">Chrome List</a> veja arquivos em chrome:// (<a class="external" href="http://addons.mozilla.org/en-US/firefox/addon/4453" rel="external nofollow" title="http://addons.mozilla.org/en-US/firefox/addon/4453">Firefox</a>, <a class="external" href="http://addons.mozilla.org/en-US/thunderbird/addon/4453" rel="external nofollow" title="http://addons.mozilla.org/en-US/thunderbird/addon/4453">Thunderbird</a>)</li>
     <li><a class="external" href="http://ted.mielczarek.org/code/mozilla/extensionwiz/" rel="external nofollow" title="http://ted.mielczarek.org/code/mozilla/extensionwiz/">Extensão Wizard</a> um gerador de estrutura para extensão web&nbsp; (Firefox and Thunderbird)</li>
    </ul>

    <p>... <a href="/en-US/docs/Setting_up_extension_development_environment#Development_extensions" title="Setting up extension development environment#Development extensions">mais ferramentas</a> ...</p>

    <h2 class="Related_Topics" id="Related_Topics" name="Related_Topics">Tópicos Relacionados</h2>

    <ul>
     <li><a href="/en-US/docs/XUL" title="XUL">XUL</a>, <a href="/en-US/docs/JavaScript" title="JavaScript">JavaScript</a>, <a href="/en-US/docs/XPCOM" title="XPCOM">XPCOM</a>, <a href="/en-US/docs/Themes" title="Themes">Temas</a>, <a href="/en-US/docs/Developer_Guide" title="Developing_Mozilla">Desenvolvendo para Mozilla</a>, <a href="/en-US/docs/Extensions" title="Extensions">Extensões</a></li>
    </ul>
   </td>
  </tr>
 </tbody>
</table>

<p>&nbsp;</p>

<p>&nbsp;</p>

