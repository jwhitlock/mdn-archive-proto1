---
version: prototype1
revision_id: 1267819
locale: fr
slug: Web/JavaScript/Reference/Opérateurs/Opérateurs_de_comparaison
tags: "JavaScript" "Opérateur" "Référence(2)"
title: Opérateurs de comparaison
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<div>{{jsSidebar("Operators")}}</div>

<p>JavaScript possède des opérateurs de comparaisons stricts et des opérateurs de comparaisons qui effectuent des conversions. Une comparaison strict (ex. : <code>===</code>) ne sera vraie que si les deux opérandes sont du même type. La comparaison d'égalité faible (<code>==</code>) convertira les deux opérandes en un même type avant d'effectuer la comparaison. Pour les comparaisons relationnelles (ex. : <code>&lt;=</code>), les opérandes sont tout d'abord converties en valeurs, puis en valeurs du même type, enfin la comparaison est effectuée.</p>

<p>Les chaînes de caractères sont comparées en fonction de l'ordre lexicographique, avec des valeurs Unicode.</p>

<p>Les règles de comparaisons pour <a href="/fr/docs/Web/JavaScript/Structures_de_données#Les_valeurs_primitives">les types primitifs</a> sont les suivantes :</p>

<ul>
 <li>Deux chaînes de caractères sont strictement égales lorsqu'elles ont la même séquence de caractères, la même longueur et les mêmes caractères aux mêmes positions.</li>
 <li>Deux nombres sont strictement égaux lorsqu'ils ont la même valeur. {{jsxref("Objets_globaux/NaN","NaN")}} n'est égal à rien, y compis lui-même. Le zéro positif et le zéro négatif sont considérés égaux.</li>
 <li>Deux booléens sont strictement égaux s'ils valent tous les deux <code>true</code> ou tous les deux <code>false</code>.</li>
 <li>Deux objets distincts ne sont jamais égaux l'un à l'autre (pour l'égalité faible et stricte).</li>
 <li>Deux objets sont égaux si les deux opérandes sont des références au même objet.</li>
 <li>Les types nul et indéfini sont strictement égaux à eux-mêmes et sont faiblement égaux l'un à autre.</li>
</ul>

<h2 id="Les_opérateurs_d'égalité">Les opérateurs d'égalité</h2>

<h3 id="Égalité_simple_()"><a>Égalité simple (==)</a></h3>

<p>L'opérateur d'égalité simple convertit les deux opérandes s'<strong>ils ne sont pas du même type</strong>, ensuite la comparaison stricte est appliquée. Si <strong>les deux opérandes sont des objets</strong>, le moteur JavaScript comparera les références internes pour voir si elles réfèrent au même objet en mémoire.</p>

<h4 id="Syntaxe">Syntaxe</h4>

<pre class="syntaxbox">
x == y
</pre>

<h4 id="Exemples">Exemples</h4>

<pre class="brush: js">
 1   ==  1;        // true
"1"  ==  1;        // true
 1   == '1';       // true
 0   == false;     // true
 0   == null;      // false
 0   == undefined  // false
null == undefined  // true

var obj1 = { "valeur": "clé"};
var obj2 = { "valeur": "clé"};
obj1 == obj2       // false
</pre>

<h3 id="Inégalité_simple_(!)"><a>Inégalité simple (!=)</a></h3>

<p>L'opérateur d'inégalité simple renvoie <code>true</code> si les deux opérandes ne sont pas égaux. Si les deux opérandes <strong>ne sont pas du même type</strong>, une conversion sera effectuée vers un type adéquat. <strong>Si les deux opérandes sont des objets,</strong> le moteur JavaScript comparera les références internes pour voir si elles réfèrent à des objets différents en mémoire.</p>

<h4 id="Syntaxe_2">Syntaxe</h4>

<pre class="syntaxbox">
x != y</pre>

<h4 id="Exemples_2">Exemples</h4>

<pre class="brush: js">
1 !=   2;     // true
1 !=  "1";    // false
1 !=  '1';    // false
1 !=  true;   // false
0 !=  false;  // false
</pre>

<h3 id="Égalité_stricte_()"><a>Égalité stricte (===)</a></h3>

<p>L'opérateur d'égalité stricte renvoie <code>true</code> si les opérandes sont strictement égaux (voir ci-avant), <strong>aucune conversion de type n'est effectuée</strong>.</p>

<h4 id="Syntaxe_3">Syntaxe</h4>

<pre class="syntaxbox">
x === y</pre>

<h4 id="Exemples_3">Exemples</h4>

<pre class="brush: js ">
3 === 3   // true
3 === '3' // false</pre>

<h3 id="Inégalité_stricte_(!)"><a>Inégalité stricte (!==)</a></h3>

<p>L'opérateur d'inégalité stricte renvoie <code>true</code> si les opérandes sont de types différents ou ne sont pas égaux.</p>

<h4 id="Syntaxe_4">Syntaxe</h4>

<pre class="syntaxbox">
x !== y</pre>

<h4 id="Exemples_4">Exemples</h4>

<pre class="brush: js">
3 !== '3' // true
4 !== 3   // true
</pre>

<h2 id="Opérateurs_relationnels">Opérateurs relationnels</h2>

<div class="note">
<p><strong>Note :</strong> Chacun de ces opérateurs invoquera la fonction <code>valueOf()</code> des opérandes qui sont des objets avant d'effectuer la comparaison.</p>
</div>

<h3 id="Supérieur_strict_(&gt;)"><a>Supérieur strict (&gt;)</a></h3>

<p>Cet opérateur renvoie <code>true</code> si l'opérande gauche est strictement supérieur à l'opérande droit.</p>

<h4 id="Syntaxe_5">Syntaxe</h4>

<pre class="syntaxbox">
x &gt; y</pre>

<h4 id="Exemples_5">Exemples</h4>

<pre class="brush: js">
4 &gt; 3; // true
</pre>

<h3 id="Supérieur_ou_égal_(&gt;)"><a>Supérieur ou égal (&gt;=)</a></h3>

<p>Cet opérateur renvoie <code>true</code> si l'opérande gauche est supérieur ou égal à l'opérande droit</p>

<h4 id="Syntaxe_6">Syntaxe</h4>

<pre class="syntaxbox">
 x &gt;= y</pre>

<h4 id="Exemples_6">Exemples</h4>

<pre class="brush: js">
4 &gt;= 3; // true
3 &gt;= 3; // true
</pre>

<h3 id="Inférieur_strict_(&lt;)"><a>Inférieur strict (&lt;)</a></h3>

<p>Cet opérateur renvoie <code>true</code> si l'opérande gauche est strictement inférieur à l'opérande droit</p>

<h4 id="Syntaxe_7">Syntaxe</h4>

<pre class="syntaxbox">
 x &lt; y</pre>

<h4 id="Exemples_7">Exemples</h4>

<pre class="brush: js">
3 &lt; 4; // true
</pre>

<h3 id="Inférieur_ou_égal_(&lt;)"><a>Inférieur ou égal (&lt;=)</a></h3>

<p>Cet opérateur renvoie <code>true</code> si l'opérande gauche est inférieur ou égal à l'opérande droit</p>

<h4 id="Syntaxe_8">Syntaxe</h4>

<pre class="syntaxbox">
 x &lt;= y</pre>

<h4 id="Exemples_8">Exemples</h4>

<pre class="brush: js">
3 &lt;= 4; // true
</pre>

<h2 id="Utiliser_les_opérateurs_d'égalité">Utiliser les opérateurs d'égalité</h2>

<p>Les opérateurs d'égalité/inégalité faible (<code>==</code> et <code>!=</code>) utilisent <a href="https://www.ecma-international.org/ecma-262/5.1/#sec-11.9.3">l'algorithme de comparaison d'égalité abstraite</a> afin de comparer les deux opérandes. Si les opérandes sont de types primitifs différents, le moteur tentera de les convertir en un même type avant d'effectuer la comparaison. Ainsi, dans l'expression <code>5 == '5'</code>, la chaîne de droite est convertie en un nombre avant que la comparaison soit faite.</p>

<p>Les opérateurs d'égalité/inégalité stricte (<code>===</code> et <code>!==</code>) utilisent <a href="https://www.ecma-international.org/ecma-262/5.1/#sec-11.9.6">l'algorithme de comparaison d'égalité stricte</a>. Si les opérandes sont de types différents, le résultat sera toujours <code>false</code>, on aura donc <code>5 !== '5'</code>.</p>

<p>Selon qu'on souhaite comparer des opérandes qui sont censés avoir le même type ou non, on utilisera l'un ou l'autre type d'opérateur.</p>

<p>Si un opérande doit être comparé à un autre type, le moteur effectuera une conversion de la façon suivante :</p>

<ul>
 <li>Lorsqu'une comparaison est opérée entre une chaîne de caractères et un nombre, Javascript tente de convertir la chaine en une valeur numérique. Une valeur mathématique est obtenue à partir de la chaîne littérale numérique, puis celle-ci est arrondie à une valeur de type Nombre.</li>
 <li>Si l'un des opérandes est de type booléen, <code>true</code> sera converti en 1 et <code>false</code> en +0.</li>
 <li>Si on compare un objet avec un nombre ou une chaîne, le moteur JavaScript tentera de renvoyer la valeur par défaut de l'objet. Les opérateurs opèrent une conversion grâce aux méthodes <code>valueOf</code> (pour obtenir un nombre) et <code>toString</code> (pour obtenir une chaîne de caractères). Si cela ne fonctionne pas, une exception sera levée.</li>
 <li>Un objet sera converti en un type primitif autre uniquement si l'autre opérande est un type primitif (autre qu'objet). Si les deux opérandes sont des objets, ils seront comparés comme deux objets (voir ci-avant) et l'égalité ne sera vérifiée que si les opérandes font référence au même objet en mémoire</li>
</ul>

<div class="note">
<p><strong>Note :</strong> Voir également la page sur <a href="/fr/docs/Web/JavaScript/Les_diff%C3%A9rents_tests_d_%C3%A9galit%C3%A9_comment_les_utiliser">les différents tests d'égalité et quand les utiliser</a>.</p>
</div>

<div class="note"><strong>Note :</strong> Les objets String sont du type objet et ne sont pas de simples chaînes de caractères ! Cela peut parfois avoir des conséquences surprenantes :</div>

<pre class="brush:js">
// true car les deux opérandes sont du type primitif chaîne de caractères
'toto' === 'toto'

var a = new String('toto');
var b = new String('toto');

// false car a et b sont du type objet mais font référence à deux objets distincts
a == b 

// false car a et b sont du type objet mais font référence à deux objets distincts
a === b 

// true car a et 'toto' sont de type différents et lorsque a est
// converti, la fonction de conversion renvoie bien la chaîne 'toto'
a == 'toto' </pre>

<h2 id="Spécifications">Spécifications</h2>

<table class="standard-table">
 <tbody>
  <tr>
   <th scope="col">Spécification</th>
   <th scope="col">État</th>
   <th scope="col">Commentaires</th>
  </tr>
  <tr>
   <td>{{SpecName('ES1')}}</td>
   <td>{{Spec2('ES1')}}</td>
   <td>Définition initiale. Implémentée avec JavaScript 1.0</td>
  </tr>
  <tr>
   <td>{{SpecName('ES3')}}</td>
   <td>{{Spec2('ES3')}}</td>
   <td>Ajoute les opérateurs <code>===</code> et <code>!==</code>. Implémentés avec JavaScript 1.3</td>
  </tr>
  <tr>
   <td>{{SpecName('ES5.1', '#sec-11.8')}}</td>
   <td>{{Spec2('ES5.1')}}</td>
   <td>Définis dans plusieurs sections de la spécification : <a href="https://www.ecma-international.org/ecma-262/5.1/#sec-11.8">opérateurs relationnels</a>, <a href="https://www.ecma-international.org/ecma-262/5.1/#sec-11.9">opérateurs d'égalité</a></td>
  </tr>
  <tr>
   <td>{{SpecName('ES6', '#sec-relational-operators')}}</td>
   <td>{{Spec2('ES6')}}</td>
   <td>Définis dans plusieurs sections de la spécification : <a href="https://www.ecma-international.org/ecma-262/6.0/#sec-relational-operators">opérateurs relationnels</a>, <a href="https://www.ecma-international.org/ecma-262/6.0/#sec-equality-operators">opérateurs d'égalité</a></td>
  </tr>
  <tr>
   <td>{{SpecName('ESDraft', '#sec-relational-operators')}}</td>
   <td>{{Spec2('ESDraft')}}</td>
   <td>Définis dans plusieurs sections de la spécification : <a href="https://tc39.github.io/ecma262/#sec-relational-operators">opérateurs relationnels</a>, <a href="https://tc39.github.io/ecma262/#sec-equality-operators">opérateurs d'égalité</a></td>
  </tr>
 </tbody>
</table>

<h2 id="Compatibilité_des_navigateurs">Compatibilité des navigateurs</h2>

<p>{{CompatibilityTable}}</p>

<div id="compat-desktop">
<table class="compat-table">
 <tbody>
  <tr>
   <th>Fonctionnalité</th>
   <th>Chrome</th>
   <th>Firefox (Gecko)</th>
   <th>Edge</th>
   <th>Internet Explorer</th>
   <th>Opera</th>
   <th>Safari</th>
  </tr>
  <tr>
   <td>Support simple</td>
   <td>{{CompatVersionUnknown}}</td>
   <td>{{CompatVersionUnknown}}</td>
   <td>{{CompatVersionUnknown}}</td>
   <td>{{CompatVersionUnknown}}</td>
   <td>{{CompatVersionUnknown}}</td>
   <td>{{CompatVersionUnknown}}</td>
  </tr>
 </tbody>
</table>
</div>

<div id="compat-mobile">
<table class="compat-table">
 <tbody>
  <tr>
   <th>Fonctionnalité</th>
   <th>Android</th>
   <th>Chrome pour Android</th>
   <th>Firefox Mobile (Gecko)</th>
   <th>Edge</th>
   <th>IE Mobile</th>
   <th>Opera Mobile</th>
   <th>Safari Mobile</th>
  </tr>
  <tr>
   <td>Support simple</td>
   <td>{{CompatVersionUnknown}}</td>
   <td>{{CompatVersionUnknown}}</td>
   <td>{{CompatVersionUnknown}}</td>
   <td>{{CompatVersionUnknown}}</td>
   <td>{{CompatVersionUnknown}}</td>
   <td>{{CompatVersionUnknown}}</td>
   <td>{{CompatVersionUnknown}}</td>
  </tr>
 </tbody>
</table>
</div>

<h2 id="Voir_aussi">Voir aussi</h2>

<ul>
 <li>{{jsxref("Object.is()")}}</li>
 <li>{{jsxref("Math.sign()")}}</li>
 <li><a href="/fr/docs/Web/JavaScript/Guide/%C3%89galit%C3%A9_en_JavaScript">L'égalité en JavaScript</a></li>
 <li><a href="/fr/docs/Web/JavaScript/Les_diff%C3%A9rents_tests_d_%C3%A9galit%C3%A9_comment_les_utiliser">Les différents tests d'égalité en JavaScript</a></li>
</ul>

