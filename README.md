# Landing Page
-Realizzazione di una Landing Full Screen, Cross Browser, Cross Device-

--FULL SCREEN--

Per realizzare una pagina come quella in oggetto si puo' ricorrere a piu' metodi e a tecnologie diverse. 
La chiave del progetto risiede nell'aspetto "cross browsing" del background animato, per il cui sviluppo avrei potuto scegliere una tecnica piu'sofisticata e d'impatto, ad esempio uno slideshow con effetto "transition" tra le due immagini dell'uomo e della donna attraverso un javascript esterno.
Pero' una landing per performare a dovere deve essere ottimizzata al meglio e possedere alcuni requisiti: deve essere si, d'impatto, ma al tempo stesso leggera nei limiti del possibile e non aver problemi di visualizzazione sui devices. Proprio in base a questa regola ho deciso di scegliere la via piu' semplice senza correre il rischio di sovraccaricare il codice di chiamate superflue. 
Quindi la pagina e' costituita sostanzialmente da due immagini (le carte di credito ed il background), un foglio di stile e l'html.
Ho pertanto deciso di sacrificare lo script ad effetto in favore di una soluzione crossbrowsing css3 sfruttando la proprieta' "COVER" del background assegnato al body; in questo modo l’immagine sarà ridimensionata senza perdere le proporzioni originali e occuperà l’intero sfondo. L'immagine e' un'unica gif animata, certo non leggerissima ma sicuramente meglio di due immagini caricate attraverso uno script.

--CROSS BROWSER E CROSS DEVICE--

Passiamo ora all'aspetto responsive.
Anche per questa tematica vale il discorso fatto in precedenza: inutile "scomodare" un Framework (Bootrap, Alux eccetera) per una semplice Landing page con il rischio di appesantirla con codice inutile, chiamate a css e librerie javascript esterne. Ho deciso quindi di suggerire al browser il modo in cui dovra' gestire la "viewport" con la proprieta' "initial-scale" uguale a 1.0. All'interno del css ho inserito quattro @media query per la visualizzazione su Tablet e Smartphone, cambiando di volta in volta i valori di lunghezza/margin/padding alla classe che contiene la leaf verticale del Form. 

--CONCLUSIONI--

In questo modo la pagina risulta visibile su tutti i browser e su tutti i devices. L'immagine di sfondo si ridimensiona restringendo la finestra del browser mantenendo le proporzioni mentre il box del form, non potendosi allargare in orizzontale, si allunga nel senso verticale restringendosi pur mantenendo proporzioni e grandezze di font ed elementi.
L'unica scelta arbitraria, non avendo la grafica di come dovrebbe apparire la landing sui monitor di un piccolo smartphone, riguarda la decisione (del tutto personale) di mantenere l'immagine di background "sotto" il box del form in trasparenza. Ho ridotto la trasparenza in modo che il contenuto non si confonda con il background mantenendo in questo modo una sorta di continuita' con la vista Desktop.




