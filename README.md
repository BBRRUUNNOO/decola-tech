# Decola tech 2025
Java RESTful API

## Diagrama de classes

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
        +String Number
        +String Agency
        +float Balance
        +float Limit
    }

    class Feature {
        +String icon
        +String description
    }

    class Card {
        +String Number
        +float Limit
    }

    class News {
        +String Icon
        +String Description
    }

    User "1" *--"1" Account
    User "1" *--"n" Feature
    User "1" *--"1" Card
    User "1" *--"n" News
```
