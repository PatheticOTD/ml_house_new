#on_policy #model_free

Рассмотрим MDP, определенного кортежем (S A P r p_0  $\gamma$) где S - states set, A - finite acitons set, P: SxAxS - [[Transition probability distribution]]

В reinforcement learning, если просто на каждом шаге делать градиентный апдейт политики (policy gradient), можно получить **резкие скачки стратегии** → это ломает обучение и приводит к нестабильности.

**Trust Region Policy Optimization** (TRPO) вводит _ограничение_ на изменение политики между итерациями, чтобы гарантировать **монотонный рост вознаграждения** и избежать "разрушительных" апдейтов.

TRPO буквально **переписывает задачу обучения с подкреплением** как задачу оптимизации с ограничением:

$$max⁡θ  E^[πθ(a∣s)πθold(a∣s)A^(s,a)]\max_{\theta} \; \hat{\mathbb{E}} \left[ \frac{\pi_{\theta}(a|s)}{\pi_{\theta_{\text{old}}}(a|s)} \hat{A}(s,a) \right]θmax​E^[πθold​​(a∣s)πθ​(a∣s)​A^(s,a)]
$$
**при условии:**

E^s[DKL(πθold(⋅∣s)  ∥  πθ(⋅∣s))]≤δ\hat{\mathbb{E}}_{s} \left[ D_{\mathrm{KL}}\left( \pi_{\theta_{\text{old}}}(\cdot|s) \;\|\; \pi_{\theta}(\cdot|s) \right) \right] \le \deltaE^s​[DKL​(πθold​​(⋅∣s)∥πθ​(⋅∣s))]≤δ

- **Целевая функция** — surrogate objective: аппроксимирует прирост вознаграждения.
    
- **Ограничение** — средний KL-divergence между старой и новой политикой ≤ δ\deltaδ. Это _trust region_ — зона допустимого изменения параметров.