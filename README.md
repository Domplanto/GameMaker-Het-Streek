Hier is een voorbeeld van een README die uitlegt hoe je jouw GameMaker-game aan deze website kunt toevoegen:

---

# Het Streek Games - Game Toevoegen

Welkom bij de repository voor **Het Streek Games**. Met deze website kunnen studenten hun eigen GameMaker-games uploaden en delen met anderen.

Volg de stappen hieronder om jouw GameMaker-game aan de website toe te voegen.

## Inhoudsopgave
1. [Voorbereidingen](#voorbereidingen)
2. [Game-bestanden uploaden](#game-bestanden-uploaden)
3. [Game-kaart toevoegen aan de website](#game-kaart-toevoegen-aan-de-website)
4. [Testen](#testen)

---

### Voorbereidingen
- Zorg ervoor dat je game gereed is voor export naar HTML5. Dit kun je doen in GameMaker door je project te exporteren naar HTML5.

### Game-bestanden uploaden
1. Exporteer je GameMaker-game als HTML5. Dit genereert een map met alle bestanden die nodig zijn om je game in de browser te draaien.
2. Voeg deze map toe aan de `GameMaker-Het-Streek` directory in de website repository. De naam van de map moet de naam van je game bevatten, zonder spaties of speciale tekens (bijv. `MijnGame`).

### Game-kaart toevoegen aan de website
1. Open het `index.html` bestand van de website.
2. Zoek naar het gedeelte met de `game-grid`. Daar zie je een HTML-structuur met verschillende `<div class="game-card">` elementen voor elke game.
3. Kopieer een bestaand `game-card` element en plak het onderaan, binnen de `game-grid` sectie.
4. Pas de details van jouw game-kaart aan:
   - **data-game-url**: Vervang `/GameMaker-Het-Streek/(De naam van de map van je game)` met de naam van je game-map.
   - **img src**: Voeg een afbeelding toe in de map van je game (bijv. `logo.jpg` van 400x200 px) en pas de src aan naar jouw game-map.
   - **alt**: Voeg een beschrijving toe voor de logo-afbeelding van je game.
   - **h2**: Vul de titel van je game in.
   - **p**: Geef een korte beschrijving van je game.

Voorbeeld van een nieuwe game-kaart:

```html
<div class="game-card" data-game-url="/GameMaker-Het-Streek/MijnGame">
  <img src="/GameMaker-Het-Streek/MijnGame/logo.jpg" alt="Mijn Game Logo">
  <div class="content">
    <h2>Mijn Game</h2>
    <p>Een spannende game over het verkennen van virtuele werelden!</p>
  </div>
</div>
```

### Testen
1. Open de website in je browser door het `index.html` bestand te openen of te hosten via een lokale server.
2. Controleer of jouw game-kaart correct wordt weergegeven in het `Games` gedeelte.
3. Klik op je game-kaart om te testen of de game in de iframe wordt geladen.

---

Je game zou nu zichtbaar moeten zijn op de website!
