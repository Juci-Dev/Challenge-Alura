Análise de Evasão de Clientes – Telecom X part 2

Projeto de Data Science para analisar churn em uma empresa fictícia de telecomunicações. O objetivo é identificar fatores que influenciam a evasão e avaliar modelos preditivos para apoiar estratégias de retenção.

🛠️ Tecnologias Utilizadas

Linguagem: Python

Bibliotecas: Pandas, NumPy, Scikit-Learn, Statsmodels, Imbalanced-Learn, XGBoost

Visualização: Matplotlib, Seaborn

🎯 Objetivos

Preparar e tratar os dados (encoding, normalização, balanceamento).

Analisar variáveis e correlações.

Treinar modelos de classificação (Logistic Regression e XGBoost).

Avaliar métricas de desempenho.

Interpretar variáveis mais relevantes.

Gerar recomendações estratégicas para reduzir churn.

🔎 Principais Fatores de Evasão

Tempo de permanência: contratos longos → menor risco.

Gastos totais: altos gastos → maior risco.

Tipo de internet: fibra ótica associada a mais cancelamentos.

Modelo contratual: contratos anuais/bianuais reduzem churn.

Serviços adicionais: streaming, suporte técnico e cobrança eletrônica ajudam na retenção.

🤖 Modelos Avaliados
Logistic Regression – Detector Sensível

Recall: 81% dos churns identificados.

Mais falsos positivos (419).

Melhor ROC AUC: 84,5%.

XGBoost – Detector Conservador

Recall: apenas 44% dos churns.

Menos falsos positivos (250).

ROC AUC: 80,9%.

📌 Conclusão: Logistic Regression é o melhor modelo (captura mais churns e salva +250 clientes a cada 1000 potenciais cancelamentos).

🔮 Próximos Passos

Testar técnicas de balanceamento (SMOTEENN, class weights).

Criar novas features (ex.: tempo até cancelamento, gasto atual vs histórico).

Ajustar hiperparâmetros com GridSearchCV / Optuna.

Explorar ensembles (Logistic + XGBoost).

Ajustar thresholds para otimizar recall/precisão.

✅ Conclusão

Contratos longos, perfil de uso da internet e gastos totais são fatores críticos no churn.

Logistic Regression apresentou melhor recall e AUC, sendo o modelo recomendado.

Estratégias devem focar em fidelização com contratos longos, melhorias na fibra ótica e valorização de clientes de alto valor.
