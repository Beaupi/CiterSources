# CiterSources
<html>
  <header>
  <script type="text/javascript">
function copieChoix()
 {
 var separ = ", ";
 var separ2 = ". ";
 var separ3 = "p. ";
 var separ4 = "n° ";
 var separ5 = " Consulté le : ";
 var separ6 = "Disponible sur : ";
 var separ7 = " [En ligne]";
 var separ8 = "\"";
var separ9 = " p.";
 if (document.form.livre.checked == true) {
 document.getElementById("result16").focus();
 var concat = document.getElementById("result").value.toUpperCase() + separ + document.getElementById("result2").value + separ2 + document.getElementById("result3").value.italics() + separ2 + document.getElementById("result6").value + separ + document.getElementById("result9").value + separ2 + document.getElementById("result12").value + separ9;
 document.getElementById("result16").value = concat;
 }
 if (document.form.chapitre.checked == true) {
 document.getElementById("result16").focus();
 var concat = document.getElementById("result").value.toUpperCase() + separ + document.getElementById("result2").value + separ2 + document.getElementById("result3").value.italics() + separ2 + document.getElementById("result6").value + separ + document.getElementById("result9").value + separ2 + document.getElementById("result7").value + separ + separ3 + document.getElementById("result13").value;
 document.getElementById("result16").value = concat;
 }
 if (document.form.article.checked == true) {
 document.getElementById("result16").focus();
 var concat = document.getElementById("result").value.toUpperCase() + separ + document.getElementById("result2").value + separ2 + separ8 + document.getElementById("result8").value + separ8 + separ2 + document.getElementById("result4").value.italics() + separ + separ4 + document.getElementById("result11").value + separ + document.getElementById("result9").value + separ2 + separ3 + document.getElementById("result13").value;
 document.getElementById("result16").value = concat;
 }
 if (document.form.web.checked == true) {
 document.getElementById("result16").focus();
 var concat = document.getElementById("result").value.toUpperCase() + separ + document.getElementById("result2").value + separ2 + separ8 + document.getElementById("result15").value + separ8 + separ2 + document.getElementById("result5").value.italics() + separ7 + separ + document.getElementById("result9").value + separ2 + separ5 + document.getElementById("result10").value + separ2 + separ6 + document.getElementById("result14").value;
 document.getElementById("result16").value = concat;
 }
 if ((document.form.livre.checked == false)&&(document.form.chapitre.checked == false)&&(document.form.article.checked == false)&&(document.form.web.checked == false)) {
 alert("Choississez un type de document !");
 return false
 }
 }
</script>


<form name="form"><br /><b>1 - Choisissez le type de document &agrave; citer.</b><br />  <br /><input name="typedoc" type="radio" value="Livre" onclick="
 if (this.checked) {
 this.form.result3.style.display='inline';
 this.form.result4.style.display='none';
 this.form.result5.style.display='none';
 this.form.result6.style.display='inline'; 
this.form.result7.style.display='none';
 this.form.result8.style.display='none';
 this.form.result9.style.display='inline';
 this.form.result10.style.display='none';
 this.form.result11.style.display='none';
 this.form.result12.style.display='inline';
 this.form.result13.style.display='none';
 this.form.result14.style.display='none';
 this.form.result15.style.display='none';
 }
 return true;" id="livre" />Livre <input name="typedoc" type="radio" value="Chapitre" onclick="
 if (this.checked) {
 this.form.result3.style.display='inline';
 this.form.result4.style.display='none';
 this.form.result5.style.display='none';
 this.form.result6.style.display='inline'; 
this.form.result7.style.display='inline';
 this.form.result8.style.display='none';
 this.form.result9.style.display='inline';
 this.form.result10.style.display='none';
 this.form.result11.style.display='none';
 this.form.result12.style.display='none';
 this.form.result13.style.display='inline';
 this.form.result14.style.display='none';
 this.form.result15.style.display='none';
 }
 return true;" id="chapitre" />Chapitre <input name="typedoc" type="radio" value="Article" onclick="
 if (this.checked) {
 this.form.result3.style.display='none';
 this.form.result4.style.display='inline';
 this.form.result5.style.display='none';
 this.form.result6.style.display='none';
 this.form.result7.style.display='none';
 this.form.result8.style.display='inline';
 this.form.result9.style.display='inline';
 this.form.result10.style.display='none';
 this.form.result11.style.display='inline';
 this.form.result12.style.display='none';
 this.form.result13.style.display='inline';
 this.form.result14.style.display='none';
 this.form.result15.style.display='none';
 }
 return true;" id="article" />Article de p&eacute;riodique (journaux, revues) <input name="typedoc" type="radio" value="Web" onclick="
 if (this.checked) {
 this.form.result3.style.display='none';
 this.form.result4.style.display='none';
 this.form.result5.style.display='inline';
 this.form.result6.style.display='none';
 this.form.result7.style.display='none';
 this.form.result8.style.display='none';
 this.form.result9.style.display='inline';
 this.form.result10.style.display='inline';
 this.form.result11.style.display='none';
 this.form.result12.style.display='none';
 this.form.result13.style.display='none';
 this.form.result14.style.display='inline';
 this.form.result15.style.display='inline';
 }
 return true;" id="web" />Page internet <br /><br /><b>2 - Remplissez les champs suivants :</b><br />(Passez la souris sur les champs pour avoir plus d'informations)<br /><br />
<table style="border-collapse: collapse; width: 450px; height: 80px;">
<tbody>
<tr>
<td style="padding-top:5px;"><input size="18" value="NOM de l'auteur" title="Vide si l'auteur est anonyme." id="result" /></td>
<td style="padding-top:5px;"><input size="18" value="Pr&eacute;nom de l'auteur" title="Vide si l'auteur est anonyme." id="result2" /></td>
<td style="padding-top:5px;"><input size="18" value="Titre du livre" id="result3" /></td>
</tr>
<tr>
<td style="padding-top:5px;"><input size="18" value="Titre du p&eacute;riodique" title="Par exemple Science &amp; vie junior, Wapiti..." id="result4" /></td>
<td style="padding-top:5px;"><input size="18" value="Nom du site web" id="result5" /></td>
<td style="padding-top:5px;"><input size="18" value="&Eacute;diteur" title="Se trouve sur la couverture ou dans les premi&egrave;res pages du livre." id="result6" /></td>
</tr>
<tr>
<td style="padding-top:5px;"><input size="18" value="Titre du chapitre" id="result7" /></td>
<td style="padding-top:5px;"><input size="18" value="Titre de l'article" id="result8" /></td>
<td style="padding-top:5px;"><input size="18" value="Date de publication" title="Se trouve dans les premi&egrave;res ou derni&egrave;res pages du livre, sous la mention 'D&eacute;p&ocirc;t l&eacute;gal'." id="result9" /></td>
</tr>
<tr>
<td style="padding-top:5px;"><input size="18" value="Date de consultation" title="Date exacte du jour comme '16/12/2012'." id="result10" /></td>
<td style="padding-top:5px;"><input size="18" value="Num&eacute;ro" id="result11" /></td>
<td style="padding-top:5px;"><input size="18" value="Nombre total de pages" title="Inscrire le dernier num&eacute;ro de page imprim&eacute;." id="result12" /></td>
</tr>
<tr>
<td style="padding-top:5px;"><input size="18" value="Pagination" title="Premi&egrave;re page et derni&egrave;re page de l'article ou du chapitre, comme '12-23'." id="result13" /></td>
<td style="padding-top:5px;"><input size="18" value="Adresse URL" title="De type 'http://www.exemple.fr/page45.html'." id="result14" /></td>
<td style="padding-top:5px;"><input size="18" value="Titre de la page web" title="Titre de la page &agrave; l'int&eacute;rieur du site web." id="result15" /></td>
</tr>
</tbody>
</table>
<br /><br /><input type="button" value="G&eacute;n&eacute;rer" onclick="copieChoix()" />    <input type="button" value="R&eacute;tablir les valeurs par d&eacute;faut" onclick="this.form.reset();" /> <br /><br />
<b>3 - Copiez-collez la r&eacute;f&eacute;rence bibliographique suivante :</b><br /><br /><textarea readonly="readonly" cols="50" rows="5" id="result16"></textarea> </form><br />
N'oubliez pas de <b>mettre en forme le titre</b> (situ&eacute; entre les balises &lt;i&gt; et &lt;/i&gt;) :<br />
- le <u>souligner</u>, pour une bibliographie &eacute;crite &agrave; la main<br />
- le mettre en <i>italique</i>, pour une bibliographie &agrave; l'ordinateur<br />
