
>[!definition] 
>
$$n!:=\prod_{i=1}^n i=\prod_{i=1}^n(n-i+1)=\prod_{i=0}^{n-1}(n-i)$$


>[!theorem]
>$n!= n(n-1)!$

>[!theorem] Stirling Approximation
$$n! \approx \sqrt{2 \pi n} \left(\frac{n}{e}\right)^n$$



- $$k^nn!=\prod_{i=1}^nki$$ 

>[!definition] Falling Factorial
A *falling factorial* is defined as:$$n^\underline{k}:=\prod_{i=1}^k(n-i+1)=\prod_{i=0}^{k-1}(n-i)$$



>[!definition] Rising Factorial
A *rising factorial* is defined as: $$n^\overline{k}:=\prod_{i=1}^k(n+i-1)=\prod_{i=0}^{k-1}(n+i)$$

>[!theorem]
$$n!=1^\overline{k}=k^\underline{k}$$

>[!theorem] Relationship with normal factorial
$$n^\underline{k}=\frac{n!}{(n-k)!}=\binom{n}{k}k!$$
$$n^\overline{k}=\frac{(n+k+1)!}{(m-1)!}=\binom{n+k-1}{k}k!$$
