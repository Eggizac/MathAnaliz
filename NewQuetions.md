# Метод замены переменной в неопределенном интеграле. (2 вопрос)
## Теория из лекции
![1](![/images/2%20вопрос%20(1).png](https://github.com/Eggizac/MathAnaliz/blob/main/images/2%20%D0%B2%D0%BE%D0%BF%D1%80%D0%BE%D1%81%20(1).png?raw=true))
![2](![/images/2%20вопрос%20(2).png](https://github.com/Eggizac/MathAnaliz/blob/main/images/2%20%D0%B2%D0%BE%D0%BF%D1%80%D0%BE%D1%81%20(2).png?raw=true))
## Примеры из демидовича на заменну переменной
![3](https://github.com/Eggizac/MathAnaliz/blob/main/images/2%20%D0%B2%D0%BE%D0%BF%D1%80%D0%BE%D1%81%20(%D0%B2%D0%BD%D0%B5%D1%81%D0%B5%D0%BD%D0%B8%D0%B5%20%D0%BF%D0%BE%D0%B4%20%D0%B7%D0%BD%D0%B0%D0%BA%20%D0%B4%D0%B8%D1%84%D1%84%20%D0%BF%D1%80%D0%B8%D0%BC%D0%B5%D1%80).jpg?raw=true)
## Метод внесения множителя под знак дифференциала
<em>Пусть про него не спрашивают в вопросе, но не зря же он находится в одном параграфе с методом замены переменной, поэтому можно его тоже рассмотреть.</em>

**Если говорить простым языком, то суть этого метода заключается в том, чтобы преобразовать подынтегральное выражение таким образом, чтобы какой-то его кусок являлся производной такой функции, при внесении которой под знак интеграла подынтегральное выражение станет табличным интегралом.**

## Примеры внесения множителя под знак дифференциала

![1](https://github.com/Eggizac/MathAnaliz/blob/main/images/2%20%D0%B2%D0%BE%D0%BF%D1%80%D0%BE%D1%81%20(%D0%BF%D1%80%D0%B8%D0%BC%D0%B5%D1%80%D1%8B%20%D0%B7%D0%B0%D0%BC%D0%B5%D0%BD%D1%8B%20%D0%BF%D0%B5%D1%80%D0%B5%D0%BC%D0%B5%D0%BD%D0%BD%D0%BE%D0%B9).jpg?raw=true)

# Интегрирование рациональных выражений. Разложение рациональной дроби на простейшие дроби. Метод неопределенных коэффициентов. (4 вопрос и 5 вопрос)




**По факту эти два вопроса являются одним вопросом**
---

## Рациональные дроби (определение, условия при которых дробь является рациональной)

Перед тем, как говорить об интегрировании надо понять, что такое рациональная дробь.

---

**Рациональная дробь** вида:

$$
R(x) = \frac{a_0x^n+a_1x^{n-1}+...\ + a_{n-1}x+a_n}{b_0x^m+b_1x^{m-1}+...\ + b_{m-1}x+b_m} = \frac{P_n(x)}{Q_m(x)}
$$

является правильной, если $n < m$ $\frac{x}{x^2+5}$

является неправильной, если $n>=m$ $\frac{x^3}{3x^2+7x-4}$

---

**Простая дробь** является рациональной дробью, если она является 1 из следующих 4 типов:

**1.** 
$$
\frac{A}{x + a} \ \ \text{или} \ \  \frac{A}{x - a} 

\ \ (A,a \in R)
$$

**2.**

$$
\frac{A}{(x + a)^n} \ \ \text{или} \ \  \frac{A}{(x - a)^n} 

\ \ (A,a \in R, \ n>=2)
$$

**3.**
$$
\frac{Mx+N}{x^2+px+q} \ \ \ \ (M, N, p, q \in R) , \ \ (x^2+px+q = 0)
$$

**4.**
$$
\frac{Mx+N}{(x^2+px+q)^n} \ \ \ \ (M, N, p, q \in R) , \ \ (x^2+px+q = 0)

\ \ (n>=2)
$$
---
Из каждой дроби можно взять интеграл:

**1.**
$$
A\ln(|x + a|) + C \ \ \ \text{или} \ \ \ A\ln(|x - a|) + C
$$

**2.**
$$
\frac{A}{(1-n)(x + a)^{n-1}} + C \ \ \ \text{или}
\ \ \ \frac{A}{(1-n)(x - a)^{n-1}} + C
$$

**3.**
$$
\frac{M}{2} \ln|x^2+px+q| + (N - \frac{PM}{2}) *\frac{1}{\sqrt{q - \frac{p^2}{4}}} * \arctg(\frac{x + \frac{P}{2}}{\sqrt{q - \frac{P^2}{4}}}) + C
$$

**4.**
$$
I_n = \frac{t}{a^2(n-1)(t^2+a^2)^{n-1}} - \frac{1}{a^n}\frac{2n-3}{2n-2} * I_{n-1}
$$ 
<i>На счет интеграла 4 типа я хз, может он неверн, надо будет проверить</i>

---

**Теорема:** Правильную дробь $\frac{P_n(x)}{Q_m(x)}\ , \ Q_m(x) = (x-a)^n * (x-b)^{\text{у меня там черточка}} *... \ * (x^2+px+q)^s$
можно обр. (хз что за полное слово) разложить на сумму простейших дробей
$$
\frac{P_n(x)}{Q_m(x)} = \frac{A_1}{x-a} + \frac{A_2}{(x-a)^2} +... + \frac{A_k}{(x-a)^k} + \frac{B_1}{x-b} + \frac{B_2}{(x-b)^2} +... +\frac{B_l}{(x-b^l)} + \frac{M_1x+N_1}{x^2+px+q} + \frac{M_2x+N_2}{(x^2+px+q)^2}
+ ...\  + \frac{M_sx+N_s}{(x^2+px+q)^s}
$$
---
Теперь, когда стало ясно, что такое рациональная дробь, стоит поговорить о том как найти интеграл от такой дроби, есть несколько методов:

## Метод неопределенных коэффециентов

Перед тем, как говорить о самом методе, нужно сказать, что очень важно определить является ли дробь **РАЦИОНАЛЬНОЙ**, потом является ли она **ПРАВИЛЬНОЙ** или **НЕПРАВИЛЬНОЙ**.

**Если дробь правильная** (самая большая степень вверху строго меньше самой большой степени внизу), то нужно просто разложить нижнию часть дроби на множители.

**Если дробь неправильная** (самая большая степень вверху больше или равна самой большой степени внизу), то нужно выделить целую часть (поделить верхнюю часть дроби на нижнюю), чтоб в итоге в выражении $S(x) + \frac{R(x)}{Q(x)}$ дробь $\frac{R(x)}{Q(x)}$ была правильной.
### Алгоритм выполнения

1. Разложить правильную рациональную дробь на простейшие дроби по формуле 1:
$$
\frac{P_n(x)}{Q_m(x)} = \frac{A}{x-a} + \frac{B}{x-b} + \frac{Cx+D}{x^2+px+q}
$$

2. Привести простейшие дроби к общему знаменателю

3. Приведем числители

4. Получаем СЛАУ, решая которую, получаем неопределенные коэффециенты. После этого находим интеграл
---
#### Пример решения

![1](https://github.com/Eggizac/MathAnaliz/blob/main/images/4%20%D0%B2%D0%BE%D0%BF%D1%80%D0%BE%D1%81%20(%D0%BF%D1%80%D0%B8%D0%BC%D0%B5%D1%80%201).jpg?raw=true)

## Метод частных значений

В данном методе придаем переменной x несколько частных значений (по числу неопределенных коэффициентов). Получим СЛАУ, решая которую, получим неопределенные коэффециенты. Данный метод очень быстро работает, когда корни многочлена простые и действительные.
#### Пример решения

![1](https://github.com/Eggizac/MathAnaliz/blob/main/images/4%20%D0%B2%D0%BE%D0%BF%D1%80%D0%BE%D1%81%20(%D0%BF%D1%80%D0%B8%D0%BC%D0%B5%D1%80%202).jpg?raw=true)

# Интегрирование иррациональных выражений (6 вопрос)

## Определение из лекции

**Интеграл** вида 

$$
\int{R (x, \sqrt{x^{m_1}}, \sqrt{x^{m_2}}, ...) dx} = |

\text{$x = t^S$, S - общий знаменатель дробей $\frac{m_1}{n_1}$, $\frac{m_2}{n_2}$} | =

\int{R (t^S, \frac{Sm_1}{n_1}, \frac{Sm_1}{n_1}, ...) St^{S-1}dt} \ \ \ 
\text{, где R - рациональная дробь, x - иррациональная часть}
$$

## Способ решения иррационального интеграла

Чтобы найти интеграл от иррациональной функции нужно нужно заменить подкоренное выражение на t со степенью корня. Например, для $\sqrt{x + 1}$ заменой будет являеться $t^2 = x + 1$, таким образом при подстановке получим $\sqrt{t^2} = t$. Теперь рассмотрим данный метод решения на некоторых примерах

## Примеры

![1](https://github.com/Eggizac/MathAnaliz/blob/main/images/6%20%D0%B2%D0%BE%D0%BF%D1%80%D0%BE%D1%81%20(%D0%BF%D1%80%D0%B8%D0%BC%D0%B5%D1%80%D1%8B).jpg?raw=true)

**P.s.** примеры взять отсюда http://mathprofi.ru/integrirovanie_kornei.html. Тут так же есть информация про интегрирование биноминальных интегралов.

# Интегрирование тригонометрических функций (8 вопрос)

## Способы нахождения 

### 1 способ (использование тригонометрических формул)

![1](https://github.com/Eggizac/MathAnaliz/blob/main/images/8%20%D0%B2%D0%BE%D0%BF%D1%80%D0%BE%D1%81%20(1%20%D0%BF%D1%80%D0%B8%D0%BC%D0%B5%D1%80).jpg?raw=true)

### 2 способ (понижение степени подынтегральной функции)

Данный приём работает, когда подынтегральные функции нафаршированы синусами и косинусами в чётных степенях. Для понижения степени используются форумлы:

$$
\sin(x)^2 = \frac{1 - \cos(2x)}{2} , \ \ \ \cos(x)^2 = \frac{1 + \cos(2x)}{2}, \ \ \ \sin(2x) = 2\sin(x)
$$

![1](https://github.com/Eggizac/MathAnaliz/blob/main/images/8%20%D0%B2%D0%BE%D0%BF%D1%80%D0%BE%D1%81%20(%D0%BF%D1%80%D0%B8%D0%BC%D0%B5%D1%80%202).jpg?raw=true)

### 3 способ (метод замены переменных)

![1](https://github.com/Eggizac/MathAnaliz/blob/main/images/8%20%D0%B2%D0%BE%D0%BF%D1%80%D0%BE%D1%81%20(%D0%BF%D1%80%D0%B8%D0%BC%D0%B5%D1%80%203).jpg?raw=true)

### 4 способ (универсальная тригонометрическая подстановка)
---

Универсальной тригонометрической подстановкой считается $t = \tg{\frac{x}{2}}$.

Таким образом, мы получаем, что

$$
\sin{x} = \frac{2t}{t^2 + 1}, \ \ \cos{x} = \frac{1 - t^2}{t^2 + 1}
$$

$$
\frac{x}{2} = \arctg{t}, \ \ x = 2\arctg{t}
$$
---
Универсальную тригонометрическую подстановку принято применять тогда, когда непонятно, что можно сделать, приведем пример такого случая:

![1](https://github.com/Eggizac/MathAnaliz/blob/main/images/8%20%D0%B2%D0%BE%D0%BF%D1%80%D0%BE%D1%81%20(%D0%BF%D1%80%D0%B8%D0%BC%D0%B5%D1%80%204).jpg?raw=true)

# Верхние и нижние суммы Дарбу. Свойства сумм Дарбу (10 вопрос)

![1](https://github.com/Eggizac/MathAnaliz/blob/main/images/10%20%D0%B2%D0%BE%D0%BF%D1%80%D0%BE%D1%81%20(1%20%D1%84%D0%BE%D1%82%D0%BE).png?raw=true)
![2](https://github.com/Eggizac/MathAnaliz/blob/main/images/10%20%D0%B2%D0%BE%D0%BF%D1%80%D0%BE%D1%81%20(2%20%D1%84%D0%BE%D1%82%D0%BE).png?raw=true)

# Свойства интегрируемых функций (12 вопрос)

![1](https://github.com/Eggizac/MathAnaliz/blob/main/images/12%20%D0%B2%D0%BE%D0%BF%D1%80%D0%BE%D1%81%201.png?raw=true)
![2](https://github.com/Eggizac/MathAnaliz/blob/main/images/12%20%D0%B2%D0%BE%D0%BF%D1%80%D0%BE%D1%81%202.png?raw=true)
![3](https://github.com/Eggizac/MathAnaliz/blob/main/images/12%20%D0%B2%D0%BE%D0%BF%D1%80%D0%BE%D1%81%203.png?raw=true)
![3](https://github.com/Eggizac/MathAnaliz/blob/main/images/12%20%D0%B2%D0%BE%D0%BF%D1%80%D0%BE%D1%81%204.png?raw=true)
![3](https://github.com/Eggizac/MathAnaliz/blob/main/images/12%20%D0%B2%D0%BE%D0%BF%D1%80%D0%BE%D1%81%205.png?raw=true)

# Определенный интеграл как функция верхнего предела. Формула Ньютона-Лейбница. (14 вопрос)

## Определенный интеграл как функция верхнего предела
![1](https://github.com/Eggizac/MathAnaliz/blob/main/images/14%20%D0%B2%D0%BE%D0%BF%D1%80%D0%BE%D1%81%201.png?raw=true)
![1](https://github.com/Eggizac/MathAnaliz/blob/main/images/14%20%D0%B2%D0%BE%D0%BF%D1%80%D0%BE%D1%81%202.png?raw=true)
## Формула Ньютона-Лейбница
![1](https://github.com/Eggizac/MathAnaliz/blob/main/images/14%20%D0%B2%D0%BE%D0%BF%D1%80%D0%BE%D1%81%203.png?raw=true)
![1](https://github.com/Eggizac/MathAnaliz/blob/main/images/14%20%D0%B2%D0%BE%D0%BF%D1%80%D0%BE%D1%81%204.png?raw=true)
![1](https://github.com/Eggizac/MathAnaliz/blob/main/images/14%20%D0%B2%D0%BE%D0%BF%D1%80%D0%BE%D1%81%205.png?raw=true)

# Формула интегрирования по частям для определенного интегралла (16 вопрос)

![1](https://github.com/Eggizac/MathAnaliz/blob/main/images/16%20%D0%B2%D0%BE%D0%BF%D1%80%D0%BE%D1%81%201.png?raw=true)
![1](https://github.com/Eggizac/MathAnaliz/blob/main/images/16%20%D0%B2%D0%BE%D0%BF%D1%80%D0%BE%D1%81%202.png?raw=true)
https://mathprofi.com/knigi_i_kursy/integraly/1_6_integrirovanie_po_chastyam_v_opredelennom_integrale.html

# Геометрические приложения определенного интеграла. Длина кривой и площадь плоской фигуры. (17 вопрос)

## Длина кривой

![1](https://github.com/Eggizac/MathAnaliz/blob/main/images/17%20%D0%B2%D0%BE%D0%BF%D1%80%D0%BE%D1%81%201.png?raw=true)
![1](https://github.com/Eggizac/MathAnaliz/blob/main/images/17%20%D0%B2%D0%BE%D0%BF%D1%80%D0%BE%D1%81%202.png?raw=true)
![1](https://github.com/Eggizac/MathAnaliz/blob/main/images/17%20%D0%B2%D0%BE%D0%BF%D1%80%D0%BE%D1%81%203.png?raw=true)
![1](https://github.com/Eggizac/MathAnaliz/blob/main/images/17%20%D0%B2%D0%BE%D0%BF%D1%80%D0%BE%D1%81%204.png?raw=true)
![1](https://github.com/Eggizac/MathAnaliz/blob/main/images/17%20%D0%B2%D0%BE%D0%BF%D1%80%D0%BE%D1%81%205.png?raw=true)

## Площадь плоской фигуры
http://mathprofi.ru/vychislenie_ploshadi_c_pomoshju_opredelennogo_integrala.html

# Геометрические приложения определенного интеграла. Площадь криволинейной трапеции и объем тела вращения. (18 вопрос)

## Площадь криволинейной трапеции

![1](https://github.com/Eggizac/MathAnaliz/blob/main/images/18%20%D0%B2%D0%BE%D0%BF%D1%80%D0%BE%D1%81%201.png?raw=true)
![1](https://github.com/Eggizac/MathAnaliz/blob/main/images/18%20%D0%B2%D0%BE%D0%BF%D1%80%D0%BE%D1%81%202.png?raw=true)
![1](https://github.com/Eggizac/MathAnaliz/blob/main/images/18%20%D0%B2%D0%BE%D0%BF%D1%80%D0%BE%D1%81%203.png?raw=true)

## Объем тела вращения
![1](https://github.com/Eggizac/MathAnaliz/blob/main/images/18%20%D0%B2%D0%BE%D0%BF%D1%80%D0%BE%D1%81%204.png?raw=true)
![1](https://github.com/Eggizac/MathAnaliz/blob/main/images/18%20%D0%B2%D0%BE%D0%BF%D1%80%D0%BE%D1%81%205.png?raw=true)
![1](https://github.com/Eggizac/MathAnaliz/blob/main/images/18%20%D0%B2%D0%BE%D0%BF%D1%80%D0%BE%D1%81%206.png?raw=true)

## Несобственный интеграл второго рода (20 вопрос)

![1](https://github.com/Eggizac/MathAnaliz/blob/main/images/20%20%D0%B2%D0%BE%D0%BF%D1%80%D0%BE%D1%81%201.png?raw=true)
![1](https://github.com/Eggizac/MathAnaliz/blob/main/images/20%20%D0%B2%D0%BE%D0%BF%D1%80%D0%BE%D1%81%202.png?raw=true)
![1](https://github.com/Eggizac/MathAnaliz/blob/main/images/20%20%D0%B2%D0%BE%D0%BF%D1%80%D0%BE%D1%81%203.png?raw=true)
