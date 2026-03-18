# Evidence a sprava firemniho majetku
Rozhodl jsem se vytvořit aplikaci pro přehlednou správu vybavení v rámci firmy nebo organizace. Hlavní motivací je nahradit nepřehledné tabulky v Excelu něčím, co má jasnou strukturu a logiku. Aplikace slouží k tomu, aby správce budovy nebo IT technik vždy věděl, kde se co nachází a kdo za danou věc zodpovídá.



Co aplikace umí (možnosti uživatele)
Při návrhu jsem se zaměřil na to, aby práce s daty byla co nejjednodušší:

Organizace prostoru: V systému si můžu vytvořit mapu budov a jednotlivých kanceláří (místností). Každá místnost logicky patří do konkrétní budovy.

Evidence věcí: Do místností pak přidávám konkrétní majetek. U každé věci sleduji její název, cenu a inventární číslo.

Přiřazení lidem: Aby v tom nebyl chaos, každá věc má svého konkrétního vlastníka (zaměstnance). Snadno tak zjistím, co má který kolega zrovna u sebe.

Rychlé hledání: Přidám funkci, která mi vyfiltruje všechny věci v jedné místnosti nebo ukáže seznam majetku konkrétního člověka.

Úpravy a mazání: Samozřejmostí je možnost cokoliv upravit, přemístit věc do jiné místnosti nebo ji ze systému vyřadit, pokud se odepíše.

Jak je to vymyšlené uvnitř (Technické detaily)
Aplikaci stavím na moderních technologiích v rámci .NET:

Backend: Jako základ používám C#. Pro práci s daty využívám knihovnu Entity Framework Core a databázi SQLite – je to rychlé a nevyžaduje to instalaci velkého databázového serveru.

Struktura kódu: Aby byl kód čistý, využívám polymorfismus. Například u majetku rozlišuji mezi elektronikou (která má navíc třeba záruku) a nábytkem. Také používám přetěžování metod pro různé způsoby vyhledávání.

Rozhraní: Projekt realizuji jako webovou aplikaci. Backend běží na ASP.NET Core a komunikuje přes REST API s frontendem (HTML/JavaScript). V další fázi projektu plánuji rozšíření o pokročilé grafické rozhraní.







Autor: Volodymyr Barabash (st69589)
Kontakt: st69589@upce.cz
