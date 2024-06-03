# Простейшие пределы и некоторые связанные приёмы
## Пределы функций
**Структура предела** - $\lim\limits_{x \to x_0} f(x) = a$\
*lim* - оператор предела \
$f(x)$ - от какой функции \
$x \to x_0$ - предел по какой базе \
$a$ - ответ (чему равен предел, может отсутствовать - предела нет).

**Предел** отвечает на вопрос как некая функция $f(x)$ ведёт себя в окрестности некоей точки (аргумент $x$ приближается к какому-то значению). \
Т.е. к какому значению стремится функция $f(x)$ по некоторой базе $x \to x_0$. \
Пределы бывают лево и правосторонние.

Пределы важны для *Машинноего обучения*, так как оно занимается вопросами оптимизации. 
Поэтому через пределы (производные, градиенты) возможно минимизировать различные фукнционалы, максимизировать метрики.

### Строгое определение предела функции
$\lim\limits_{x \to x_0} f(x) = a \iff \forall \varepsilon > 0 \ \exists \sigma_\varepsilon > 0: \ f(\dot{U_{\sigma_\varepsilon}} (x_0)) \subset V_\varepsilon(a)$ \
Какую бы маленькую $\varepsilon$-окрестность точки $a$ мы ни взяли, всегда найдётся такая $\sigma$-окрестность точки $x_0$, 
что её образ будет полностью лежать внутри $\varepsilon$-окрестности точки $a$

### Связь односторонних пределов с двусторонними
Двусторонний предел одинаково стремится к точке $x_0$ с обеих сторон $\lim\limits_{x \to x_0} f(x) = a$\
Односторонний предел стремится к точке $x_0$ с правой стороны ($\lim\limits_{x \to x_0^+} f(x) = a$) или с левой стороны ($\lim\limits_{x \to x_0^-} f(x) = a$).

## Базовые элементарные функции и их пределы
Проверка правильности вычисленного предела исходя из строго определения предела\
$\forall \varepsilon > 0 \ \exists \sigma_\varepsilon > 0: \ f(\dot{U_{\sigma_\varepsilon}} (x_0)) \subset V_\varepsilon(a) \iff \forall \varepsilon > 0 \ \exists \sigma_\varepsilon > 0: \ \forall x:|x-x_0| < \sigma \to |f(x)-a| < _\varepsilon$

**Простейшие пределы некоторых элементарных функций**\
$f(x) = \frac{1}{x}$ \
$\lim\limits_{x \to -\infty} \frac{1}{x} = 0$ \
$\lim\limits_{x \to +\infty} \frac{1}{x} = 0$ \
$\lim\limits_{x \to 0^+} \frac{1}{x} = +\infty$ \
$\lim\limits_{x \to 0^-} \frac{1}{x} = -\infty$ \
Но матиметики договорились, плюс и минус бесконечности - это бесконечности (строго формально значение не существует) и последние два предела можно записать вот так 
$\lim\limits_{x \to 0} \frac{1}{x} = \infty$

$f(x) = 2^x$ \
$\lim\limits_{x \to -\infty} 2^x = 0$ \
$\lim\limits_{x \to +\infty} 2^x = +\infty$

$f(x) = \frac{1}{2}^x$ \
$\lim\limits_{x \to -\infty} \frac{1}{2}^x = +\infty$ \
$\lim\limits_{x \to +\infty} \frac{1}{2}^x = 0$

$f(x) = log_e x$ \
$\lim\limits_{x \to 0^+} log_e x = -\infty$ \
$\lim\limits_{x \to +\infty} log_e x = +\infty$

$f(x) = log_{\frac{1}{5}} x$ \
$\lim\limits_{x \to 0^+} log_{\frac{1}{5}} x = +\infty$ \
$\lim\limits_{x \to +\infty} log_{\frac{1}{5}} x = -\infty$

$f(x) = arcctg \ x$ \
$\lim\limits_{x \to -\infty} arcctg \ x = \pi$ \
$\lim\limits_{x \to +\infty} arcctg \ x = 0$

$f(x) = arctg \ x$ \
$\lim\limits_{x \to -\infty} arctg \ x = -\frac{\pi}{2}$ \
$\lim\limits_{x \to +\infty} arctg \ x = \frac{\pi}{2}$ \

Эти пределы не требуют вычислений и наглядно видны по графикам функций.

