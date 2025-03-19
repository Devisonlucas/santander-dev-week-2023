# santander Dev Week 2023
Java RESTful API criada para a Santander Dev Week.

## Diagrama de Classes 

```mermaid
classDiagram
    class User {
        +string name
        +Account account
        +Feature[] features
        +Card card
        +News[] news
    }
    
    class Account {
        +string number
        +string agency
        +float balance
        +float limit
    }
    
    class Feature {
        +string icon
        +string description
    }
    
    class Card {
        +string number
        +float limit
    }
    
    class News {
        +string icon
        +string description
    }
    
    User "1" *-- "1" Account
    User "1" *-- "n" Feature
    User "1" *-- "1" Card
    User "1" *-- "n" News
```
