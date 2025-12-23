# Algoritma program konversi suhu

## Algoritma Deskriptif
1. Mulai
2. Masukan Celcius
3. Hitung konversi Celcius ke Fahrenheit 9/5 dikalikan dengan celcius ditambah 32
4. Hitung Konversi Celcius ke reamur 4/5 dikalikan dengan nilai Celcius
5. Hitung Konversi Celcius ke kelvin nilai celcius ditambah 273
6. Selesai

## Flowchart

```mermaid
flowchart TD
A@{ shape: circle, label: "Start" }
B@{ shape: lean-r, label: "Input:Celcius" }
C@{ shape: diamond, label: "Celcius % 5 == 0" }
D@{ shape: rect, label: "F = (9/5)*C+32
R=(4/5)*C" }
E@{ shape: rect, label: "k= c+273" }
F@{ shape: rect, label: "k= c+273" }
G@{ shape: lean-r, label: 'Output: "K" '}
L@{ shape: rect, label: "F = (9/5)*C+32" }
M@{ shape: lean-r, label: 'Output: "F" '}
N@{ shape: rect, label: "R=(4/5)*C" }
O@{ shape: lean-r, label: 'Output: "R" '}
P@{ shape: dbl-circ, label: "Stop" }



A--->B-->C
C--True-->D
C--False-->E
D-->F
E-->F-->G-->L-->M-->N-->O-->P

```