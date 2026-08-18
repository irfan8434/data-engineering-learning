# Conceptual Data Model

```mermaid
flowchart LR

    A["Source Systems<br/>DBMS / RDBMS"]
    B["Staging / Landing Pad<br/>Raw Files"]
    C["DSA<br/>Data loaded into tables"]
    D["ODS<br/>Cleansing and Standardisation"]
    E["Enterprise Data Warehouse<br/>Facts / Dimensions / Business Logic"]
    F["Data Marts<br/>HR / Finance / Sales"]
    G["Reports / Analytics / KPIs"]

    A --> B
    B --> C
    C --> D
    D --> E
    E --> F
    F --> G
