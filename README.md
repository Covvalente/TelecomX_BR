
# 📊 Análise de Evasão de Clientes (Customer Churn)

Neste repositório, apresento um projeto completo de Ciência de Dados focado na análise da evasão de clientes (Churn) de uma empresa fictícia de telecomunicações. O objetivo principal é transformar dados brutos em **insights estratégicos** para a equipe de retenção.

---

## 📖 O Problema de Negócio

O custo de aquisição de um novo cliente (CAC) é muito maior do que o custo de manter um cliente atual. Nesta empresa, a taxa geral de evasão está na casa dos **27%**. A missão deste projeto é responder: 
* *Quais perfis de clientes estão cancelando os serviços?*
* *Quais fatores têm maior correlação com a decisão de cancelamento?*

---

## 🛠️ Tecnologias Utilizadas

Este projeto foi desenvolvido utilizando as seguintes tecnologias e bibliotecas:

* **Linguagem:** Python 3.x
* **Manipulação de Dados:** Pandas, NumPy
* **Visualização de Dados:** Matplotlib, Seaborn
* **Ambiente de Desenvolvimento:** Google Colab / Jupyter Notebook

---

## 🚀 Como Executar o Projeto

Siga os passos abaixo para rodar a análise na sua máquina local:

1. **Clone este repositório:**
   ```bash
   git clone [https://github.com/SEU_USUARIO/NOME_DO_REPOSITORIO.git](https://github.com/SEU_USUARIO/NOME_DO_REPOSITORIO.git)

```

2. **Navegue até o diretório do projeto:**
```bash
cd NOME_DO_REPOSITORIO

```


3. **Instale as dependências necessárias:**
```bash
pip install pandas numpy matplotlib seaborn

```


4. **Abra o notebook:**
Inicie o Jupyter Notebook ou importe o arquivo `.ipynb` para o Google Colab e execute as células sequencialmente.

---

## 🔍 Etapas do Projeto

O desenvolvimento foi dividido nas seguintes fases:

1. **Coleta e Limpeza de Dados:** - Tratamento de valores nulos (NaN) e inconsistências.
* Conversão de tipos de dados (ex: `Charges_Total` de *string* para *float*).
* Tradução de colunas e registros para o português.


2. **Feature Engineering:**
* Criação da variável `Cobranca_Diaria`.
* Criação da variável `Total_Servicos` (soma dos serviços adicionais contratados).


3. **Análise Exploratória de Dados (EDA):**
* Geração de gráficos de barras, pizza, densidade (KDE) e boxplots.
* Construção de painéis para comparar categorias (Gênero, Contrato, etc.) com a variável alvo (`Cancelou`).


4. **Análise de Correlação:**
* Criação de Heatmaps para entender a relação matemática entre tempo de contrato, cobranças e evasão.



---

## 💡 Principais Insights Extraídos

Durante a Análise Exploratória, descobrimos padrões cruciais sobre a evasão:

* **Fidelidade Contratual:** Clientes com contratos de renovação **Mensal** são os grandes responsáveis pela taxa de evasão. Contratos anuais e bienais têm churn quase nulo.
* **Período Crítico (Onboarding):** A maior parte dos cancelamentos ocorre nos **primeiros 5 meses** de assinatura. Se o cliente ultrapassa o primeiro ano, a retenção é altíssima.
* **Serviços Críticos:** Assinantes do serviço de **Fibra Óptica** e usuários que pagam via **Cheque Eletrônico** apresentam taxas de cancelamento desproporcionalmente altas.
* **Engajamento no Ecossistema:** Comprovamos matematicamente que clientes que contratam pacotes completos (com segurança online, backup, streaming, etc.) têm probabilidade drasticamente menor de cancelar.

---

## 🔮 Próximos Passos (Trabalhos Futuros)

* Implementar a técnica de **One-Hot Encoding** nas variáveis categóricas restantes.
* Treinar e testar algoritmos de *Machine Learning* (como **Random Forest**, **XGBoost** ou **Regressão Logística**) para prever a probabilidade de um cliente cancelar no próximo mês.
* Criar uma API para colocar o modelo de predição em produção.


*Desenvolvido com dedicação durante o desafio de Análise de Dados.*



## Autor:
### Mateus Rodrigues de Oliveira

## Agradecimentos
Aos dados de exemplo da TelecomX.
A todas as bibliotecas e ferramentas de código aberto que tornaram esta análise possível. E Alura Oracle One

## GIF do projeto
<p align="center">
  <img src="gif_do_projeto.gif" width="800">
</p>
