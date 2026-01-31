# 📘 Manual do Projeto — Previsão de Estoque com SageMaker Canvas

Este manual documenta o passo a passo completo do laboratório realizado no **Amazon SageMaker Canvas**, utilizando Machine Learning para prever reposição de estoque.

---

## ✅ Objetivo

Criar um modelo de classificação capaz de prever se um produto precisa ou não de reposição (`reorder_needed`), baseado em dados de vendas e estoque.

---

## 1. Upload do Dataset

O dataset foi importado via upload local no Canvas.

📌 Arquivo utilizado:

- `electronics_inventory_dataset_v2_pro.csv`

🖼️ Print:

![Upload Dataset](./prints/01-upload.png)

---

## 2. Pré-visualização e Criação do Dataset

Após o upload, o Canvas exibiu uma prévia das colunas e linhas antes da importação final.

🖼️ Print:

![Preview Dataset](./prints/02-preview.png)

---

## 3. Seleção da Coluna Target

A coluna escolhida como alvo foi:

- `reorder_needed`

Ela representa se o produto precisa ou não ser reabastecido.

🖼️ Print:

![Target Column](./prints/03-target.png)

---

## 4. Treinamento com Quick Build

O modelo foi treinado automaticamente utilizando a opção **Quick Build**.

🖼️ Print:

![Quick Build](./prints/04-quickbuild.png)

---

## 5. Avaliação do Modelo

O Canvas apresentou métricas de performance:

- Accuracy: 100%
- F1 Score: 1.000

🖼️ Print:

![Model Metrics](./prints/05-metrics.png)

---

## 6. Geração de Predições (Batch Prediction)

Foi executada uma previsão em lote utilizando o dataset completo.

🖼️ Print:

![Batch Prediction](./prints/06-batch.png)

---

## 7. Download do Arquivo Final

O arquivo final com as previsões foi exportado:

📌 Arquivo gerado:

- `electronics_inventory_predictions.csv`

🖼️ Print:

![Predictions Output](./prints/07-output.png)

---

## ✅ Conclusão

O projeto demonstrou como utilizar o **Amazon SageMaker Canvas** para criar um modelo de Machine Learning sem código, aplicando IA para decisões inteligentes de estoque.

🚀 Resultado pronto para uso em cenários reais de varejo e logística.
