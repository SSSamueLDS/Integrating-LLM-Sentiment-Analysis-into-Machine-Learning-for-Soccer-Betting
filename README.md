# Sports-betting-with-Machine-Learning

[](https://github.com/SSSamueLDS/Integrating-LLM-Sentiment-Analysis-into-Machine-Learning-for-Soccer-Betting/tree/main)

**Code & experiments for the paper:** [*Integrating LLM Sentiment Analysis into Machine
Learning for Soccer Betting*](https://wi-lab.com/cyberchair/2025/icdm25/scripts/submit.php?subarea=S09&undisplay_detail=1&wh=/cyberchair/2025/icdm25/scripts/ws_submit.php)

It supports:

* **Reproducible experiments** from the paper.

## Features

[](https://github.com/SSSamueLDS/Integrating-LLM-Sentiment-Analysis-into-Machine-Learning-for-Soccer-Betting/tree/main)

* **Prompt templates** : Zero shot templates to get sentiment score with LLM.
* **Evaluation metrics** : F1 , logloss
* **Reproducibility** : Saves raw model features, parameters, hyperparameters, metrics results.
* **Analysis notebooks** : plotting of figures/tables for the paper.

---

## Repository Structure

[](https://github.com/SSSamueLDS/Integrating-LLM-Sentiment-Analysis-into-Machine-Learning-for-Soccer-Betting/tree/main)

```

betting_simulation_results/ # tick-by-tick raw betting simulation results
dataset/                    # raw and processed datasets used for the paper
final_compiled_results/     # compiled results (metrics) and model betting performance and figures 
model_metric_json/          # saved hyperparameters of the models
model_performance_results/  # model parameters, raw metrics results per model
notebooks/                  # Analysis notebooks 
pkl_files/                  # saved ran models.
```

## Setup

[](https://github.com/SSSamueLDS/Integrating-LLM-Sentiment-Analysis-into-Machine-Learning-for-Soccer-Betting/tree/main)

* **Python** : 3.10+ recommended
* **Install dependencies** :

```shell
pip install -r requirements.txt
```

* **Configure environment:**

```shell
cp .env.example .env
```

* Set keys and paths in .env:
  * OPENAI_API_KEY — for OpenAI models
  * DEEPSEEK_API_KEY + BASE_URL — for DeepSeek/OpenAI-compatible endpoints
  * QWEN_API_KEY - For Qwen Models
  * GOOGLE_API_KEY - To search for BBC commentary articles on specific matches
  * GOOGLE_CX - To search for BBC commentary articles on specific matches

## Datasets

[](https://github.com/SSSamueLDS/Integrating-LLM-Sentiment-Analysis-into-Machine-Learning-for-Soccer-Betting/tree/main)

* EPL Soccer Statistics:
  * Various match statistics from 2015-16 to 2023-24 seasons (dataset/epl_stats)
* EPL Historical Betting Odds:
  * 2023-24 EPL Betting Odds(dataset/epl_odds)
* BBC Match Commentaries:
  * BBC Post-Match Commentaries from 2015-16 to 2023-24 seasons (dataset/epl_sentiment_analysis/bbc_articles)

## License

[](https://github.com/SSSamueLDS/Integrating-LLM-Sentiment-Analysis-into-Machine-Learning-for-Soccer-Betting/tree/main)

MIT — see LICENSE.
