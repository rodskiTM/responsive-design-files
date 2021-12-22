1. Bekijken zonder en met display: flex;
2. Centreren (in .child)
   a. Bekijken zonder
   margin: auto;
   -> dus dit centreert de box binnen de flex-container.
   b. Andere manier (flex-manier).  
    Bekijk ook eens zonder (in .child)
   width: 60%;
   height: 100px;
   Voeg toe (in .parent)
   justify-content: center; (aligneren langs de hoofdas)
   align-items: center; (aligneren langs de dwarsas)
   Zelfde als margin: auto; Maar nu is alles 'flex'-geïnitialiseerd.
3. Verander
   a. justify-content: start;
   b. flex-flow : row-reverse nowrap; (was row).
   c. justify-content: flex-start;
   -> Er is geen verschil tussen 'start' en 'flex-start' als er 1 flex-item is
4. Verander
   flex-flow : column nowrap; (was row-reverse).
   En zorg ervoor dat :
   justify-content: center; (aligneren langs de hoofdas)
   align-items: center; (aligneren langs de dwarsas)
   -> Hoofdas wordt nu verticaal gelegd (weinig effect want slechts 1 element)
   Verander (in .parent) :
   align-items: start; (Waarom verplaatst de blok zich naar links en niet naar boven?)
   -> HORIZONTALE centrering, wordt vervangen door een '(flex)start'. De dwarsas ligt nu horizontaal.
5. Verwijder uit .child
   height: 100px;
   width: 60%;
   => eventuele bijkomende inhoud vergroot de box (dus reageert als 'auto')
   => Zal in het ergste geval 'uit' zijn container vloeien
