# Challenge_Alura_TelecomX

# 📊 Telecom X: Análisis de Retención de Clientes (Churn)

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?style=for-the-badge&logo=python)
![Pandas](https://img.shields.io/badge/Pandas-1.3.0-150458?style=for-the-badge&logo=pandas)
![Seaborn](https://img.shields.io/badge/Seaborn-0.11.2-444876?style=for-the-badge)

## Introducción
Este proyecto presenta un análisis profundo sobre la deserción de clientes (**Churn**) en la compañía **Telecom X**, la cual registra una tasa de abandono del **26.5%**. El objetivo principal es identificar los factores demográficos, contractuales y de servicio que impulsan esta métrica para proponer estrategias de retención basadas en evidencia de datos.

El análisis aborda el problema desde una perspectiva técnica (limpieza de datos) y estratégica (insights de negocio).

##  Limpieza y Tratamiento de Datos
Para garantizar resultados precisos, se realizó un proceso exhaustivo de ingeniería de datos:
* **Importación:** Carga de datos desde una API externa en formato JSON y transformación a DataFrame.
* **Depuración:** Se gestionaron valores nulos en cargos totales y se eliminaron registros con inconsistencias en la etiqueta de Churn.
* **Estandarización:** Traducción de categorías al español y renombrado de columnas para mejorar la legibilidad del análisis.
* **Ingeniería de Características:** * Creación de la métrica `cuentas_diarias`.
    * Limpieza de cargos totales mediante expresiones regulares.
    * Transformación de variables binarias y categóricas para análisis estadístico.

##  Análisis Exploratorio de Datos (EDA)
El estudio visual y estadístico reveló patrones críticos en el comportamiento del cliente:
* **Antigüedad:** El **53% del abandono** ocurre en los primeros **6 meses**, identificando una etapa de "alto riesgo" inicial.
* **Servicios de Internet:** Los usuarios de **Fibra Óptica** presentan un churn del **41.9%**, un área de oportunidad crítica frente al DSL.
* **Contratos:** Los contratos mensuales presentan una tasa de evasión del **42.7%**, comparada con el **2.8%** de los contratos a dos años.
* **Correlación:** Se detectó que a mayor cargo mensual, mayor es la probabilidad de abandono, impactando directamente en los clientes de mayor valor.



##  Conclusiones e Insights
1. **Puntos de Inflexión:** La mediana de contrato es de **29 meses**. Cruzar esta barrera reduce drásticamente la probabilidad de fuga.
2. **Anclas de Fidelidad:** Los clientes con pareja, dependientes o servicios de **soporte técnico** tienden a ser significativamente más leales.
3. **Fricción en Pagos:** El método de **cheque electrónico** está fuertemente vinculado a la deserción (**45.3%**), sugiriendo una necesidad de digitalización.
4. **Perfil del Desertor:** Generalmente es un usuario nuevo, con contrato mensual, cargos altos y sin servicios adicionales de seguridad o soporte.

##  Recomendaciones
Basado en el análisis, se sugieren las siguientes acciones estratégicas:
* **Onboarding Intensivo:** Seguimiento proactivo durante los primeros 90 días para clientes de fibra óptica.
* **Incentivos de Permanencia:** Campañas de migración de contratos mensuales a anuales.
* **Ecosistema de Valor:** Promover servicios de seguridad y soporte técnico como "anclas" de retención.
* **Renovación Preventiva:** Activar alertas de retención a partir del mes 20 de antigüedad para evitar el churn en el ciclo bianual.

##  Cómo ejecutar el proyecto
1. Clonar el repositorio:
   ```bash
   git clone [https://github.com/tu-usuario/nombre-del-repo.git](https://github.com/tu-usuario/nombre-del-repo.git)
