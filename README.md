# ML-Orchestrator

## 目的

透過 Workflow Orchestrator 將外部資料作清整並匯入至Data warehouse (batch/streaming)

並根據資料內容作模型訓練,並產出視覺化資料。

  *註* : 本次案例將以各項經濟/股市..等公開資訊為主

-------------------------------

## 專案說明

目前規劃共4個Repo

- [Workflow Manager - Airflow, Dagster]()
- [Data Module Build Tool(dbt)]()
- [Streaming Event Platform](https://github.com/Wiwi-Creator/FinDataLoader)
- [ML mlflow]()

依序建置以上模組來建立資料架構，不限定以上工具並依現實發展做評估更換，並保持各功能模組可替換工具性。

- DB的建置提供資料存儲的服務，以結構化資料為主，不限且必須包含非結構化資料
- Workflow Manager 提供任務排列與調度功能
- dbt 擔任資料模組創建與資料轉換的工具
- Kafka 提供Streaming Data Process
- ML Platform 提供機器學習開發、模型版本控制服務

-------------------------------

## 專案狀態
| Application | Status | Release Time | Expected Release Time | Developer | Supporter | repo |
|----------|----------|----------|----------|----------|----------|----------|
| Airflow/Dagster | Continue | - | 2024-09-10 | Wiwi | Josh | []() |
| dbt | Continue | - | 2024-09-10 | Josh | Wiwi | [dbt](https://github.com/JoshuaChen40/data_archt_dbt.git) |
| Streaming Event Platform | Continue | - | 2024-09-10 | Wiwi | Josh | []() |
| MLflow | Continue | - | 2024-09-10 | Josh | Andy | []() |

