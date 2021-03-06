# Тип char

Тип char слугує для збереження символів, які у мові С++ можна задати з допомогою одинарних лапок. Наприклад:

```cpp
char firstLetterInAlphabet{'a'};
```

{% hint style="warning" %}
Розмір, який займає змінна типу `char` у пам'яті - завжди 1 байт.
{% endhint %}

По суті, тип `char` зберігає код символу у [таблиці ASCII](https://uk.wikipedia.org/wiki/ASCII) \(_American Standard Code for Information Interchange_\). Ця таблиця задає числовий код для кожного символу. Під час виводу текстової інформації кожен числовий код перетворюється та відповідний символ відображається на екрані. Таблиця ASCII складається з двох частин. Друга частина \(коди 128-255\) можуть різнитися в залежності від налаштувань системи. Перша ж частина \(коди 0-127\) завжди містить усі необхідні знаки, цифри, латинськи та інші спеціальні символи. Ця частина наведена нажче:

| \# | chr | \# | chr | \# | chr | \# | chr | \# | chr | \# | chr | \# | chr |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 0 | NUL | 20 | DC4 | 40 | \( | 60 | &lt; | 80 | P | 100 | d | 120 | x |
| 1 | SOH | 21 | NAK | 41 | \) | 61 | = | 81 | Q | 101 | e | 121 | y |
| 2 | STX | 22 | SYN | 42 | \* | 62 | &gt; | 82 | R | 102 | f | 122 | z |
| 3 | ETX | 23 | ETB | 43 | + | 63 | ? | 83 | S | 103 | g | 123 | { |
| 4 | EOT | 24 | CAN | 44 | , | 64 | @ | 84 | T | 104 | h | 124 | \| |
| 5 | ENQ | 25 | EM | 45 | - | 65 | A | 85 | U | 105 | i | 125 | } |
| 6 | ASK | 26 | SUB | 46 | . | 66 | B | 86 | V | 106 | j | 126 | ~ |
| 7 | BEL | 27 | ESC | 47 | / | 67 | C | 87 | W | 107 | k | 127 | DEL |
| 8 | BS | 28 | FS | 48 | 0 | 68 | D | 88 | X | 108 | l |  |  |
| 9 | TAB | 29 | GS | 49 | 1 | 69 | E | 89 | Y | 109 | m |  |  |
| 10 | LF | 30 | RS | 50 | 2 | 70 | F | 90 | Z | 110 | n |  |  |
| 11 | VT | 31 | US | 51 | 3 | 71 | G | 91 | \[ | 111 | o |  |  |
| 12 | FF | 32 | '  ' | 52 | 4 | 72 | H | 92 | \ | 112 | p |  |  |
| 13 | CR | 33 | ! | 53 | 5 | 73 | I | 93 | \] | 113 | q |  |  |
| 14 | SO | 34 | " | 54 | 6 | 74 | J | 94 | ^ | 114 | r |  |  |
| 15 | SI | 35 | \# | 55 | 7 | 75 | K | 95 | \_ | 115 | s |  |  |
| 16 | DLE | 36 | $ | 56 | 8 | 76 | L | 96 | \` | 116 | t |  |  |
| 17 | DC1 | 37 | % | 57 | 9 | 77 | M | 97 | a | 117 | u |  |  |
| 18 | DC2 | 38 | & | 58 | : | 78 | N | 98 | b | 118 | v |  |  |
| 19 | DC3 | 39 | ' | 59 | ; | 79 | O | 99 | c | 119 | w |  |  |

{% hint style="info" %}
**Деталі: керуючі символи**

Перші 32 символи у таблиці мають спеціальне значення. Їх називають **керуючими символами**. Деякі з цих керуючих символів позначаються спеціальними комбінаціями у програмах на мові С++ \(для зручності\), це так звані **escape-послідовності** \(_escape sequences_\). Наприклад, при виводі можна перевести курсор на новий рядок додавши у кінець символ `'\n'`\(LF\) на Linux або символи `'\r'`\(CR\) та `'\n'`\(LF\) на Windows. Ми ж для цієї мети використовуємо `std::endl`, який додає до рядка необхідну послідовність в залежності від ситуації. Детальніше читайте про це тут: [https://stackoverflow.com/questions/1761051/difference-between-n-and-r](https://stackoverflow.com/questions/1761051/difference-between-n-and-r)
{% endhint %}

