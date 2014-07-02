Mapfishapp : sélecteur WMSle vendredi  1 octobre 2010, 20:00 
        
    <div class="post-content"><p>Camptocamp a intégré un nouveau et pratique sélecteur de serveur WMS pour
mapfishapp. Il est composé d'une liste de serveurs, la sélection d'un serveur
déclenche un getCapabilities et liste les couches du serveur. La liste des
serveurs provient d'un flux JSON ressemblant à ceci :</p>
<pre>
{
  servers: [
    {&quot;name&quot;: &quot;GeoLittoral&quot;, &quot;url&quot;: &quot;http://geolittoral.application.equipement.gouv.fr/wms/metropole&quot;},
    {&quot;name&quot;: &quot;GeoBretagne.fr&quot;, &quot;url&quot;: &quot;http://geobretagne.fr/geoserver/wms&quot;}
  ]
}
</pre>
<p>Le fichier de conf javascript permet de modifier l'origine de ce flux avec
le paramètre <code>GEOR.custom.WMS_LIST_URL</code>. Cette fonctionnalité est
disponible à partir du <a href="http://csm-bretagne.fr/hudson/view/georchestra/job/mapfishapp-custom/17/" hreflang="en">build #17</a>.</p>
<p><a href="/public/screenshots/wms-selector.png"><img src="/public/screenshots/.wms-selector_s.jpg" alt="sélecteur wms" title="sélecteur wms, oct. 2010" /></a></p></div>

      </div>

  