# Fisherman Go – webbprototyp

Spelbar prototyp av hela loopen: karta → skugga i vattnet → kast → napp → drill → fångst i 3D → fiskedex.

## Riktig karta

Kartan är OpenStreetMap-data från [OpenFreeMap](https://openfreemap.org) (ingen API-nyckel), ritad med MapLibre. Spelet läser vattnet direkt ur kartans vektordata:

- **Sjöar och dammar:** abborre, gädda, gös.
- **Älvar, åar och kanaler:** abborre, gädda, gös, lax.
- **Bäckar:** abborre, lax.
- **Hav:** torsk, lax, fenknot, marulk, abborre, gädda och en mycket sällsynt vithaj.

Fiskarna dyker bara upp inom kastavstånd från en strand, så att man alltid kan nå dem från land. Vattnets namn visas på fångsten.

Tryck på **Starta GPS och kompass**:

- **GPS:** du står där du står i verkligheten och går genom att gå.
- **Kompass:** kartan vrids så att hållet du tittar åt är uppåt.
- **Sving:** i kastvyn siktar du genom att vrida dig och kastar med en snabb sving framåt. Svep uppåt fungerar också.

Utan GPS startar du vid Riddarholmen i Stockholm och går genom att trycka på kartan. Du kan välja en annan startplats med `?lat=59.33&lon=18.07`, och `?demo` öppnar demosjön direkt. Om kartan inte kan laddas byter spelet till demosjön av sig självt.

Sensorerna kräver https, vilket GitHub Pages ger. På iPhone frågar Safari om tillstånd första gången.

Filer: `index.html` är hela spelet, `fish/*.txt` är 3D-fiskarna (GLB som base64) och `dex/*.png` är porträtten i fiskedexen.

Kartdata © OpenStreetMap-bidragsgivare, © OpenMapTiles, OpenFreeMap.
