---
version: prototype1
revision_id: 1274939
locale: pt-PT
slug: Mozilla/Add-ons
tags: "Extras" "Landing" "Mozilla" "Extensões" "extensão"
title: Extras (Add-ons)
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: True
table_of_contents_depth: 1
based_on: None
---
<div>{{AddonSidebar}}</div>

<p><span class="seoSummary">Os extras permitem que os responsáveis pelo desenvolvimento estendam e modifiquem a funcionalidade do Firefox. As mesmas são criadas&nbsp;utilizando as tecnologias da Web padrão - CSS, HTML e JavaScript - mais algumas APIs de JavaScript dedicadas. Entre outras coisas, um extra poderia:</span></p>

<ul>
 <li>Modificar e alterar a aparência ou conteúdo de um site em particualr</li>
 <li>Modificar a interface de utilizador do Firefox</li>
 <li>Adicionar novas funcionalidades ao Firefox</li>
</ul>

<h2 id="Desenvolver_extras">Desenvolver extras</h2>

<p>Existem, de momento, vários conjuntos&nbsp;de &nbsp;ferramentas utilizadas para desenvolver Aplicações Complementares mas as &nbsp;chamadas&nbsp;<a href="/en-US/Add-ons/WebExtensions">Extensões da Web</a>&nbsp;vão tornar-se o padrão pelo final de 2017. Das restantes a expectativa é de que se tornem&nbsp;<a href="/en-US/Add-ons/Overlay_Extensions">obsoletas</a>&nbsp;dentro do mesmo periodo de tempo.</p>

<p>Neste documento vai encontrar informação sobre&nbsp;as opções disponíveis para desenvolver aplicações complementares para que possa decidir qual a melhor para si agora e no futuro.</p>

<h3 id="Criar_um_Novo_Extra">Criar um Novo Extra</h3>

<p>Se está a desenvolver uma nova aplicação complementar recomendamos que escolha entre um dos dois seguintes métodos. Até que a transição para as Extensões da Web&nbsp;esteja finalizada, existirão prós e contras em relação a ambos os métodos. Por favor leia atentamente as opções para decidir qual a melhor para funcionar com a sua aplicação.</p>

<ul class="card-grid">
 <li style="position: relative; max-width: 400px;">
  <div style="margin-bottom: 70px;">
  <h4 id="Extensões_da_Web"><a href="pt-PT/Add-ons/WebExtensions">Extensões da Web</a></h4>

  <p>As Extensões da Web são o futuro das Aplicações Complementares para o Firefox. Se a puder utilizar, a API das Extensões da Web será a melhor escolha. Pode começar a desenvolver e publicar Extensões da Web imediatamente, mas as mesmas ainda estão num estado embrionário.<br />
   <br />
   A maioria das funcionalidades da API Extensões da Web estão também disponíveis &nbsp;no <a href="/en-US/Add-ons/WebExtensions/Browser_support_for_JavaScript_APIs">Firefox para&nbsp;Android</a>.</p>

  <p>We're preparing a first full release for <a href="https://wiki.mozilla.org/RapidRelease/Calendar">Firefox 48</a>.</p>
  </div>
  <a class="card-grid-button" href="/en-US/Add-ons/WebExtensions">Saber mais</a></li>
 <li style="position: relative; max-width: 400px;">
  <div style="margin-bottom: 70px;">
  <h4 id="SDK_de_Extras"><a href="/en-US/Add-ons/SDK">SDK de Extras</a></h4>

  <p>O SDK de Extra proporcina várias APIs para desenvolvimento de extras para o Firefox, e uma ferramenta para desenvolvimento, teste e finalização.</p>

  <p>Também pode executar as extensões de SDK de Extras no<a href="/en-US/Add-ons/SDK/Tutorials/Mobile_development">&nbsp;Firefox para&nbsp;Android</a>.</p>

  <p>We encourage you to use only <a href="/en-US/Add-ons/SDK/High-Level_APIs">high-level APIs</a> because this will make it easier to migrate to WebExtensions down the road.</p>
  </div>
  <a class="card-grid-button" href="/en-US/Add-ons/SDK">Learn more</a></li>
</ul>

<h3 id="Migrar_um_Extra_Existente">Migrar um Extra Existente</h3>

<p>There are changes coming to Firefox in the next year that will make browsing more reliable for users, and creating add-ons easier for developers. Your add-on may require updating to maintain its compatibility, but once this is done and the transition is complete, your add-on will be more interoperable, secure, and future-proof than ever.</p>

<p>We've created <a href="https://wiki.mozilla.org/Add-ons/developer/communication">resources, migration paths, office hours, and more</a>, to ensure you have the support you need to get through the transition.</p>

<p>To get started, use the <a href="https://compatibility-lookup.services.mozilla.com/">add-on compatibility checker</a> to see if your add-on will be affected.</p>

<h2 id="Publicação_de_extras">Publicação de extras</h2>

<p><a href="https://addons.mozilla.org">Addons.mozilla.org</a>, commonly known as "AMO," is Mozilla's official site for developers to list add-ons, and for users to discover them. By uploading your add-on to AMO, you can participate in our community of users and creators, and find an audience for your add-on.</p>

<p>You are not required to list your add-on on AMO, but starting with Firefox 40, your code must be signed by Mozilla or users won't be able to install it.</p>

<p>For an overview of the process of publishing your add-on, see <a href="https://developer.mozilla.org/en-US/Add-ons/Distribution">Signing and distributing your add-on</a>.</p>

<h2 id="Outros_tipos_de_extras">Outros tipos de extras</h2>

<p>Generally, when people speak of add-ons they're referring to extensions, but there are a few other add-on types that allow users to customize Firefox. Those add-ons include:</p>

<ul>
 <li><a href="https://developer.mozilla.org/Add-ons/Themes/Background">Lightweight themes</a> are a simple way to provide limited customization for Firefox.</li>
 <li><a href="/en-US/Add-ons/Firefox_for_Android">Mobile add-ons</a> are add-ons for Firefox for Android. Note, though, that we intend to deprecate some of the technology underlying these APIs. In the future, WebExtensions will be fully supported on Firefox for Android.</li>
 <li><a href="/en-US/docs/Creating_OpenSearch_plugins_for_Firefox">Search engine plugins</a> add new search engines to the browser's search bar.</li>
 <li><a href="/pt-PT/docs/Mozilla/Criação_de_um_complemento_de_dicionário_de_verificação_ortográfica">Dicionários do utilizador</a> são complementos que o deixam verificar a ortografia em diferentes idiomas.</li>
 <li><a href="https://support.mozilla.org/pt-PT/kb/use-firefox-interface-other-languages-language-pack">Pacotes de idioma </a>são complementos que o deixam ter mais idiomas disponíveis para a interface do utilizador do Firefox.</li>
</ul>

<hr />
<h2 id="Contacte-nos">Contacte-nos</h2>

<p>Pode utilizar as hiperligações abaixo para obetr ajuda, manter-se atualizado com as notícias relacionadas com os complementos, e dar-nos a sua opinião/comentário.</p>

<h3 id="Fórum_de_extras">Fórum de extras</h3>

<p>Utilize o <a href="https://discourse.mozilla-community.org/c/add-ons">fórum de conversação sobre os complementos</a> para discutir todos aspetos do desenvolvimento de complementos e obter ajuda.</p>

<h3 id="Listas_de_endereçosdiscussão">Listas de endereços/discussão</h3>

<p>Use the <strong>dev-addons</strong> list to discuss development of the add-ons ecosystem, including the development of the WebExtensions system and of AMO:</p>

<ul>
 <li><a href="https://mail.mozilla.org/listinfo/dev-addons">dev-addons list info</a></li>
 <li><a href="https://mail.mozilla.org/pipermail/dev-addons/">dev-addons archives</a></li>
</ul>

<h3 id="IRC">IRC</h3>

<p>If you're a fan of IRC, you can get in touch at:</p>

<ul>
 <li><a href="irc://irc.mozilla.org/addons">#addons</a> (discussion of the add-ons ecosystem)</li>
 <li><a href="irc://irc.mozilla.org/extdev">#extdev</a> (general discussion of add-on development)</li>
 <li><a href="irc://irc.mozilla.org/webextensions">#webextensions</a> (discussion of WebExtensions in particular)</li>
</ul>

