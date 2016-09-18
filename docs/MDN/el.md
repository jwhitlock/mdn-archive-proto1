---
version: prototype1
revision_id: 1120505
locale: el
slug: MDN
tags: "MDN Meta" "Landing" "l10n:priority"
title: Project:Αποσαφηνισμοί
summary: 
keywords: 
needs_technical_review: False
needs_editorial_review: False
needs_localization: False
table_of_contents_depth: 1
based_on: None
---
<h2 id="Εισαγωγή">Εισαγωγή</h2>

<p>Οι <strong>Αποσαφηνισμοί</strong> στο MDC wiki είναι η διαδικασία επίλυσης <em style="font-style:italic">ασαφειών</em><em>,</em> αναφερόμενοι στα θέματα που δημιουργούνται όταν άρθρα σχετικά με δύο ή περισσότερα αντικείμενα έχουν τον ίδιο "φυσικό" τίτλο.</p>

<p>Κάθε σελίδα μέσα στο wiki θα πρέπει να έχει έναν μοναδικό τίτλο. Αυτό μπορεί να προκαλέσει προβλήματα όταν δύο σελίδες, θεωρητικά, έχουν τον ίδιο ακριβώς τίτλο. Για παράδειγμα, το <a href="/en/indexOf" title="en/indexOf">indexOf</a> είναι μια μέθοδος και για String αλλά και για Array objects στην JavaScript.</p>

<div class="note"><span class="highlightred"><strong>Σημείωση</strong>: η ακόλουθη πολιτική έχει αλλάξει από την πρώτη της έκδοση.</span></div>

<p>Όπως και στην Wikipedia, διαφοροποιούμε τις σελίδες τοποθετώντας περιεχόμενο σε παρενθέσεις μετά το όνομα (π.χ., "Mercury (planet)"). Ωστόσο, κάποιοι χρήστες που θα ψάξουν πληροφορίες για το "indexOf" είναι πολύ πιθανό να έρθουν στο Devmo και να γράψουν "indexOf" μέσα στο search box. Η αναζήτηση θα δώσει αποτελέσματα για όλες τις σελίδες που περιέχουν την λέξη "indexOf", κάτι που δεν θα βοηθούσε γενικότερα, δεδομένου ότι θα εμφανιστεί σε τίτλους, άρθρα, οδηγούς, δείγματα κώδικα, και αναφορές μέσα σε όλο το wiki. Με σκοπό να βοηθήσουμε όσους ψάχνουν κάτι τέτοιο να το βρούνε πιο εύκολα, ξεκινήσαμε να προσθέτουμε σελίδες αποσαφηνισμού (disambiguation pages) στο wiki.</p>

<h3 id="When_to_create_a_disambiguation_page" name="When_to_create_a_disambiguation_page">Πότε να δημιουργήσετε μια σελίδα αποσαφηνισμού</h3>

<p>Οι σελίδες αποσαφηνισμού θα πρέπει να δημιουργούνται μόνο για να επιλύσουν κάποιο θέμα ασάφειας ανάμεσα σε δύο ή περισσότερες σελίδες.</p>

<h3 id="How_to_create_a_disambiguation_page" name="How_to_create_a_disambiguation_page">Πώς να δημιουργήσετε μια σελίδα αποσαφηνισμού</h3>

<p>Οι σελίδες αποσαφηνισμού είναι σχεδιασμένες ξεχωριστά από τους συντάκτες να συνδέονται με όλες τις σελίδες που ο χρήστης μπορεί να ψάχνει για έναν όρο. Αυτό βοηθάει τους χρήστες να βρούν γρήγορα αυτό που ψάχνουν.</p>

<p>Για να δημιουργήσετε μια σελίδα αποσαφηνισμού, απλώς δημιουργήστε μια σελίδα όπου ο τίτλος της θα είναι ο ασαφής όρος; για παράδειγμα, <a href="/en/indexOf" title="en/indexOf">indexOf</a>.</p>

<h3 id="What_to_include_in_a_disambiguation_page" name="What_to_include_in_a_disambiguation_page">Τι να προσθέσετε σε μια σελίδα αποσαφηνισμού</h3>

<p>Όταν δημιουργείτε μια σελίδα αποσαφηνισμού, θα πρέπει να κάνετε τα ακόλουθα:</p>

<h4 id="Short_introductory_line" name="Short_introductory_line">Σύντομος πρόλογος μιας γραμμής</h4>

<p>Προσθέστε μια σειρά σύντομου προλόγου στην αρχή, όπως για παράδειγμα&nbsp;"το<strong> indexOf</strong> είναι μια μέθοδος για διάφορα JavaScript objects:", "το <strong>indexOf</strong> χρησιμοποιείται με διάφορους τρόπους:", ή, πιο απλά, "το <strong>indexOf</strong> μπορεί να σημαίνει πολλά πράγματα:".</p>

<h4 id="The_.22disambig.22_template" name="The_.22disambig.22_template">Το "disambig" template</h4>

<p>Προσθέστε την <a href="/Project:en/Custom_Templates#Template:disambig" title="Project:en/Custom_Templates#Template:disambig">disambig template</a> στο τέλος της σελίδας. Αυτό εισάγει μια standard σημείωση καθώς και την κατηγορία αποσαφηνισμού.</p>

<h4 id="Linked_list_of_ambiguous_page_titles" name="Linked_list_of_ambiguous_page_titles">Συνδεδεμένη λίστα τίτλων μια ασαφούς σελίδας</h4>

<p>Απλώς προσθέστε μια linked list από τους τίτλους μιας ασαφούς σελίδας, με μια σύντομη περιγραφή για το καθένα. Θα αναφερόμαστε στην σελίδα <a href="/en/indexOf" title="en/indexOf">indexOf</a> για περισσ.</p>

<p>Σε περίπτωση που το παραπάνω δεν είναι εύκολα χρήσιμο, μπορείτε να αναδιατάξετε τις πληροφορίες σε νέα λογικά τμήματα στην σελίδα.</p>

<h3 id="Best_Practices" name="Best_Practices">Καλύτερες πρακτικές</h3>

<ol>
 <li>Οι σελίδες αποσαφηνισμού θα να δείχνουν μόνο σε σελίδες που υπάρχουν μέσα στο wiki.</li>
 <li>Μην βάζετε συνδέσμους σε άλλες σελίδες στην σύνοψη των σελίδων αποσαφηνισμού. Για παράδειγμα, μην κάνετε αυτό: "<em><a href="/en/indexOf" title="en/indexOf">indexOf</a> - <a href="/en/DOM/form.method" title="en/DOM/form.method">method</a> for the <a href="/en/String" title="en/String">String</a> object in <a href="/en/JavaScript" title="en/JavaScript">JavaScript</a></em>". Απλά αφήστε το ως "<em><a href="/en/indexOf" title="en/indexOf">indexOf</a> - method for the String object in JavaScript</em>". Τα επιπρόσθετα links δεν βοηθάνε σε κάτι σε μια σελίδα αποσαφηνισμού.</li>
 <li>Μικρύνετε τον τίτλο του συνδέσμου, αν είναι απαραίτητο, για τον όρο που πρόκειται να αποσαφηνιστεί. Αντί να δείχνετε στο <a href="/en/JavaScript/Reference/Global_Objects/String/indexOf" title="en/Core_JavaScript_1.5_Reference/Global_Objects/String/indexOf">Core JavaScript 1.5 Reference:Objects:String:indexOf</a>, χρησιμοποιείστε εναλλακτικά την πιο σύντομη μορφή <a href="/en/JavaScript/Reference/Global_Objects/String/indexOf" title="en/Core_JavaScript_1.5_Reference/Global_Objects/String/indexOf">indexOf</a>.</li>
 <li>Οι σελίδες αποσαφηνισμού δεν προσφέρονται για τακτικές "free association". <strong>Χρησιμοποιείστε τες προσεκτικά και μόνο όταν χρειάζεται.</strong></li>
</ol>

<h3 id="Fixing_links_to_disambiguated_topics" name="Fixing_links_to_disambiguated_topics">Διορθώνοντας συνδέσμους σε θέματα αποσαφηνισμού</h3>

<p>Αφού έχετε δημιουργήσει μια disambiguation page, κάντε κλικ στον σύνδεσμο "What links here" για να δείτε αν οποιαδήποτε σελίδα οδηγεί στην νέα disambiguation page. Σ'αυτήν την περίπτωση, παρακαλούμε πηγαίνετε σε αυτές τις σελίδες και αλλάξτε τα links όπου είναι δυνατό, ώστε να δείχνουν στην σωστή σελίδα μέσα στο wiki.</p>

<p>Για παράδειγμα, αν μια σελίδα που αναφέρεται στην μέθοδο JavaScript String object's <code>indexOf</code>, συνδέεται με την <a href="/en/indexOf" title="en/indexOf">indexOf</a> σελίδα disambiguation, αυτό το link θα πρέπει να αλλάξει έτσι ώστε να δείχνει κατευθείαν στην σελίδα <a href="/en/JavaScript/Reference/Global_Objects/String/indexOf" title="en/Core_JavaScript_1.5_Reference/Global_Objects/String/indexOf">Core JavaScript 1.5 Reference:Objects:String:indexOf</a>.</p>

<p>Εάν δημιουργείτε μια σελίδα αποσαφηνισμού που θα περιλαμβάνει links που οδηγούν σε μια υπάρχουσα σελίδα, κάντε κλικ στο "What links here" για να βρείτε όλες τις σελίδες που συνδέονται με την σελίδα που πρόκειται να μετακινήσετε. Σιγουρευτείτε ότι εκείνες οι σελίδες δεν θα υποστούν αλλαγές πριν κάνετε την μεταφορά.</p>

<p><strong>Ο κώδικας τιμής για την δημιουργία σελίδων αποσαφηνισμού είναι να διορθωθούν όλα τα links που συνδέονται με αυτή.</strong></p>

<h3 id="If_you_need_help_or_have_questions" name="If_you_need_help_or_have_questions">Εάν χρειάζεστε βοήθεια ή έχετε ερωτήσεις</h3>

<p>Εάν δεν γνωρίζετε πώς να ονομάσετε ή να αποσαφηνίσετε μια σελίδα, παρακαλούμε επικοινωνήστε με email στον <a class="link-mailto" href="mailto:eshepherd@mozilla.com" title="mailto:eshepherd@mozilla.com">Eric Shepherd</a> ή στείλτε το στην <a class="external" href="http://mail.mozilla.org/listinfo/devmo-general">devmo-general mailing list</a>.</p>

<p>Εναλλακτικά, μπείτε στο IRC στον server <code>irc.mozilla.org</code> και ρωτήστε κάποιον στο κανάλι <code><a class="link-irc" href="irc://irc.mozilla.org/#devmo">#devmo</a></code>.</p>

<h3 id="For_more_information" name="For_more_information">Για περισσότερες πληροφορίες</h3>

<p>Η σελίδα <a class="external" href="http://en.wikipedia.org/wiki/Disambiguation">Wikipedia Disambiguation page</a> περιέχει συνοπτικά τις πολιτικές και τους τρόπους προσέγγισης. Σημειώστε ότι οι πολιτικές μας δεν συμφωνούν απόλυτα.</p>

<h5 id="Subnav">Subnav</h5>

<ol>
 <li><a href="/el/docs/MDN/About">About MDN</a>

  <ol>
   <li><a href="/el/docs/MDN/About">About MDN</a></li>
   <li><a href="/el/docs/MDN/About/Promote">Promote MDN</a></li>
   <li><a href="/el/docs/MDN/Feedback">Send feedback about MDN</a></li>
  </ol>
 </li>
 <li><a href="/el/docs/MDN/Getting_started">Get started on MDN</a></li>
 <li><a href="/el/docs/MDN/Contribute">Help improve MDN</a>
  <ol>
   <li><a href="/el/docs/MDN/Contribute">Help improve MDN</a></li>
   <li><a href="/el/docs/MDN/Contribute/Howto">Things you can do</a></li>
   <li><a href="/el/docs/MDN/Contribute/Localize">Localizing MDN</a></li>
   <li><a href="/el/docs/MDN/Contribute/Editor">MDN editor UI</a></li>
   <li><a href="/el/docs/MDN/Contribute/Tools">Tools for power users</a></li>
   <li><a href="/el/docs/MDN/Contribute/Guidelines">Guidelines</a></li>
   <li><a href="/el/docs/MDN/Contribute/Processes">Work processes</a></li>
   <li><a href="/el/docs/MDN/Contribute/Structures">Content structures</a></li>
  </ol>
 </li>
 <li><a href="/el/docs/MDN/Kuma">Kuma: MDN's wiki platform</a></li>
 <li><a href="/el/docs/MDN/Community">Join the MDN community</a></li>
 <li><a href="/el/docs/MDN/Doc_status">Doc status by topic</a>
  <ol>
   <li><a href="/el/docs/MDN/Doc_status">Doc status by topic</a></li>
   <li><a href="/el/docs/MDN/Doc_status/Overview">Are we documented yet?</a></li>
  </ol>
 </li>
</ol>

