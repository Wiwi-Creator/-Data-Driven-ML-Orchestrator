模組說明:
```
目前規劃共8個模組:
1. DB - Postgre
2. MQ - Redis
3. Workflow Manager - Airflow
4. Log Manager - ELK
5. Data Module Build Tool - dbt
6. Api Platform - Fastapi
7. Streaming Event Platform - Kafka
8. ML Platform - mlflow

依序建置以上模組來建立資料架構，不限定以上工具並依現實發展做評估更換，並保持各功能模組可替換工具性。
1. DB的建置提供資料存儲的服務，以結構化資料為主，不限且必須包含非結構化資料
2. MQ緩存即時且小量數據
3. Workflow Manager提供任務排列與調度功能
4. Log Manager集中管控各服務Log，兼具儲存文本資料
5. Data Module Build Tool擔任資料模組創建與資料轉換的工具
6. Api Platform提供向外資料服務，例如對外API服務或網頁顯示
7. Streaming Event Platform 提供流資料處理服務
8. ML Platform 提供機器學習開發、模型版本控制服務
```

模組狀態:
| 模組 | 狀態 | 首次發布時間 | 預計首次發布時間 | 邀請協助 |
|----------|----------|----------|----------|----------|
| DB | 已發行 | 2024-06-10 | 2024-06-10 | - |
| MQ | 未發行 | - | 2024-06-16 |-|
| Workflow Manager | 未發行 | - | 2024-06-10 | - |
| Log Manager | 未發行 | - | 2024-07-14 | - |
| Data Module Build Tool | 已發行 | 2024-06-10 | 2024-06-10 | Wiwi |
| Api Platform | 未發行 | - | 2025-09-15 | Wiwi,Andy |
| Streaming Event Platform | 未發行 | - | 2025-10-13 | - |
| ML Platform | 未發行 | - | 2025-12-15 | - |

架構規劃:
```
└── 📁/
    └── 📁usr
        └── 📁data_archt
            /* each folder below will be a respostory in the future */
            /* the * after the folder means it's priority to build */
            └── 📁grafana *
            └── 📁redis ***
            └── 📁mysql ***
            └── 📁mongo ***
            └── 📁elasticswarch **
            └── 📁kibana **
            └── 📁logstash **
            └── 📁kafka ***
            └── 📁python_module ***
            └── 📁airflow ***
                └── 📁images
                    └── Dockerfile
                    └── requirements.txt
                    └── docker-compose.yaml
                └── 📁dags
                    └── 📁DL
                        └── DL.py
                        └── 📁FLOWS
                            └── DAG_PARSE.json
                            └── ODSFlow.json
                    └── 📁ODS
                    └── 📁DW
                    └── 📁DM
                    └── 📁AP
                └── 📁config
                └── 📁logs
                └── 📁plugins
            └── 📁dbt ***
            └── 📁mlflow **
            └── 📁fastapi *
            └── 📁dash *
            └── 📁docker ***
                /* Put the docker build and docker compose up scripts in the folder */
                /* Design cd pattern to capture the change and do the action what we want */
                └── 📁docker_build
                └── 📁docker_compose
            └── build.sh
            └── README.md
```

發行日誌:
```
2024-06-10 14:04:00 新增架構說明與規劃(README)
2024-06-10 14:10:00 發行 DB - Postgre
```