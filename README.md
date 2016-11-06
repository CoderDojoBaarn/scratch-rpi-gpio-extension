# Scratch Raspberry PI GPIO extensie
Met deze plugin kun je heel eenvoudig alle gpio pinnen van de Raspberry PI aansturen.

## Installatie
Je kunt deze plugin installeren door in de offline Scratch editor de `shift` toets ingedrukt te houden en dan te klikken op `bestand`. Dan krijg je helemaal onderin de optie `Importeer experimentele HTTP-uitbreiding`. Zoek dan het bestandje `rpio-gpio.json` op en klik op OK.

Naast de plugin heb je op zijn minst het helper programma nodig die met de plugin praat. Mocht je de offline Scratch editor niet hebben draaien op een PI dan kun je ipv het helper programma het proxy programma draaien.

## Voorbeeld setup
Raspberry PI met ip 192.168.0.10 draait het programma rpio-gpio-helper:
```
python rpio-gpio-helper
```

Laptop met ip 192.168.0.48 heeft de offline Scratch editor met de extensie geladen en draait het programma rpio-gpio-proxy:
```
python rpio-gpio-proxy http://192.168.0.10:5000
```

Nu kun je vanuit Scratch alle gpio pinnen aansturen.
