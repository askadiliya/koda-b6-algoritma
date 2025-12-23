


```mermaid
flowchart TD
    A@{ shape: circle, label: "Start" }
    B@{ shape: lean-r, label: "Angka" }
    C@{ shape: diamond, label: "Angka % 2 = 0" }
    D@{ shape: lean-r, label: "Bilangan Ganjil" }
    E@{ shape: lean-r, label: "Bilangan Genap" }
    F@{ shape: dbl-circ, label: "Stop" }

    A --> B --->C
    C --True--> E
    C --False--> D
    E-->F
    D-->F

    
```