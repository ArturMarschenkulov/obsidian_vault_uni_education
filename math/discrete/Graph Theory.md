
>[!definition] Independence System
Let $S$ be a finite set. Let $\mathscr{I} \subseteq \mathcal{P}(S) \setminus \varnothing$ which has the following axioms:
>- $\varnothing \in \mathscr{I}$
>- $\forall X \in \mathscr{I}: \forall Y \subseteq S: Y \subseteq X \implies Y \in \mathscr{I}$
>
>Then $I = (S, \mathscr{I})$ is an *independence system*.


>[!definition] Matroid
Let $M = (S, \mathscr{I})$ be an *independence system*, which has the following property:
>- $\forall U, V \in \mathscr{I}: |V|<|U| \implies \exists x \in U \setminus V:V \cup \set{x}\in\mathscr{I}$ (Exchange Property
>
>Then $M$ is a *matroid*.

