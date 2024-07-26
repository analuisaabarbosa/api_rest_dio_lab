# Lab DIO publicando uma API REST na Nuvem Usando Spring Boot, Java e Railway
RESTful API criada para o Bootcamp Java Back-end Santander

# Diagrama das Classes 

```mermaid
classDiagram
    class User {
        +String name
        +Account account
        +Feature[] features
        +Card card
        +News[] news
    }

    class Account {
        +String number
        +String agency
        +Float balance
        +Float limit
    }

    class Feature {
        +String icon
        +String description
    }

    class Card {
        +String number
        +Float limit
    }

    class News {
        +String icon
        +String description
    }

    User "1" *-- "1" Account : has
    User "1" *-- "1" Card : has
    User "1" *-- "0..*" Feature : has
    User "1" *-- "0..*" News : has
```mermaid
