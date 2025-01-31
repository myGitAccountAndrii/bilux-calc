---
share: "true"
layout: default
title: Внутрішні теплонадходження
parent: Методика розрахунку
nav_order: "3"
---


# Внутрішні теплонадходження

Внутрішні теплонадходження, теплонадходження від внутрішніх теплових джерел, від'ємні теплонадходження (розсіяна теплота від внутрішнього середовища до холодних джерел або «стоки»), формують з будь-якої теплоти, що утворюється в кондиціонованому об'ємі внутрішніми джерелами, крім тієї, що навмисно використовують для опалення, охолодження або ГВП (гаряче водопостачання).

ДСТУ 9190[^1] враховує такі теплонадходження:

- внутрішній тепловий потік від людей $\Phi_{int,Oc}$;
- внутрішній тепловий потік від освітлення $\Phi_{int,L}$;
- внутрішній тепловий потік від обладнання $\Phi_{int,A}$.

## 1 Теплонадходження від внутрішніх теплових джерел

Теплонадходження від внутрішніх теплових джерел у будівлі, $Q_{int}$, Вт·год, розраховують для кожного місяця за формулою:

$$Q_{int}=\frac{N}{168}\left(\sum \Phi_{int,mn}A_{f}\right)t,\tag{1}$$

де $N$ — графік використання, залежно від призначення будівлі, може бути прийнятий згідно з таблицею [1.1](internal.md#11-теплонадходження-від-людей-освітлення-та-обладнання-значення-за-замовчуванням), год/тиждень;  
$\Phi_{int,mn}$ — усереднена за часом щільність теплового потоку від внутрішніх джерел, залежно від призначення будівлі, що може бути прийнята згідно з таблицею [1.1](internal.md#11-теплонадходження-від-людей-освітлення-та-обладнання-значення-за-замовчуванням) як сума метаболічної теплоти, освітлення та обладнання, Вт/м²;  
$A_f$ — кондиціонована площа будівлі, м²;  
$t$ — тривалість місяця, для якого проводять розрахунок, год, визначена згідно з [таблицею 2 розділу теплопередача трансміссією](./transmission.md#2-щомісячна-тривалість-часових-інтервалів).

{: .note }
> Даний розрахунок, для спрощення, не враховує період невикористання будівлі, що залежить від її функційного призначення. Тобто тут і далі вважається що будівля експлуатується 365 днів на рік.

{: .note }
> Кондиціонована площа будівлі — сумарна площа поверхів (враховуючи, зокрема, мансардний, опалюваний цокольний і підвальний поверхи) будівлі, яку вимірюють у межах внутрішніх поверхонь зовнішніх стін, з урахуванням площі, що займають горизонтальні проекції внутрішніх стін і перегородок.

### 1.1 Теплонадходження від людей, освітлення та обладнання, значення за замовчуванням

<table>
<thead>
  <tr>
    <th rowspan="2">Призначення будівлі</th>
    <th rowspan="2">Графік використання, $N$, год/тиждень</th>
    <th colspan="3">Щільність теплового потоку, Вт/м², від</th>
  </tr>
  <tr>
    <th>метаболічної теплоти, $\Phi_{int,Oc}$</th>
    <th>освітлення, $\Phi_L$</th>
    <th>обладнання, $\Phi_A$</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Одноквартирні будинки</td>
    <td style="text-align: center;">112</td>
    <td style="text-align: center;">1,2</td>
    <td style="text-align: center;">2,0</td>
    <td style="text-align: center;">2,0</td>
  </tr>
  <tr>
    <td>Багатоквартирні будинки, гуртожитки</td>
    <td style="text-align: center;">112</td>
    <td style="text-align: center;">1,8</td>
    <td style="text-align: center;">2,0</td>
    <td style="text-align: center;">2,0</td>
  </tr>
  <tr>
    <td>Громадські будівлі адміністративного призначення, офіси</td>
    <td style="text-align: center;">50</td>
    <td style="text-align: center;">4,0</td>
    <td style="text-align: center;">7,0</td>
    <td style="text-align: center;">6,0</td>
  </tr>
  <tr>
    <td>Будівлі навчальних закладів</td>
    <td style="text-align: center;">50</td>
    <td style="text-align: center;">7,0</td>
    <td style="text-align: center;">7,0</td>
    <td style="text-align: center;">6,0</td>
  </tr>
  <tr>
    <td>Будівлі дитячих навчальних закладів</td>
    <td style="text-align: center;">50</td>
    <td style="text-align: center;">7,0</td>
    <td style="text-align: center;">7,0</td>
    <td style="text-align: center;">3,0</td>
  </tr>
  <tr>
    <td>Будівлі закладів охорони здоровʼя</td>
    <td style="text-align: center;">168</td>
    <td style="text-align: center;">2,7</td>
    <td style="text-align: center;">7,0</td>
    <td style="text-align: center;">6,0</td>
  </tr>
  <tr>
    <td>Готелі</td>
    <td style="text-align: center;">168</td>
    <td style="text-align: center;">4,0</td>
    <td style="text-align: center;">8,0</td>
    <td style="text-align: center;">2,0</td>
  </tr>
  <tr>
    <td>Ресторани</td>
    <td style="text-align: center;">84</td>
    <td style="text-align: center;">5,0</td>
    <td style="text-align: center;">8,0</td>
    <td style="text-align: center;">4,0</td>
  </tr>
  <tr>
    <td>Спортивні заклади</td>
    <td style="text-align: center;">84</td>
    <td style="text-align: center;">5,0</td>
    <td style="text-align: center;">8,0</td>
    <td style="text-align: center;">1,0</td>
  </tr>
  <tr>
    <td>Будівлі закладів гуртової та роздрібної торгівлі</td>
    <td style="text-align: center;">84</td>
    <td style="text-align: center;">7,0</td>
    <td style="text-align: center;">12,0</td>
    <td style="text-align: center;">2,0</td>
  </tr>
  <tr>
    <td>Будівлі культурно-розважальних закладів та дозвільних установ</td>
    <td style="text-align: center;">56</td>
    <td style="text-align: center;">5,0</td>
    <td style="text-align: center;">8,0</td>
    <td style="text-align: center;">2,0</td>
  </tr>
  <tr>
    <td>Інші види будівель</td>
    <td style="text-align: center;">60</td>
    <td style="text-align: center;">3,0</td>
    <td style="text-align: center;">7,0</td>
    <td style="text-align: center;">2,0</td>
  </tr>
</tbody>
</table>

[^1]: [ДСТУ 9190:2022 Енергетична ефективність будівель. Метод розрахунку енергоспоживання під час опалення, охолодження, вентиляції, освітлення та гарячого водопостачання](https://online.budstandart.com/ua/catalog/doc-page.html?id_doc=98995)
