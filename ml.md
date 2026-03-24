# Machine Learning / AI Engineering — Plan de estudios vivo

## 0. Meta-capa: qué significa saber ML

- formular problemas correctamente
- representar datos
- elegir y entrenar modelos con criterio
- evaluar sin engañarse
- entender límites (estadísticos, computacionales)
- desplegar y mantener sistemas en producción
- razonar sobre incertidumbre

---

## 1. Mathematical Foundations

### 1.1. Álgebra lineal
- vectores, matrices, tensores
- espacios vectoriales
- transformaciones lineales
- autovalores y autovectores
- SVD
- normas y métricas

### 1.2. Probabilidad
- variables aleatorias
- distribuciones
- esperanza, varianza
- independencia
- ley de grandes números
- teorema central del límite

### 1.3. Estadística
- estimación
- inferencia
- intervalos de confianza
- tests de hipótesis
- sesgo vs varianza

### 1.4. Optimización
- gradiente
- descenso de gradiente
- convexidad
- Lagrangianos
- regularización

### 1.5. Qué debería saber hacer
- derivar funciones de coste
- interpretar distribuciones
- entender cuándo un resultado es estadísticamente débil
- razonar sobre convergencia

---

## 2. Data as First-Class Object

### 2.1. Tipos de datos
- tabulares
- series temporales
- texto
- imágenes
- grafos
- señales

### 2.2. Representación
- feature engineering
- embeddings
- normalización / escalado
- codificación (one-hot, ordinal, etc.)

### 2.3. Calidad
- missing data
- outliers
- leakage
- bias en datos
- distribución train vs test

### 2.4. Qué debería saber hacer
- detectar cuándo el problema es de datos y no de modelo
- diseñar features útiles
- evitar leakage
- entender que garbage in → garbage out

---

## 3. Supervised Learning

### 3.1. Problemas
- clasificación
- regresión

### 3.2. Modelos clásicos
- regresión lineal
- regresión logística
- k-NN
- Naive Bayes
- SVM
- árboles de decisión
- random forests
- gradient boosting (XGBoost, LightGBM)

### 3.3. Evaluación
- train / validation / test split
- cross-validation
- métricas:
  - accuracy
  - precision / recall
  - F1
  - ROC-AUC
  - MSE / MAE

### 3.4. Qué debería saber hacer
- elegir modelo según datos y problema
- interpretar métricas correctamente
- evitar overfitting
- ajustar hiperparámetros con criterio

---

## 4. Unsupervised Learning

### 4.1. Clustering
- k-means
- hierarchical clustering
- DBSCAN

### 4.2. Reducción de dimensión
- PCA
- t-SNE
- UMAP

### 4.3. Modelos generativos básicos
- Gaussian Mixture Models

### 4.4. Qué debería saber hacer
- descubrir estructura en datos sin labels
- interpretar clusters (no solo generarlos)
- usar reducción de dimensión para análisis y no solo visualización

---

## 5. Statistical Learning Theory (nivel conceptual)

### 5.1. Conceptos
- riesgo empírico vs real
- generalización
- bias-variance tradeoff
- overfitting / underfitting
- regularización

### 5.2. Qué debería saber hacer
- entender por qué un modelo funciona o no
- no confiar en métricas sin contexto
- interpretar resultados con incertidumbre

---

## 6. Deep Learning

### 6.1. Fundamentos
- perceptrón
- redes feedforward
- backpropagation
- funciones de activación
- inicialización

### 6.2. Arquitecturas
- CNN
- RNN / LSTM / GRU
- Transformers
- attention mechanisms

### 6.3. Entrenamiento
- optimizers (SGD, Adam)
- batch / mini-batch
- learning rate schedules
- regularización (dropout, weight decay)

### 6.4. Qué debería saber hacer
- entender qué calcula una red (no solo usarla)
- diagnosticar problemas de entrenamiento
- distinguir cuándo DL es overkill

---

## 7. Natural Language Processing

### 7.1. Representación
- bag of words
- TF-IDF
- embeddings (word2vec, GloVe)

### 7.2. Modelos modernos
- transformers
- BERT / GPT-like

### 7.3. Tareas
- clasificación
- NER
- QA
- generación

### 7.4. Qué debería saber hacer
- entender limitaciones del lenguaje natural
- evaluar outputs más allá de métricas automáticas
- manejar prompts con criterio

---

## 8. Computer Vision

### 8.1. Fundamentos
- convoluciones
- filtros
- detección de bordes

### 8.2. Modelos
- CNNs
- object detection
- segmentation

### 8.3. Qué debería saber hacer
- entender cómo una imagen se transforma en features
- distinguir tareas (classification vs detection vs segmentation)

---

## 9. Time Series

- autocorrelación
- ARIMA
- modelos estacionales
- forecasting
- anomalías

Qué debería saber hacer:
- detectar patrones temporales
- evitar leakage temporal
- evaluar correctamente predicciones en el tiempo

---

## 10. Reinforcement Learning (conceptual)

- agentes
- estados
- acciones
- recompensas
- políticas
- Q-learning
- exploración vs explotación

---

## 11. ML Engineering 

### 11.1. Pipeline
- data ingestion
- preprocessing
- training
- validation
- deployment

### 11.2. Herramientas
- Python ecosystem
- notebooks vs código productivo
- reproducibilidad

### 11.3. Model lifecycle
- versionado de datos
- versionado de modelos
- experiment tracking
- model registry

### 11.4. Qué debería saber hacer
- pasar de notebook a sistema reproducible
- automatizar pipelines
- evitar experimentos irreproducibles

---

## 12. MLOps

### 12.1. Producción
- serving (batch vs online)
- APIs de modelos
- latencia vs throughput

### 12.2. Monitorización
- data drift
- concept drift
- performance decay

### 12.3. Retraining
- pipelines automáticos
- triggers

### 12.4. Qué debería saber hacer
- mantener modelos vivos en producción
- detectar cuándo dejan de funcionar
- evitar degradación silenciosa

---

## 13. Evaluation & Experimentation

### 13.1. Diseño experimental
- A/B testing
- offline vs online evaluation

### 13.2. Métricas reales
- métricas técnicas vs métricas de negocio

### 13.3. Qué debería saber hacer
- no optimizar la métrica equivocada
- detectar p-hacking
- validar impacto real

---

## 14. Ethics & Limitations

- bias
- fairness
- explainability
- privacidad
- uso indebido

Qué debería saber hacer:
- identificar riesgos éticos
- explicar limitaciones del modelo
- no sobreprometer capacidades

---

## 15. Performance & Scaling

- GPU vs CPU
- batch inference
- model compression
- quantization
- distillation

---

## 16. Specialization Tracks

### 16.1. Applied ML
- pipelines
- modelos clásicos
- negocio

### 16.2. Deep Learning Engineer
- arquitecturas
- entrenamiento a escala
- optimización

### 16.3. ML Systems
- infra
- serving
- scaling
- distributed training

### 16.4. Research
- teoría
- papers
- nuevos modelos

---

## 17. Self-assessment

- 0–7 como en SWE

---

## 18. Evidence

- notebooks reproducibles
- datasets procesados
- modelos entrenados
- experimentos comparativos
- deployment real
- análisis de errores

---

## 19. Missing areas

- teoría de generalización más profunda
- optimización avanzada
- modelos probabilísticos complejos
- RL aplicado real
- ML distribuido
