# Meteo Città - Spring Boot + Docker + Thymeleaf

Applicazione web realizzata con **Spring Boot** che mostra le temperature orarie della giornata odierna per alcune città italiane, utilizzando l’API gratuita di [Open-Meteo](https://open-meteo.com/).

Il frontend è sviluppato con **Thymeleaf** e integra un **grafico interattivo** per visualizzare le temperature. Il backend utilizza Spring Boot per effettuare chiamate HTTP all'API meteo. L’intero progetto è containerizzato con Docker e supporta l’avvio tramite `docker-compose`.

---

## Funzionalità principali

- Menu a tendina per scegliere una città italiana
- Recupero automatico dei dati meteo orari tramite API REST
- Visualizzazione in tempo reale delle **temperature nelle 24 ore**
- Grafico dinamico realizzato con **Chart.js**
- Frontend HTML + Thymeleaf
- Progetto completamente eseguibile via Docker o Docker Compose

---

## Stack tecnologico

- Java 17
- Spring Boot 3
- Thymeleaf
- RestTemplate
- Chart.js
- Docker
- Docker Compose

---

## Città supportate

- Rome  
- Milan  
- Naples  
- Turin  
- Florence  

Coordinate geografiche predefinite nella classe `CityCoordinates.java`.

---

## Come eseguire il progetto

### Opzione 1: Avvio manuale con Maven

```bash
git clone https://github.com/FabioBl77/meteo-springboot.git
cd meteo-springboot

# Costruzione del progetto
./mvnw clean package -DskipTests

# Esecuzione
java -jar target/*.jar
