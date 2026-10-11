# Príprava notebooku na firemný kontext

Jeden príkaz pripraví tvoj notebook: nainštaluje, čo chýba, prihlási ťa do GitHubu, stiahne repozitár tvojej oblasti a otvorí ho vo VS Code. Trvá to 10–20 minút, väčšinu času sa len sťahuje. Príkaz môžeš kedykoľvek spustiť znova — čo už je hotové, preskočí.

## Skôr než začneš (10 minút)

1. **Pozvánka z GitHubu.** V pracovnom e-maile nájdi správu od GitHubu „… invited you to join …“ (pozri aj v spame). Klikni na **Join**, vytvor si účet s **pracovným e-mailom** a nastav **dvojstupňové overenie** (aplikácia v mobile, napríklad Google Authenticator alebo Microsoft Authenticator). Bez neho pozvánku neprijmeš. Záložné kódy, ktoré GitHub ukáže, si ulož.
2. **Pozvánka do Claude.** V e-maile od Anthropic prijmi pozvánku a prihlás sa pracovným e-mailom.
3. **Heslo k notebooku** maj po ruke — inštalácia si ho môže vypýtať.

## Mac

Otvor aplikáciu **Terminal** (Cmd + medzerník, napíš *Terminal*, Enter). Skopíruj celý riadok, vlož ho do Terminalu (Cmd + V) a stlač Enter:

```bash
bash -c "$(curl -fsSL https://raw.githubusercontent.com/TAKTIK-GROUP/kontext-start/main/priprav.sh)"
```

## Windows

Otvor **PowerShell** (tlačidlo Štart, napíš *PowerShell*, Enter — nie „ako správca“). Skopíruj celý riadok, vlož ho (pravé tlačidlo myši alebo Ctrl + V) a stlač Enter:

```powershell
irm https://raw.githubusercontent.com/TAKTIK-GROUP/kontext-start/main/priprav.ps1 | iex
```

Keď sa Windows opýta, či povoliť zmeny v zariadení, klikni **Áno**.

## Čo sa bude diať

1. Nainštaluje sa Git, Node.js, GitHub CLI a VS Code (čo už máš, preskočí).
2. **Prihlásenie do GitHubu:** zobrazí sa kód, napríklad `ABCD-1234`. Stlač Enter, v prehliadači sa prihlás, vlož kód a klikni **Authorize**. Ak sa niečo opýta, stlač Enter.
3. Stiahne sa repozitár tvojej oblasti do priečinka **Kontext** vo tvojom domovskom priečinku a otvorí sa vo VS Code.

## Posledné kroky vo VS Code

1. Ak sa VS Code pýta, či dôveruješ autorom priečinka, klikni **Yes, I trust the authors**.
2. Otvor panel **Claude** (ikona Claude vpravo hore alebo na boku) a prihlás sa firemným účtom.
3. Keď sa Claude pýta, či dôveruješ tomuto priečinku, potvrď **Yes**.
4. Napíš **„ahoj“**. Asistent ti odpovie prehľadom tvojej oblasti.
5. Pošli správcovi riadok **`PRIPRAVA: OK …`**, ktorý ti príkaz vypísal na konci.

## Keď niečo nejde

Príkaz skončí riadkom **`PRIPRAVA: CHYBA …`** a krátkym vysvetlením. Pošli tento riadok správcovi (pokojne aj s fotkou obrazovky) — podľa neho vie, kde je problém. Nič nemaž a nič nepresúvaj ručne.
