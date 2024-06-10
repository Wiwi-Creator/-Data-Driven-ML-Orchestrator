架構規劃圖:
```
└── 📁/
    └── 📁usr
        └── 📁data_archt
            /* each folder below will be a respostory */
            └── 📁grafana
            └── 📁redis
            └── 📁mysql
            └── 📁mongo
            └── 📁elk
            └── 📁kafka
            └── 📁python_module
            └── 📁airflow
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
            └── 📁dbt
            └── 📁mlflow
            └── 📁fastapi
            └── 📁dash
            └── 📁docker
                /* the folder put the docker build and docker compose up scripts in */
                └── 📁docker_build
                └── 📁docker_compose
            └── README.md
```