We release surprisal estimates for ten languages in the MECO corpus (Finnish, Greek, Koean, Russian, Turkish, English, Spanish, Estonian, Italian, German). These estimates have been extracted using a multilingual neural language model, namely XGLM (Lin et al., 2022).

The columns in the dataframe that include surprisal values are:
"s": surprisal calculated by XGLM - 564 million parameters (smallest model)
"s_1.7": surprisal calculated by XGLM - 1.7 billion parameters
"s_2.9": surprisal calculated by XGLM - 2.9 billion parameters
"s_4.5": surprisal calculated by XGLM - 4.5 billion parameters (largest model)
Each "s" column is paired with a "m" correspondent (e.g. "m_1.7"), which indicates whether the surprisal has been computed by summing over multiple sub-word log-probabilities. This shouldn't be a problem (surprisal is additive by definition, and we kept those words in our analyses), but previous studies have removed them (e.g., Boyce & Levy, 2023).

We recommend to use the values computed from the smallest model if you are working with early eye-movement data (e.g., first fixation duration, gaze duration), and to consider a slightly bigger model (XGLM - 1.7 billion) if you are working on late measurements (total reading time; see our paper - https://aclanthology.org/2023.acl-short.14/ - on how different surprisal estimates better capture certain eye-movement measurements). 

Our code is publicly available on GitHub (https://github.com/Andrea-de-Varda/surprisal-across-languages/tree/main). Note that the code can be easily adapted for other language models to derive surprisal estimates for languages in the MECO corpus that are not included in our sample (e.g., Dutch).

OSF link for estimates and further details: 
https://osf.io/vcbp6/

If you use these surprisal estimates, please cite:
Andrea de Varda and Marco Marelli. 2023. Scaling in Cognitive Modelling: a Multilingual Approach to Human Reading Times. In Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 2: Short Papers), pages 139–149, Toronto, Canada. Association for Computational Linguistics.
