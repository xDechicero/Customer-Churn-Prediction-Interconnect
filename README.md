# Predicción de Cancelación de Clientes — Interconnect Telecom

En el sector de telecomunicaciones, anticipar la pérdida de clientes permite reducir el churn, personalizar estrategias de retención y mejorar el valor de vida del cliente. Este proyecto se centra en **predecir qué usuarios tienen mayor probabilidad de cancelar su servicio**, apoyando al área de marketing con decisiones basadas en datos.

#### 🛠️Herramientas y tipo de proyecto
![Python](https://img.shields.io/badge/python-357ebd?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23357ebd.svg?style=for-the-badge&logo=pandas&logoColor=white)
![LightGBM](https://img.shields.io/badge/LightGBM-357ebd?style=for-the-badge)
![scikit-learn](https://img.shields.io/badge/scikit--learn-%23357ebd.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
![EDA](https://img.shields.io/badge/Análisis_Exploratorio-295F98?style=for-the-badge)
![Balanceo de clases](https://img.shields.io/badge/Balanceo_de_clases-295F98?style=for-the-badge)
![Modelado predictivo](https://img.shields.io/badge/Modelado_predictivo-295F98?style=for-the-badge)

### Preguntas clave
1. ¿Qué variables afectan más la cancelación de clientes?
2. ¿Cuál es la probabilidad de que un cliente abandone el servicio?
3. ¿Qué perfiles presentan mayor riesgo de churn?

### Metodología

- **Integración y limpieza de datos:** Se consolidaron 4 fuentes de datos (`contract.csv`, `internet.csv`, `phone.csv`, `personal.csv`), tratando valores faltantes y estandarizando variables categóricas.
- **Exploratory Data Analysis (EDA):** Se identificaron patrones como el impacto de contratos mensuales y métodos de pago electrónicos en la cancelación.
- **Balanceo de clases:** Se aplicó upsampling con técnicas de remuestreo para equilibrar la clase objetivo (cancelación vs no cancelación).
- **Modelado predictivo:** Se entrenó un modelo con LightGBM, logrando un AUC-ROC de `0.805`.
- **Interpretabilidad:** Se analizaron las variables más relevantes para comprender las razones detrás de las predicciones.

### ✅Conclusiones y recomendaciones

#### Factores clave del churn:
- **Contratos mensuales** presentan mayor riesgo de abandono.
- **Método de pago "Electronic Check"** asociado con mayor tasa de cancelación.
- **Falta de servicios adicionales** como soporte técnico, seguridad o streaming, correlaciona con clientes que abandonan.

#### Estrategias recomendadas:
- **Campañas de fidelización personalizadas** para clientes en riesgo.
- **Promociones en servicios adicionales** como soporte o antivirus para aumentar el compromiso.
- **Incentivos para contratos anuales o bianuales**, especialmente para usuarios nuevos.
- **Segmentación automatizada de clientes**, integrando el modelo predictivo en procesos de CRM.
