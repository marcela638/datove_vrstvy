Domácí úkol na kurz Datové inženýrství

Na vytváření datových vrstev byl používán Big Query a Cloud Storage v Google Cloudu. Zdrojová data byla z Data sheetů na Google Disku

Jedná se o imaginární zakázku od společnosti nabízející předplatné na streamovací TV, filmy atd.

V pipelině jsou vytvořeny 3 datové vrstvy. 

L1 je vytvářena kvůli přetypování (castování) dat původně ve stringu na odpovídající datové typy. Na začátku je 7 tabulek.

L2 je omezen počet tabulek na základě předpokladů pro budoucí analytický report na 5 tabulek. Jsou doplněna nějaká omezení na data... s jakými kategoriemi počítat na základě požadavků zákazníka. Jsou dopočítání další sloupce. 
Business otázky:
Kteří zákazníci a kdy odcházejí?
Nakupují málo/hodně?
Existují ještě produkty, které nakupovali?

L3 Počet tabulek je omezen na 4. Tabulka contract byla zvolena jako faktická tabulka pro star schema pro budoucí report. Na tomto základě byla doplněna o některé faktické údaje z ostatních tabulek. 


![dat_inz_du drawio](https://github.com/user-attachments/assets/2a3c8924-0d36-4011-9767-be0e17c4fd36)
