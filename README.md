# Moonbase Control: Control Flow

Zadanie z modułu Angular. Repozytorium zawiera kod startowy aplikacji Moonbase Control dla tej lekcji.

## Zadanie

#### Zrefaktoryzuj dashboard, wykorzystując nowoczesny Control Flow Angulara.

### 1. Zmień model danych
Połącz wszystkie karty w jedną tablicę według przykładu:

```
statusCards: StatusCard[] = [
  {
    id: 'total-missions',
    title: 'Total Missions',
    value: 8,
  },
  ...
];
```

### 2. Wygeneruj karty za pomocą `@for`
- Usuń ręcznie dodane instancje komponentu `Card`.
- Wykorzystaj `@for`, aby wygenerować wszystkie karty na podstawie tablicy.
- 💡 Dodanie nowej karty powinno wymagać jedynie dopisania kolejnego elementu do tablicy.

### 3. Dodaj `track`
Podczas iteracji wykorzystaj właściwość `id` jako identyfikator elementu.

💡 `track` pomaga Angularowi efektywnie aktualizować widok.

### 4. Wyświetlaj wybraną kartę warunkowo
- Obecnie informacja `Card selected: ...` jest widoczna przez cały czas.
- Wyświetlaj ją tylko wtedy, gdy użytkownik wybierze kartę.
- Wykorzystaj `@if`.

### 5. Dodaj blok `@else`
- Jeżeli żadna karta nie została wybrana, wyświetl komunikat: "Select a card to see available actions."
- Po wybraniu karty wyświetl informację o wybranej karcie.
- 💡 Dzięki `@else` użytkownik zawsze otrzymuje informację o aktualnym stanie aplikacji.

## Jak zacząć

1. Zrób fork tego repozytorium na swoje konto GitHub.
2. Sklonuj swój fork na komputer.
3. Zainstaluj zależności: `npm install`.
4. Uruchom aplikację: `npm start`.
5. Jeśli zadanie korzysta z danych z API, uruchom w drugim terminalu mock API: `npm run api`.

## Jak oddać zadanie

1. Zapisz zmiany w commicie i wypchnij je do swojego forka.
2. Otwórz Pull Request z forka do repozytorium `mate-academy/angular_control-flow`, do brancha `main`.
3. Platforma uruchomi review Twojego Pull Requesta.
