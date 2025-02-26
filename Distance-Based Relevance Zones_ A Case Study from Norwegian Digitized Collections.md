  
Distance-Based Relevance Zones: A Case Study from Norwegian Digitized Collections

This paper extends distance and frequency-based approaches for measuring distributional relevance between words by introducing a three-zone model of contextual relevance. Using data from the Norwegian newspaper digitization project, we demonstrate how the right context of target words can be systematically divided into three distinct zones: near (1-3 words), middle (4-8 words), and distant (\>8 words), each capturing different types of linguistic relationships.

Our analysis shows that these zones exhibit distinct statistical patterns in terms of Pointwise Mutual Information (PMI, treated here as Radon-Nikodym derivatives) and positional variance. The near zone typically captures syntactic relationships with high PMI and low positional variance, while the distant zone reveals discourse-level relationships with selective high PMI values and moderate variance. The middle zone serves as a transition area, characterized by higher variance and generally lower PMI values.

We combine PMI values with position statistics to create zone-specific word embeddings and graphs. The data is captured in tuples of the form (w₁, w₂, pmi, dist, dist\_variance), where:

\- pmi \= p(w₂|w₁)/p(w₂) measures co-occurrence strength  
\- dist \= avg(position(w₂)-position(w₁)) captures average distance  
\- dist\_variance \= variance(dist) indicates positional consistency

Initial results from Norwegian newspaper data (1800-2020) show distinct patterns in how different word classes behave across these zones, offering new perspectives on historical language change and textual organization. The approach enables efficient analysis of large historical corpora while maintaining sensitivity to both local syntactic and broader discourse patterns.

