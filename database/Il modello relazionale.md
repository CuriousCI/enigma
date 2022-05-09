# Il modello relazionale
%% Tutta robba prima%%

## Normalizzazione di un database
La **normalizzazione** serve ad eliminare la *ridondanza dei dati*, e ne esistono vari livelli *(forme normali)*:
- prima forma normale *($1^{st}$ Normal Form: 1NF)*
- seconda forma normale *($2^{nd}$ Normal Form: 2NF)
- terza forma normale *($3^{rd}$ Normal Form: 3NF)

Il processo di **normalizzazione** si basa sull'idea che se una **relazione** contiene più concetti fra loro indipendenti, la si decompone in relazioni più piccole, in modo che:
- Non si perdano informazioni.
- Si conservino le **dipendenze** *(i vincoli di integrità)*.

La **decomposizione senza perdita** consiste nel concetto per cui, se suddivido una tabella $T$ in due tabelle $T_1$ e $T_2$, bisogna conservare le **dipendenze** tra i dati, e la condizione $T = T_1\;join\;T_2$.

Le varie forme normali **forme normali** si possono descrivere nella seguente maniera:
- **Prima forma normale (1NF)**: una tabella è in **1NF** se tutti gli attributi hanno **domini atomici** *(non si possono ulteriormente scomporre)*, ed esiste una **chiave primaria**.
- **Seconda forma normale (2NF)**: una tabella è in **2NF** se è in **1NF** ed esistono solo dipendenze *funzionali* complete fra gli attributi: ogni **attributo** **dipende** dalla **chiave primaria (o composta)**.
- **Terza forma normale (3NF)**: una tabella è in **3NF** quando è in **2NF** e tutti gli attributi **non chiave** dipendono dalla **chiave** soltanto.

Le **4NF**, **5NF** e **6NF** vengono raramente utilizzate, perchè portano ad un'inefficienza delle modifiche al database. 

%%https://en.wikipedia.org/wiki/Database_normalization %%