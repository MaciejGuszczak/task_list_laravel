# Task List Laravel

**Task List Laravel** to aplikacja webowa napisana w frameworku Laravel, umożliwiająca zarządzanie listami zadań. Projekt jest przykładem wykorzystania Laravel do stworzenia prostego CRUD dla zadań, z obsługą autoryzacji i relacji użytkownik-zadanie.

## Wymagania

- PHP >= 8.1
- Composer
- Laravel >= 10.x
- MySQL lub inna kompatybilna baza danych
- Node.js + npm (do assetów frontendowych)

## Instalacja

1. Sklonuj repozytorium:

   ```
   git clone https://github.com/MaciejGuszczak/task_list_laravel.git
   cd task_list_laravel
   ```

2. Zainstaluj zależności PHP:

   ```
   composer install
   ```

3. Skonfiguruj plik `.env` według swoich ustawień bazy danych:

   ```
   cp .env.example .env
   ```

4. Wygeneruj klucz aplikacji:

   ```
   php artisan key:generate
   ```

5. Wykonaj migracje bazy danych:

   ```
   php artisan migrate
   ```

6. (Opcjonalnie) Zainstaluj zależności frontendowe:

   ```
   npm install
   npm run dev
   ```

## Uruchomienie

Aby uruchomić lokalny serwer developerski:

```
php artisan serve
```
Aplikacja będzie dostępna pod adresem `http://localhost:8000`.

## Funkcjonalności

- Rejestracja i logowanie użytkownika
- Dodawanie, edycja, usuwanie zadań
- Lista zadań użytkownika
- Oznaczanie zadań jako ukończone
- Prosty interfejs użytkownika

## Struktura projektu

- `app/Models` — modele Eloquent
- `app/Http/Controllers` — kontrolery logiki
- `resources/views` — widoki Blade
- `routes/web.php` — trasy webowe
- `database/migrations` — migracje bazy danych

## Przykład użycia

Po rejestracji możesz dodawać własne zadania do listy, edytować je, usuwać oraz oznaczać jako ukończone.
