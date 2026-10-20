# The IndexHot GEO Measurement Standard v1.0 (October 2026)

## 1. The Problem with Black-Box Scores
Generative Engine Optimization (GEO) requires more than just tracking keywords. It requires understanding how AI models retrieve, synthesize, and cite information. Existing tools often provide a single, opaque score. Without an open methodology, users cannot verify the data, reproduce the results, or optimize their content effectively.

## 2. The Measurement Framework

### 2.1 Governed Question Library
Measurements must be based on real user queries, not just brand names. The IndexHot standard requires a minimum of 50 questions per brand:
- **10 Brand Prompts:** Direct questions about the brand (e.g., "What is [Brand]?").
- **40 Non-Brand Prompts:** Category-level questions where the brand *could* be recommended (e.g., "Best [Category] tools for B2B SaaS").

### 2.2 Citation Metrics
We define three levels of AI visibility:
- **Mention (Level 1):** The brand name appears anywhere in the AI's generated text.
- **Citation (Level 2):** The AI provides a clickable link or explicit reference to the brand's website or properties (e.g., Wikipedia, G2).
- **Absorption (Level 3):** The AI not only cites the brand but uses its content as the primary factual basis for the answer. (Studies show Perplexity has high citation rates but low absorption, while ChatGPT has lower citations but higher absorption).

### 2.3 Cross-Platform Scoring
A brand's final IndexHot Score is a weighted average across platforms (ChatGPT, Perplexity, Gemini). The score accounts for:
- Overall Mention Rate
- Average Rank Position (when listed)
- Citation Quality (domain authority of the cited source)
- Sentiment (positive, neutral, negative)

## 3. How to Reproduce

1. **Build the Prompt Library:** Create 10 brand prompts and 40 category prompts relevant to your industry.
2. **Execute Queries:** Run the prompts through ChatGPT, Perplexity, and Gemini. (Note: Ensure fresh sessions to avoid context contamination).
3. **Record Data:** Document the Mention, Citation Source, and Rank Position for each query.
4. **Calculate Score:** Apply the IndexHot weighting formula (available in the `geo-data` repository).

## 4. Open Data
The data generated using this standard is published openly. You can access the datasets and contribute to the research at: [https://github.com/indexhot-code/geo-data](https://github.com/indexhot-code/geo-data)
