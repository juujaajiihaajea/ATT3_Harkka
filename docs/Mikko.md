# Lämpötilaseuranta

## Kenelle ja miksi
- **Kenelle:** Automaatiolaboratorion opiskelijoille ja opettajille.
- **Ongelma:** Lämpötiladatan manuaalinen kirjaaminen mittauspisteiltä vie liikaa aikaa.
- **Hyöty:** Ohjelmisto lukee anturidatan automaattisesti, jolloin poikkeamat huomataan heti.

## Testikoodi
```python
def tarkista_lampotila(temp):
    if temp > 75.0:
        return "HÄLYTYS: Liian kuuma!"
    return "Normaali"

# Testiajo
print(tarkista_lampotila(80.5))
