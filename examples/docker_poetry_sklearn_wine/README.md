# MLFlow 101
Build, deploy & serve model tutorial with MLFlow

## Get started

### Spin up cluster with docker
  + Spin up mlflow cluster:
    ```bash
    docker-compose up --build
    
    ```
  + Tear down mlflow cluster:
    ```bash
    docker-compose down --remove-orphans
    
    ```

### Local install
#### 1. Install dependancies
```bash
poetry install -v
```

#### 2. Run notebook
```bash
poetry run jupyter lab
```

#### 3. Run MLFlow
```bash
poetry run mlflow run  .

```

#### 4. Run MLFlow UI
```bash
poetry run mlflow ui

```
#### 5. Train Model
```bash
poetry run python train.py

```
    
## Tutorials
+ [Quickstart: Install MLflow, instrument code & view results in minutes](https://mlflow.org/docs/latest/quickstart.html)