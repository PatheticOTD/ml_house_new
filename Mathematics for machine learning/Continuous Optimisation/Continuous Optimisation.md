по сути это просто нахождение минимумов функций.
![[Pasted image 20250807151925.png]]
Есть [[Unconstrained optimization]] и [[Constrained optimization]].

Предполагается, что все оптимизируемые функции дифференцируемы.

### Constrained Optimization and Lagrange Multipliers

Самый простой способ лечения проблем с [[Constrained optimization]] это просто смерджить всё в единую функцию, добавив функцию индикатора: $$J(x) = f(x) + \sum\limits_{i=1}^{m}(g_{i}(x))$$
где $l$ - 