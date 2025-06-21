# PLAICraft: Age Groups Likely To Contribute More to Data (R, K-NN Regression)
### Members: Victor T., Jack G., Andy W., Danny Z.

***Main question***: What is the age group of players that are likely to contribute the most to the datasets?

This project explores how player age relates to engagement in video games, using real-world datasets from the **Pacific Laboratory for Artificial Intelligence (PLAI)** at the University of British Columbia (UBC). Specifically, it aims to identify which **age group of players** is more likely to contribute a larger volume of data—measured by **total playtime**—to support ongoing AI research in gaming environments for PLAICraft Research Team.

The analysis is conducted in **R** using a tidy modelling workflow that includes **data wrangling**, **exploratory data analysis (EDA)**, and a **K-Nearest Neighbours (KNN) regression model**. The model is evaluated using **10-fold cross-validation** and **Root Mean Squared Prediction Error (RMSPE)**.

## 🔍 Key Features
- Investigated age-related trends in total playtime using `KNN` regression
- Cleaned and merged two datasets: `players.csv` and `sessions.csv`
- Preprocessed data using `recipes`, and modelled using `parsnip` and `workflows`
- Applied **10-fold cross-validation** and reported **RMSPE** for model accuracy
- Discussed the impact of outliers, dataset size, and audio activity exclusions

## 🧠 Key Insights
- Players aged **17–20** (post-secondary students) had the **highest total playtime**
- Despite expectations, younger players contributed **less** overall playtime
- Model RMSPE was **38.26 hours**, largely influenced by extreme outliers
- The correlation between age and playtime was **positive but weak**
- Suggests university-age players may be ideal candidates for targeted research or product development

## 🛠️ Technologies Used
- `R`, `Jupyter Notebook` (via JupyterLab)
- `repr`, `tidymodels`, `tidyverse`,  `ggplot2`

## 📊 Dataset
Internal anonymized datasets provided by PLAI:
- `players.csv`: Contains hashed emails and age
- `sessions.csv`: Contains session start/end times in UNIX format  
(Only `players.csv` was used for modelling due to its relevance to the research question)

## 📚 Reference
- El-Helaly, M. (2024). Artificial Intelligence and occupational health and safety, benefits and drawbacks. PubMed, 115(2), e2024014–e2024014. https://doi.org/10.23749/mdl.v115i2.15835

- Johnson, D., Gardner, J., & Sweetser, P. (2016). Motivations for videogame play: Predictors of time spent playing. Computers in Human Behavior, 63, 805–812. https://doi.org/10.1016/j.chb.2016.06.028

- Khlaif, Z. N., Mousa, A., Hattab, M. K., Itmazi, J., Hassan, A. A., Sanmugam, M., & Ayyoub, A. (2023). The potential and concerns of using AI in scientific research: ChatGPT performance evaluation. JMIR Medical Education, 9, e47049. https://doi.org/10.2196/47049

- PLAICraft. (2024). Plaicraft.ai. https://www.plaicraft.ai/

- Rashid, A. B., & Karim, A. (2024). AI revolutionizing industries worldwide: A comprehensive overview of its diverse applications. Hybrid Advances, 7, 100277–100277. https://doi.org/10.1016/j.hybadv.2024.100277

- Tang, X., Li, X., Ding, Y., Song, M., & Bu, Y. (2020). The pace of artificial intelligence innovations: Speed, talent, and trial-and-error. Journal of Informetrics, 14(4), 101094–101094. https://doi.org/10.1016/j.joi.2020.101094

