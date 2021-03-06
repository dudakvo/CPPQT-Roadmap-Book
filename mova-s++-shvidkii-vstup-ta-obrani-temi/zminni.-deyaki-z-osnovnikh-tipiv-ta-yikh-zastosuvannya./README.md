# Змінні. Деякі з основних типів та їх застосування.

## Змінні

Для того, щоб зберігати у програмі будь-яку інформацію, нам необхідно оголосити **змінну \(**_**variable**_**\)**, яка буде містити ці дані. 

Оголошення змінної складається з назви **типу** даних \(_data type_\), які будуть зберігатися у змінній та **імені змінної** \(_variable name_\), через яке ми зможемо доступатися до даних. Наприклад:

```cpp
int backyardTreeCount;
double milesToRun;
char currentLetterInVocabulary;
```

Змінній, ми можемо **присвоїти \(**_**assign**_**\) значення \(**_**value**_**\)** використавши **оператор присвоєння** `=` **\(**_**assigment operator**_**\)**. Наприклад:

```cpp
backyardTreeCount = 3;
```

Ми можемо **оголошувати змінні і одразу ж присвоювати їм значення з допомогою фігурних дужок**, як у випадку з `numberOfBenchesOnBackyard`. 

```cpp
int numberOfBenchesOnBackyard{2};
```

Врешті решт, ми можемо доступитися до значення змінної через її ім'я. Наприклад, вивести у консоль її значення:

```cpp
std::cout << "My backyard:" << std::endl;
std::cout << "    number of trees: " << backyardTreeCount << std::endl;
std::cout << "    number of benches: " << numberOfBenchesOnBackyard << std::endl;
```

**Змінна отримує тип при оголошенні і цей тип не може змінитися**. Тобто до кінця використання цієї змінної вона буде зберігати значення виключно лише цього типу.

Так, загалом ми також можемо присвоювати одній змінній значення іншої змінної за умови, що **типи співпадають або можуть бути відповідним чином перетворені**.  

## Деякі важливі типи

Нижче приведена таблиця \(для зручності\) з кількома типами, корисними для того, щоб почати писати прості програми мовою С++. Далі ідуть кілька парагафів з більш детальними прикладами та особливостями використання цих типів. Автор рекомендує, ознайомитися з типами та наведеними нижче відомостями про них та використовувати їх. Найкращим підходом буде - написати кілька маленьких програм та поексперементувати з ними, а потім - повертатися до цього розділу час від часу. Надалі у прикладах та завданнях ви зможете ці типи повноціно опанувати.

| Тип | Опис | Приклад | Бібліотека |
| :--- | :--- | :--- | :--- |
| `int` | Цілі позитивні та від'ємні числа. | `int backyardTreeCount {3};` | Вбудований тип. Не потребує підключення додаткових бібіліотек. |
| `double` | Числа з плаваючою комою. | `double milesToRun {2.1};` | Вбудований тип. Не потребує підключення додаткових бібіліотек. |
| `bool` | Логічний тип. Може містити значення `true` \(істина\) або `false` \(брехня\) | `bool pllugIsCool {true};` | Вбудований тип. Не потребує підключення додаткових бібіліотек. |
| `char` | Символ | `char firstLetter = 'a';` | Вбудований тип. Не потребує підключення додаткових бібіліотек. |
| `void` | Позначає відсутність типу. Використовується при оголошенні функцій. Змінну цього типу створити неможливо. | `void function() {}` | Вбудований тип. Не потребує підключення додаткових бібіліотек. |
| `std::string` | Текстовий рядок. | `std::string message{"Hello!"};` | `#include <string>` |
| `std::vector<тип>` | Список елементів заданого типу. Тип задають всередині гострих дужок. Список може змінювати розмір, елементи можна додавати та видаляти зі списку. | `std::vector<std::string> friendList {"Harry", "Ron", "Hermiona"};` | `#include <vector>` |
| `std::array<тип, розмір>` | Масив\(список фіксованого розміру\). Розмір масиву змінювати не можна. | `std::array<bool, 3> semaphorLightPowered {false, false, true};` | `#include <array>` |

