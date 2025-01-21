# Assessing European and Brazilian Portuguese LLMs for NER in Specialised Domains

Named Entity Recognition (NER) is a fundamental task in Natural Language Processing (NLP) that involves identifying and classifying entities such as names, organizations, locations, dates, and more within a given text. This study evaluates the impact of Portuguese variants in Large Language Models (LLMs) for NER in specialised domains, focusing on Brazilian Portuguese legal texts and European Portuguese historical documents.

We evaluated the performance of BERTimbau (PT-BR), Albertina (PT-PT and PT-BR), and XLM-R (multilingual), highlighting the importance of linguistic alignment and model architecture in improving NER performance.

## Results Summary

### Parish Memories Corpus (European Portuguese)
| Model            | Precision | Recall | F1 Score |
|-----------------|-----------|--------|----------|
| Albertina PT-PT | **72.76%** | 76.10% | **74.39%** |
| Albertina PT-BR | 69.71%    | 73.11% | 71.37%   |
| XLM-R-Large     | 68.31%    | 73.38% | 70.76%   |
| BERTimbau-Large | 67.36%    | **74.00%** | 70.53%   |

### UlyssesNER-Br Corpus (Brazilian Portuguese)
| Model            | Precision | Recall | F1 Score |
|-----------------|-----------|--------|----------|
| Albertina PT-PT | 86.83%    | 91.32% | **89.02%** |
| Albertina PT-BR | **87.93%** | 89.98% | 88.94%   |
| XLM-R-Large     | 82.39%    | 89.82% | 85.94%   |
| BERTimbau-Large | 84.14%    | **90.32%** | 87.12%   |

## Datasets

- **Parish Memories Corpus (PT-PT):** Annotated 18th-century historical texts from Portugal.
- **UlyssesNER-Br Corpus (PT-BR):** Legislative documents annotated with fine-grained legal entities.

## Models Used

1. **BERTimbau (PT-BR)** - Pre-trained on Brazilian Portuguese corpora.
2. **Albertina PT-PT/PT-BR** - Two variants trained on European and Brazilian Portuguese.
3. **XLM-R** - A multilingual transformer model supporting over 100 languages.

## Conclusion

This study underscores the importance of using language-specific models for domain-specific NER tasks. The Albertina PT-PT model excelled in historical texts, while Albertina PT-BR performed well on legislative texts. Future work will explore domain adaptation techniques to further improve results.

## Citation

```
@inproceedings{nunes2024assessing,
  author    = {Rafael Oleques Nunes, Joaquim Santos, Andre Spritzer, Dennis Giovani Balreira, Carla Maria Dal Sasso Freitas, Fernanda Olival, Helena Freire Cameron, Renata Vieira},
  title     = {Assessing European and Brazilian Portuguese LLMs for NER in Specialised Domains},
  booktitle = {Proceedings of BRACIS 2024},
  year      = {2024}
}
```

## Acknowledgements
This work was supported by CAPES (Brazil) and FCT (Portugal).
