# 📦 Previsão de Reposição de Estoque com Amazon SageMaker Canvas

Este projeto demonstra como utilizar o **Amazon SageMaker Canvas** para criar um modelo preditivo capaz de identificar se um produto precisa ou não de reposição (**reorder_needed**) com base em dados de estoque e vendas.

O objetivo é construir um fluxo completo de **Machine Learning sem código (no-code)**, desde o upload do dataset até a geração de previsões em lote.

---

## 🚀 Objetivo do Projeto

Usando dados simulados de estoque de eletrônicos, iremos:

- Fazer upload do dataset no SageMaker Canvas  
- Treinar um modelo preditivo (Quick Build)
- Prever quais produtos precisam ser reabastecidos
- Exportar os resultados para análise

---

## 📂 Dataset Utilizado

O dataset contém as seguintes colunas:

- `product_id`
- `product_name`
- `category`
- `brand`
- `stock_quantity`
- `daily_sales_avg`
- `reorder_needed` (coluna alvo)

---

# ✅ Guia Passo a Passo (com Prints)

---

## 1. Acessar o Console da AWS

Abra a página inicial do Console da AWS.

![Step 00](./prints/00-aws-console-home.png)

---

## 2. Buscar por SageMaker Canvas

Utilize a barra de pesquisa para localizar o **SageMaker Canvas**.

![Step 01](./prints/01-busca-sagemaker-canvas.png)

---

## 3. Abrir o Dashboard do SageMaker

Acesse o painel principal do SageMaker.

![Step 02](./prints/02-home-sagemaker-dashboard.png)

---

## 4. Criar um Domínio

Vá até a configuração de Domínio e crie um novo domínio.

![Step 03](./prints/03_sagemaker_dominios_criar_dominio.png)

---

## 5. Configuração de Usuário Único

Selecione a opção de configuração rápida para um único usuário.

![Step 04](./prints/04_configuracao_dominio_usuario_unico.png)

---

## 6. Botão Desabilitado Durante Setup

Durante o processo de criação, o botão pode ficar desabilitado.

![Step 05](./prints/05_botao_configurar_dominio_desabilitado.png)

---

## 7. Configuração do Ambiente do Studio

O Canvas inicia o processo de preparação do ambiente.

![Step 06](./prints/06_setup_studio_configurando_ambiente_16.png)

![Step 07](./prints/07_setup_studio_configurando_ambiente_96.png)

![Step 08](./prints/08_setup_studio_configurando_ambiente_100.png)

---

## 8. Status do Domínio como READY

Após finalizar, o domínio aparece como pronto (READY).

![Step 09](./prints/09_dominio_criado_status_ready.png)

---

## 9. Abrir o SageMaker Studio

Clique para abrir o Studio pelo dashboard.

![Step 10](./prints/10_dashboard_sagemaker_abrir_studio.png)

---

## 10. Página Inicial do Studio (Modelos)

Dentro do Studio, acesse a seção de modelos.

![Step 11](./prints/11_sagemaker_studio_home_models.png)

---

## 11. Página Inicial do Canvas Parada (Stopped)

O Canvas pode iniciar em estado parado.

![Step 12](./prints/12_canvas_pagina_inicial_stopped.png)

---

## 12. Workspace Iniciando

O Canvas inicializa o ambiente de trabalho.

![Step 13](./prints/13_canvas_iniciando_workspace.png)

---

## 13. Canvas em Execução

O status muda para running.

![Step 14](./prints/14_canvas_status_running.png)

---

## 14. Integração com Amazon Q

A interface do Canvas inclui suporte do Amazon Q.

![Step 15](./prints/15_canvas_web_home_amazon_q.png)

---

## 15. Criar Novo Modelo

Inicie o processo de criação de modelo.

![Step 16](./prints/16_canvas_web_home_create_model_card.png)

---

## 16. Modal de Novo Modelo

O Canvas abre a janela de criação.

![Step 17](./prints/17_canvas_create_new_model_modal.png)

---

## 17. Botão Desabilitado Até Preencher Campos

O botão fica desabilitado até completar os dados.

![Step 18](./prints/18_canvas_create_model_button_disabled.png)

---

## 18. Selecionar Tipo de Problema Preditivo

Escolha análise preditiva.

![Step 19](./prints/19_canvas_problem_type_predictive_selection.png)

---

## 19. Selecionar Dataset

O Canvas pede a origem do dataset.

![Step 20](./prints/20_canvas_select_dataset_screen.png)

---

## 20. Criar Nome do Dataset

Defina um nome para o dataset.

![Step 21](./prints/21_create_dataset_name.png)

---

## 21. Tela de Upload do Dataset

Faça upload do arquivo CSV.

![Step 22](./prints/22_upload_dataset_screen.png)

---

## 22. Selecionar Arquivo CSV no Windows

Escolha o arquivo local.

![Step 23](./prints/23_select_csv_file_windows.png)

---

## 23. Arquivo Carregado com Sucesso

Canvas confirma que o dataset foi carregado.

![Step 24](./prints/24_file_loaded_ready_preview.png)

---

## 24. Importação e Prévia Carregando

O Canvas processa o preview.

![Step 25](./prints/25_import_preview_loading.png)

---

## 25. Prévia da Tabela do Dataset

Visualize linhas e colunas.

![Step 26](./prints/26_dataset_table_preview.png)

---

## 26. Lista de Processamento do Dataset

Canvas prepara os dados.

![Step 27](./prints/27_dataset_processing_list.png)

---

## 27. Selecionar Coluna Alvo

Escolha a coluna que será prevista.

![Step 28](./prints/28_select_target_column_screen.png)

---

## 28. Coluna Alvo: reorder_needed

Selecione `reorder_needed`.

![Step 29](./prints/29_target_column_reorder_needed.png)

---

## 29. Colunas do Dataset Carregadas

Canvas confirma todas as colunas.

![Step 30](./prints/30_canvas_dataset_loaded_columns.png)

---

## 30. Dropdown de Seleção do Target

Menu dropdown para confirmar.

![Step 31](./prints/31_canvas_select_target_column_dropdown.png)

---

## 31. Quick Build Pronto

Canvas está pronto para treinar rapidamente.

![Step 32](./prints/32_canvas_target_selected_quick_build_ready.png)

---

## 32. Pré-processamento e Validação

Canvas valida e prepara os dados.

![Step 33](./prints/33_canvas_preprocessing_validating_data.png)

---

## 33. Métricas e Impacto de Variáveis

Canvas mostra precisão e importância.

![Step 34](./prints/34_canvas_model_analysis_accuracy_impact.png)

---

## 34. Previsão em Lote Manual

Selecione batch prediction manual.

![Step 35](./prints/35_canvas_predict_batch_manual_option.png)

---

## 35. Modal para Dataset de Previsão

Canvas solicita dataset para prever.

![Step 36](./prints/36_canvas_select_dataset_for_predictions_modal.png)

---

## 36. Job de Previsão Criado

A previsão em lote foi criada com sucesso.

![Step 37](./prints/37_canvas_prediction_job_created.png)

---

## 37. Toast: Previsões Prontas

Canvas exibe notificação.

![Step 38](./prints/38_canvas_predictions_ready_toast.png)

---

## 38. Resultados Finais + Download

Tabela final de previsões com opção de download.

![Step 39](./prints/39_canvas_prediction_results_table_download.png)

---

# ✅ Resultado Final

Você agora tem uma previsão completa mostrando quais produtos precisam de reposição.

Este laboratório demonstra como o SageMaker Canvas permite aplicar Machine Learning sem escrever código.

---

# 📌 Próximos Melhorias Possíveis

- Exportar resultados para dashboards (QuickSight / Power BI)
- Trocar dataset simulado por dados reais de loja
- Automatizar previsões contínuas

---

## 👩‍💻 Autora

Criado por **Tatiana Cristina de Araujo**  
QA Engineer migrando para IA + Dados 🚀
