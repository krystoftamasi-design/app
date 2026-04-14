Testovací protokol: The Adaptation Experiment
TC01: Základní pád (Smrt na nečinnost)
Cíl: Ověřit funkčnost časovače a koncového stavu.

Akce: Spusť aplikaci a nic nedělej. Sleduj bílý bar "MEANING".

Očekávaný výsledek: Bar lineárně klesá. Zhruba po 50 vteřinách dojde na nulu. Vyskočí modrá obrazovka "SYSTEM FAILURE". Finální balance ukazuje $ 0.

TC02: Past luxusu (Hedonická adaptace v praxi)
Cíl: Ověřit akceleraci pádu (hlavní pointa tvé prezentace).

Akce: Spusť hru a rychle 5x klikni na "ACQUIRE (+10K)".

Očekávaný výsledek: Konto se zvýší na $ 50,000. Bar "MEANING" začne vizuálně mizet exponenciálně rychleji. Hráč zbankrotuje v řádech jednotek sekund.

TC03: Anti-Cheat (Pokus o podvod bez komunikace)
Cíl: Ověřit, že generátor ID a validace s modulo 7 funguje a hráči nemohou tipovat.

Akce: Do pole "ENTER PARTNER ID" zadej klasické sekvence z nudy: 1111, 1234, 0000, nebo 9999. Klikni CONNECT.

Očekávaný výsledek: Systém vypíše červeně INVALID ID. Rychlost pádu se neresetuje. (Algoritmus pustí jen čísla, jejichž součet cifer končí sedmičkou).

TC04: Zablokování sobectví
Cíl: Ověřit, že hráč nemůže použít vlastní kód jako záchranný kruh.

Akce: Podívej se na svoje "UNIQUE ID" a zadej ho přesně do input pole pod ním. Klikni CONNECT.

Očekávaný výsledek: Systém vypíše červeně SELF-CONNECTION BLOCKED.

TC05: Úspěšná záchrana (Konfelicita)
Cíl: Ověřit propojení dvou nezávislých hráčů.

Akce: Přečti si UNIQUE ID z Okna č. 2 (např. 3130). Zadej toto ID do pole v Okně č. 1. Klikni CONNECT.

Očekávaný výsledek: Input pole se vymaže. Modrý text oznámí CONNECTION SUCCESSFUL. Bar "MEANING" se okamžitě vrátí na 100 %. Rychlost klesání se zresetuje na původní, pomalou rychlost. Klávesnice na mobilu se sama schová.

TC06: Blokace opakování (Prevence farmení jednoho ID)
Cíl: Ověřit paměť použitých kódů.

Akce: Ihned po úspěšném dokončení testu TC05 zadej do Okna č. 1 znovu stejné ID z Okna č. 2.

Očekávaný výsledek: Systém odmítne záchranu s chybou ID ALREADY USED. Hráč je nucen začít komunikovat s někým dalším.

TC07: Systém rekordů (Local Storage)
Cíl: Ověřit, že si telefon pamatuje nejvyšší skóre i přes obnovení stránky.

Akce: 1. Klikni na ACQUIRE, abys měl $ 30,000. Nech bar spadnout na nulu.
2. Na obrazovce "SYSTEM FAILURE" se musí objevit blikající nápis NEW RECORD.
3. Klikni na "REBOOT SYSTEM" (nebo obnov stránku).
4. Na hlavní obrazovce v pravém horním rohu "MAX ASSETS" musí svítit $ 30,000.
5. Zahraj znovu, umři naschvál s $ 10,000. Rekord nahoře musí zůstat původní.