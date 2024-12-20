# Sovai's Open Investment Datasets
![Hugging Face Logo](https://huggingface.co/front/assets/huggingface_logo-noborder.svg) 

Building the industry's first open-source datasets for investment research. Unlike traditional vendors who limit trials to institutions, we believe in open access. Free access to all datasets with a brief delay; [subscribers](https://sov.ai) receive real-time data.


## 👋 About Me
I'm [Derek Snow](https://github.com/firmai/), founder and researcher at [sov.ai](https://sov.ai). My focus lies in **AI & ML in Quantitative Finance**, where I develop and curate datasets to advance research and applications in this field. 


## 🌐 Connect with Me

[LinkedIn](https://www.linkedin.com/in/snowderek/) | [GitHub](https://github.com/sovai-research/) | [Hugging Face](https://huggingface.co/sovai)

## 📚 Datasets

The price is for commercial usage of lagged data. If you are an academic ignore it, simply download your data from Huggingface!

| Emoji | Dataset | Description | Documentation | Price p/m |
|-------|---------|-------------|---------------|-------------------|
| 📰 | [sovai/news_sentiment](https://huggingface.co/datasets/sovai/news_sentiment) | Two types of news datasets have been developed, one is ticker-matched, and the next is theme-matched. | [Documentation](https://docs.sov.ai/realtime-datasets/equity-datasets/news-sentiment) | $200 |
| 📈 | [sovai/price_breakout](https://huggingface.co/datasets/sovai/price_breakout) | A dataset with daily updated predictions of price breaking upwards for US Equities. | [Documentation](https://docs.sov.ai/realtime-datasets/equity-datasets/price-breakout) | $220 |
| 🔍 | [sovai/insider_flow_prediction](https://huggingface.co/datasets/sovai/insider_flow_prediction) | More than 60+ insider trading features helpful for machine learning, including a flow prediction value. | [Documentation](https://docs.sov.ai/realtime-datasets/equity-datasets/insider-flow-prediction) | $465 |
| 💼 | [sovai/institutional_trading](https://huggingface.co/datasets/sovai/institutional_trading) | The dataset provides a comprehensive analysis of institutional investment behaviors, strategies, and portfolio dynamics. | [Documentation](https://docs.sov.ai/realtime-datasets/equity-datasets/institutional-trading) | $580 |
| 📢 | [sovai/lobbying_data](https://huggingface.co/datasets/sovai/lobbying_data) | A ticker-matched lobbying data to see fine-grained corporate lobbying behavior. | [Documentation](https://docs.sov.ai/realtime-datasets/equity-datasets/lobbying-data) | $645 |
| 🔽 | [sovai/short_selling](https://huggingface.co/datasets/sovai/short_selling) | This section covers the usage of various short-selling datasets for risk analysis. | [Documentation](https://docs.sov.ai/realtime-datasets/equity-datasets/short-selling) | $780 |
| 📖 | [sovai/wikipedia_views](https://huggingface.co/datasets/sovai/wikipedia_views) | A look at some of the largest firms and their daily Wikipedia page views and trends. | [Documentation](https://docs.sov.ai/realtime-datasets/equity-datasets/wikipedia-views) | $200 |
| 💊 | [sovai/pharma_clinical_trials](https://huggingface.co/datasets/sovai/pharma_clinical_trials) | This section covers a very unique dataset that tags clinical trials with their predicted outcome success. | [Documentation](https://docs.sov.ai/realtime-datasets/sectorial-datasets/pharma-clinical-trials) | $850 |
| 📊 | [sovai/factor_signals](https://huggingface.co/datasets/sovai/factor_signals) | This dataset includes traditional accounting factors, alternative financial metrics, and advanced statistical analyses, enabling sophisticated financial modeling. | [Documentation](https://docs.sov.ai/realtime-datasets/equity-datasets/factor-signals) | $270 |
| 📉 | [sovai/financial_ratios](https://huggingface.co/datasets/sovai/financial_ratios) | More than 80+ financial ratios calculated from financial statement and market data. | [Documentation](https://docs.sov.ai/realtime-datasets/equity-datasets/financial-ratios) | $270 |
| 📜 | [sovai/government_contracts](https://huggingface.co/datasets/sovai/government_contracts) | Government contracts data from publicly traded companies. | [Documentation](https://docs.sov.ai/realtime-datasets/equity-datasets/government-contracts) | $580 |
| ⚠️ | [sovai/corp_risks](https://huggingface.co/datasets/sovai/corp_risks) | Chapter 7 and Chapter 11 bankruptcy predictions made easy for over 13,000 US publicly traded stocks. | [Documentation](https://docs.sov.ai/realtime-datasets/equity-datasets/corp-risks) | $270 |
| 🛡️ | [sovai/risks](https://huggingface.co/datasets/sovai/risks) |  We offer daily updates on global risk perceptions, using leading indicators and advanced models to forecast various types of risk. | [Documentation](https://docs.sov.ai/realtime-datasets/economic-datasets/turing-risk-index) | $270 |
| 💬 | [sovai/cfpb_complaints](https://huggingface.co/datasets/sovai/cfpb_complaints) | This section covers the usage of the Consumer Financial Complaint ticker-mapped dataset. | [Documentation](https://docs.sov.ai/realtime-datasets/sectorial-datasets/cfpb-complaints) | $480 |
| 🧮 | [sovai/risk_indicators](https://huggingface.co/datasets/sovai/risk_indicators) | We construct a comprehensive corporate risk score for US stocks by analyzing company events. | [Documentation](https://docs.sov.ai/realtime-datasets/equity-datasets/risk-indicators) | $270 |
| 🚦 | [sovai/traffic_agencies](https://huggingface.co/datasets/sovai/traffic_agencies) | Data on government website agency traffic. | [Documentation](https://docs.sov.ai/realtime-datasets/economic-datasets/government-traffic) | $250 |
| 👥 | [sovai/earnings_surprise](https://huggingface.co/datasets/sovai/earnings_surprise) | Earnings announcements are obtained from external sources as well as estimate information leading up to the actual announcement. | [Documentation](https://docs.sov.ai/realtime-datasets/equity-datasets/earnings-surprise) | $680 |
| ❗ | [sovai/bankruptcy](https://huggingface.co/datasets/sovai/bankruptcy) | Chapter 7 and Chapter 11 bankruptcy predictions made easy for over 5,000 US publicly traded stocks. | [Documentation](https://docs.sov.ai/realtime-datasets/equity-datasets/bankruptcy-predictions) | $270 |

**Cost Tip:** For commercial access to all **30 real-time datasets** on [docs.sov.ai](https://docs.sov.ai), I recommend you subscribe to the **$285 p/m package**, you can save as much as **90%** of the costs. 

All our datasets are in beta, be part of our development process. Submit suggestions or error reports through the issues portal.

## 🧪 Example Use Cases

```bash
pip install datasets
```
    
Below are example code snippets demonstrating how to load each dataset using the Hugging Face `datasets` library.

- 📰 **[sovai/news_sentiment](https://huggingface.co/datasets/sovai/news_sentiment)**
    ```python
    from datasets import load_dataset
    df_news_sentiment = load_dataset("sovai/news_sentiment", split="train").to_pandas()
    ```

- 📈 **[sovai/price_breakout](https://huggingface.co/datasets/sovai/price_breakout)**
    ```python
    from datasets import load_dataset
    df_price_breakout = load_dataset("sovai/price_breakout", split="train").to_pandas()
    ```

- 🔍 **[sovai/insider_flow_prediction](https://huggingface.co/datasets/sovai/insider_flow_prediction)**
    ```python
    from datasets import load_dataset
    df_insider_flow = load_dataset("sovai/insider_flow_prediction", split="train").to_pandas()
    ```

- 💼 **[sovai/institutional_trading](https://huggingface.co/datasets/sovai/institutional_trading)**
    ```python
    from datasets import load_dataset
    df_institutional_trading = load_dataset("sovai/institutional_trading", split="train").to_pandas()
    ```

- 📢 **[sovai/lobbying_data](https://huggingface.co/datasets/sovai/lobbying_data)**
    ```python
    from datasets import load_dataset
    df_lobbying_data = load_dataset("sovai/lobbying_data", split="train").to_pandas()
    ```

- 🔽 **[sovai/short_selling](https://huggingface.co/datasets/sovai/short_selling)**
    ```python
    from datasets import load_dataset
    df_short_selling = load_dataset("sovai/short_selling", split="train").to_pandas()
    ```

- 📖 **[sovai/wikipedia_views](https://huggingface.co/datasets/sovai/wikipedia_views)**
    ```python
    from datasets import load_dataset
    df_wikipedia_views = load_dataset("sovai/wikipedia_views", split="train").to_pandas()
    ```

- 💊 **[sovai/pharma_clinical_trials](https://huggingface.co/datasets/sovai/pharma_clinical_trials)**
    ```python
    from datasets import load_dataset
    df_pharma_trials = load_dataset("sovai/pharma_clinical_trials", split="train").to_pandas()
    ```

- 📊 **[sovai/factor_signals](https://huggingface.co/datasets/sovai/factor_signals)**
    ```python
    from datasets import load_dataset
    df_factor_signals = load_dataset("sovai/factor_signals", split="train").to_pandas()
    ```

- 📉 **[sovai/financial_ratios](https://huggingface.co/datasets/sovai/financial_ratios)**
    ```python
    from datasets import load_dataset
    df_financial_ratios = load_dataset("sovai/financial_ratios", split="train").to_pandas()
    ```

- 📜 **[sovai/government_contracts](https://huggingface.co/datasets/sovai/government_contracts)**
    ```python
    from datasets import load_dataset
    df_government_contracts = load_dataset("sovai/government_contracts", split="train").to_pandas()
    ```

- ⚠️ **[sovai/corp_risks](https://huggingface.co/datasets/sovai/corp_risks)**
    ```python
    from datasets import load_dataset
    df_corp_risks = load_dataset("sovai/corp_risks", split="train").to_pandas()
    ```

- 🛡️ **[sovai/risks](https://huggingface.co/datasets/sovai/risks)**
    ```python
    from datasets import load_dataset
    df_risks = load_dataset("sovai/risks", split="train").to_pandas()
    ```

- 💬 **[sovai/cfpb_complaints](https://huggingface.co/datasets/sovai/cfpb_complaints)**
    ```python
    from datasets import load_dataset
    df_cfpb_complaints = load_dataset("sovai/cfpb_complaints", split="train").to_pandas()
    ```

- 🧮 **[sovai/risk_indicators](https://huggingface.co/datasets/sovai/risk_indicators)**
    ```python
    from datasets import load_dataset
    df_risk_indicators = load_dataset("sovai/risk_indicators", split="train").to_pandas()
    ```

- 🚦 **[sovai/traffic_agencies](https://huggingface.co/datasets/sovai/traffic_agencies)**
    ```python
    from datasets import load_dataset
    df_traffic_agencies = load_dataset("sovai/traffic_agencies", split="train").to_pandas()
    ```

- 👥 **[sovai/earnings_surprise](https://huggingface.co/datasets/sovai/earnings_surprise)**
    ```python
    from datasets import load_dataset
    df_earnings_surprise = load_dataset("sovai/earnings_surprise", split="train").to_pandas()
    ```

- ❗ **[sovai/bankruptcy](https://huggingface.co/datasets/sovai/bankruptcy)**
    ```python
    from datasets import load_dataset
    df_bankruptcy = load_dataset("sovai/bankruptcy", split="train").to_pandas()
    ```

