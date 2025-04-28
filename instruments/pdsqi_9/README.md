The Provider Documentation Summarization Quality Instrument (PDSQI-9) was developed to evaluate LLM-generated clinical summaries of multiple notes with a target specialty. Its development is outlined [here](https://arxiv.org/abs/2501.08977).

## Inputs

For evaluation, each item must have:

- summary: the single string of text to evaluate
- notes: a dictionary of notes used as reference for the summary
- target_specialty: the specialty of the target user, for which the summary was generated

## Outputs

The PDSQI-9 evaluation provides scores for the following distinct criteria:

- Citation: Accurately indicates when statements are drawn directly from source notes without appropriate attribution.
- Accurate: Evaluates the factual correctness of all information in the summary compared to the source notes.
- Thorough: Assesses whether the summary contains all important information from the source notes.
- Useful: Determines if the summary is helpful and relevant to the intended specialty provider.
- Organized: Evaluates how well the summary is structured in a logical and coherent fashion.
- Comprehensible: Measures how easily the summary can be understood without reference to the source notes.
- Succinct: Assesses whether the summary is appropriately concise without unnecessary information.
- Abstration: Evaluates the need for paraphrasing or synthesizing data. A no is represented as an NA response for Synthesized.
- Synthesized: Measures how well information from multiple notes is integrated into a coherent summary.
- Stigmatizing: Identifies presence of potentially stigmatizing language that could bias patient care. (Yes/No)

Each criterion is scored on a 5-point scale unless noted as Yes/No.
