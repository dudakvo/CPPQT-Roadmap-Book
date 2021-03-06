# Вказівники: примітивна демонстрація програми у пам'яті

Давайте спробуємо продемонструвати візуально, як виглядає робота з вказівниками та пам'яттю у програмі С++. Зауважте, що візуалізація навмисно спрощена і лише дуже примітивно \(але не достовірно!\) демонструє, що насправді відбувається. 

![&#x41F;&#x440;&#x43E;&#x433;&#x440;&#x430;&#x43C;&#x430; &#x431;&#x430;&#x447;&#x438;&#x442;&#x44C; &#x43E;&#x43F;&#x435;&#x440;&#x430;&#x442;&#x438;&#x432;&#x43D;&#x443; &#x43F;&#x430;&#x43C;&apos;&#x44F;&#x442;&#x44C;, &#x44F;&#x43A; &#x432;&#x435;&#x43B;&#x435;&#x442;&#x435;&#x43D;&#x44C;&#x43A;&#x438; &#x43C;&#x430;&#x441;&#x438;&#x432; &#x43A;&#x43E;&#x43C;&#x456;&#x440;&#x43E;&#x43A;.](../../.gitbook/assets/memdemo_1.png)

Звичайно, як насправді організована пам'ять на різних рівнях архітектури комп'ютера - то окрема складна тема. Але, з точки зору програміста, який доступається до пам'яті з програми на мові С++ - все виглядає саме так. На малюнку вище, ми розглянемо уявну область пам'яті. Кожна з комірок може містити значення \(за замовчуванням, у комірці містяться випадкові дані, що позначено `???`\). Кожна така комірка має унікальну адресу у пам'яті \(у прикладі ми маємо адреси з `0x00` до `0x1F`\).

![&#x41F;&#x456;&#x434; &#x447;&#x430;&#x441; &#x437;&#x430;&#x43F;&#x443;&#x441;&#x43A;&#x443; &#x43F;&#x440;&#x43E;&#x433;&#x440;&#x430;&#x43C;&#x438;, ](../../.gitbook/assets/memdemo_2.png)

![](../../.gitbook/assets/memdemo_3.png)

![](../../.gitbook/assets/memdemo_4.png)

![](../../.gitbook/assets/memdemo_5.png)

![](../../.gitbook/assets/memdemo_6.png)

![](../../.gitbook/assets/memdemo_7.png)

![](../../.gitbook/assets/memdemo_8.png)

![](../../.gitbook/assets/memdemo_9.png)

![](../../.gitbook/assets/memdemo_9.png)

![](../../.gitbook/assets/memdemo_10.png)

![](../../.gitbook/assets/memdemo_11.png)

![](../../.gitbook/assets/memdemo_12.png)

