# Zabbix z PostgreSQL przy użyciu Docker Compose

To repozytorium zawiera konfigurację Docker Compose do uruchomienia serwera Zabbix z bazą danych PostgreSQL oraz agentem Zabbix.

## Usługi

Plik Docker Compose definiuje następujące usługi:

- **postgres**: Baza danych PostgreSQL do przechowywania danych Zabbixa.
- **zabbix-server**: Serwer Zabbix, który komunikuje się z bazą danych PostgreSQL.
- **zabbix-web**: Interfejs webowy Zabbixa, używający Nginx i PHP.
- **zabbix-agent**: Agent Zabbix do monitorowania hosta.

## Wymagania

- Docker
- Docker Compose

## Instalacja

1. Sklonuj to repozytorium:

    ```sh
    git clone https://github.com/yourusername/zabbix-docker-compose.git
    cd zabbix-docker-compose
    ```

2. Utwórz i uruchom kontenery:

    ```sh
    docker-compose up -d
    ```

3. Uzyskaj dostęp do interfejsu webowego Zabbix pod adresem [http://localhost:8080](http://localhost:8080).

4. Zaloguj się, używając domyślnych danych logowania:
    - **Użytkownik**: `Admin`
    - **Hasło**: `zabbix`
