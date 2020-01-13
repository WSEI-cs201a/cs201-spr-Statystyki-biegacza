### Statystyki biegacza - LINQ to Objects

> Autor: _Krzysztof Molenda_
>
> Wersja: 1.0 (2019.12.05)

Poniższy przykładowy napis `"00:45,01:32,02:18,03:01,03:44,04:31,05:19,06:01,06:47,07:35"` reprezentuje sekwencję zarejestrowanych wyników biegacza wykonującego kolejne okrążenia. Wyniki te należy interpretować jako pomiary aktualnego czasu w chwili pokonania kolejnego okrążenia, mierzonego od momentu rozpoczęcia biegu. W podanym przykładzie

* pierwsze okrążenie biegacz pokonał w 45 sekundzie,
* drugie okrążenie zaliczył po minucie i 32 sekundach od momentu rozpoczęcia biegu,
* ...

Należy przyjąć, że łączny czas biegu jest krótszy niż godzina.

Dane przedstawione są w formacie (`minuta:sekunda`), oddzielone tylko przecinkami.

Napisz program, który wczyta ze standardowego wejścia sekwencję wyników zawodnika i wypisze na standardowe wyjście - w oddzielnych wierszach - podstawowe statystyki biegu:

1. liczbę okrążeń zaliczonych przez biegacza
2. czasy kolejnych okrążeń, oddzielone spacją
3. czas i numery najszybszego okrążenia, oddzielone spacją
4. czas i numery najwolniejszego okrążenia, oddzielone spacją
5. średni czas okrążenia (średnia arytmetyczna), w zaokrągleniu w górę do pełnych sekund

Wszystkie czasy podajesz w formacie (`mm:ss`).

**Zadanie wykonaj, wykorzystując operatory LINQ.**

**Przykład:**

Wejście:

```plaintext
00:45,01:32,02:18,03:01,03:44,04:31,05:19,06:01,06:47,07:35
```

Wyjście:

```plaintext
10
00:45 00:47 00:46 00:43 00:43 00:47 00:48 00:42 00:46 00:48
00:42 8
00:48 7 10
00:46
```
