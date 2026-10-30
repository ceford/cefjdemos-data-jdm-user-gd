<!--
{
    "source": "https://jdocmanual.org/jdocmanual?article=user/templates/pagination-wrap",
    "title": "Pasgadh na duilleige",
    "description": "Ionnsaich d\u00f2igh sh\u00ecmplidh gus an liosta de dhuilleagan a phasgadh air scrionaichean caola. ",
    "author": ""
}
-->

Ann an Joomla, faodaidh liostaichean de dh’artaigilean, luchd-cleachdaidh agus nithean eile a bhith glè fhada, agus mar sin tha iad air an taisbeanadh ann am buidhnean, 20 mar an roghainn bhunaiteach.

## Am bàr àbhaisteach de dhuilleagan

Gus seòladh eadar na buidhnean, tha bàr de dhuilleagan fon liosta de nithean a leigeas leis an neach-cleachdaidh an ath bhuidheann de nithean a thaghadh, mar a chithear san dealbh seo:

![bàr àbhaisteach dhuilleagan na liosta](../../../en/images/templates/pagination-wrap/01-pagination-wide-screen.png)

## Duilleagan air scrionaichean caola

Tha am bàr de dhuilleagan ag obair gu math air scrionaichean leathann. Ach, air scrionaichean caola, faodaidh am bàr de dhuilleagan a bhith nas leatha na an sgrìn. Tha seo ag adhbharachadh gum feumar sgroladh chun na làimhe deise gus nithean eile air an duilleig a lorg, leithid clàir-hamburger.

![am bàr de dhuilleagan air sgrìn caol](../../../en/images/templates/pagination-wrap/02-pagination-narrow-screen.png)

San dealbh gu h-àrd, tha nithean sam bith san raon ghlas air an làimh dheis *far an sgrìn* an toiseach agus tha coltas ann gun tèid an ionndrainn. Feumaidh an neach-cleachdaidh sgroladh chun na làimhe deise gus am faicinn. Anns a’ chùis seo, ’s iad na nithean far na sgrìn an ìomhaigheag Innealan aig a’ mhullach air an làimh dheis agus an ìomhaigheag Clàir aig a’ bhonn air an làimh dheis.

## Ceartaich le bhith a’ dèanamh ath-sgrìobhadh air teamplaid

Tha an ceartachadh seo a’ cur clas *flex-wrap* ris a’ chòd a chruthaicheas am bàr de dhuilleagan.

- Anns a’ cheann-cùil, rach gu System > Administrator Templates > Atum Details and Files
- Roghainneil, tagh html > layouts dìreach gus faicinn dè tha ann
- Tagh an taba **Create Overrides**
- Anns a’ bhogsa Layouts tagh **joomla** agus an uair sin **pagination**
- Anns an taba Editor tagh html > layouts > joomla > pagination > **links.php**
- Lorg loidhne 70 anns a bheil `<ul class="pagination ms-auto me-0">`
- Cuir `flex-wrap` ri liosta nan clasaichean: `<ul class="pagination ms-auto me-0 flex-wrap">`
- **Sàbhail & Dùin**
- Roghainneil: Faodaidh tu /html/layouts/joomla/pagination/link.php agus /html/layouts/joomla/pagination/links.php a sguabadh às

Seall air an toradh air scrionaichean leathann agus caola. Tha an sgrìn caol a-nis a’ sealltainn na h-ìomhaigheig Innealan agus na h-ìomhaigheig Clàir taobh a-staigh leud àbhaisteach na sgrìn:

![am bàr atharraichte de dhuilleagan air sgrìn caol](../../../en/images/templates/pagination-wrap/02-modified-pagination-narrow-screen.png)

Airson teamplaid na làraich, lean an stiùireadh seo ach cruthaich ath-sgrìobhadh ann an teamplaid Cassiopeia.

*Air eadar-theangachadh le openai.com*