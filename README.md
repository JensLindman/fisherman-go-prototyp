# Fisherman Go – webbprototyp

Spelbar prototyp av hela loopen: karta → skugga i vattnet → kast → napp → drill → fångst i 3D → fiskedex.

Öppna sidan i mobilen och tryck på **Kompass** för att slå på sensorerna:

- **Kompass:** kartan vrids så att hållet du tittar åt är uppåt.
- **GPS:** du går på kartan när du går i verkligheten (sjön placeras där du startar).
- **Sving:** i kastvyn siktar du genom att vrida dig och kastar med en snabb sving framåt. Svep uppåt fungerar också.

Sensorerna kräver https, vilket GitHub Pages ger. På iPhone frågar Safari om tillstånd första gången.

Filer: `index.html` är hela spelet, `fish/*.txt` är 3D-fiskarna (GLB som base64).
