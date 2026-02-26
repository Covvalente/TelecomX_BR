# 📊 Análise de Churn em Empresa de Telecomunicações

## Descrição do Projeto
Este projeto consiste em uma análise detalhada dos fatores que influenciam a evasão de clientes (também conhecida como Churn) em uma empresa de telecomunicações. O objetivo principal é identificar padrões e características que diferenciam os clientes que permanecem fiéis dos que optam por cancelar seus serviços. Através da exploração, limpeza e tratamento de dados, bem como da aplicação de técnicas de visualização, buscamos fornecer insights acionáveis para o desenvolvimento de estratégias de retenção eficazes.

## Problema de Negócio
O churn de clientes representa um desafio significativo para empresas de telecomunicações. A perda constante de clientes impacta diretamente a receita, a base de usuários e a competitividade no mercado. A compreensão dos motivos que levam os clientes a evadir é crucial para que a empresa possa intervir proativamente, otimizando a experiência do cliente e maximizando o valor de vida útil do cliente (CLV - Customer Lifetime Value).

## Dados
Os dados utilizados neste projeto foram extraídos de uma base de clientes de uma empresa de telecomunicações, em formato JSON. O dataset contém informações detalhadas sobre:

customerID: Identificador único do cliente.
Churn: Variável alvo, indicando se o cliente evadiu ('Yes' ou 'No').
customer: Informações demográficas (gênero, idade, parceiro, dependentes, tempo de serviço).
phone: Detalhes do serviço telefônico (serviço de telefone, múltiplas linhas).
internet: Detalhes do serviço de internet (tipo de serviço, segurança online, backup online, proteção de aparelho, suporte técnico, streaming de TV, streaming de filmes).
account: Informações da conta (tipo de contrato, fatura online, método de pagamento, cobrança mensal, cobrança total).

## Etapas do Projeto
### 1. Extração de Dados
Os dados foram carregados diretamente de um repositório GitHub, utilizando pandas.read_json().

### 2. Limpeza e Tratamento de Dados
Expansão de Colunas Aninhadas: As colunas com dados aninhados (dicionários) foram "aplanadas" para converter cada atributo em uma coluna independente.
Tratamento da Coluna 'Charges': Valores não numéricos foram convertidos para NaN e preenchidos com 0.0, garantindo a integridade dos dados financeiros.
Criação de Features: Novas features, como CobrancaDiaria e TotalGasto foram criadas para enriquecer a análise.
Renomeação de Colunas: Colunas foram renomeadas para facilitar a compreensão e padronização (ex: tenure para MesesServico, Churn para Evasao).
Codificação de Variáveis: Variáveis categóricas binárias foram convertidas para representação numérica (0 e 1) para viabilizar análises quantitativas.
### 3. Análise Exploratória de Dados (EDA)
Foram realizadas análises descritivas e visualizações para identificar padrões de churn. As principais observações incluem:

Distribuição Geral do Churn: Identificação da proporção de clientes que evadiram vs. os que permaneceram.
Análise por Variáveis Categóricas: Exploração da taxa de churn por gênero, tipo de contrato, método de pagamento e tipo de serviço de internet, utilizando gráficos de barras e torta.
Análise por Variáveis Numéricas: Exame da relação entre churn e tempo de serviço (MesesServico), cobrança mensal (CobrancaMensal) e total gasto (TotalGasto), através de boxplots.
Análise de Correlação: Utilização de heatmap para visualizar a correlação entre as variáveis numéricas e o churn.
### 4. Conclusões e Recomendações
Com base na EDA, foram elaboradas conclusões detalhadas sobre os principais impulsionadores do churn, acompanhadas de recomendações estratégicas e acionáveis, formuladas seguindo os critérios SMART (Specific, Measurable, Achievable, Relevant, Time-bound), para ajudar a empresa a mitigar o problema de evasão.

## Como Executar o Projeto
Pré-requisitos
Certifique-se de ter as seguintes bibliotecas Python instaladas:

pandas
matplotlib
seaborn
numpy
Você pode instalá-las usando pip:

pip install pandas matplotlib seaborn numpy
Passos para Execução
Clonar o Repositório:

git clone [Link do seu repositório GitHub, se aplicável]
cd [nome-do-seu-repositorio]
Abrir no Google Colab ou Ambiente Jupyter:

Faça o upload do arquivo .ipynb para o Google Colab ou abra-o em um ambiente Jupyter (Jupyter Notebook/Lab).
Executar as Células:

Execute as células do notebook sequencialmente. O notebook está estruturado para carregar, processar, analisar e visualizar os dados em uma ordem lógica.
Contribuições
Contribuições são bem-vindas! Se você tiver sugestões de melhoria, novas análises ou correções, sinta-se à vontade para:

Fazer um fork do projeto.
Criar uma nova branch (git checkout -b feature/AmazingFeature).
Commita suas alterações (git commit -m 'Add some AmazingFeature').
Fazer um push para a branch (git push origin feature/AmazingFeature).
Abrir um Pull Request.
Licença
Este projeto está licenciado sob a Licença MIT - veja o arquivo LICENSE.md para detalhes.

## Autor:
### Mateus Rodrigues de Oliveira

## Agradecimentos
Aos dados de exemplo da TelecomX.
A todas as bibliotecas e ferramentas de código aberto que tornaram esta análise possível. E Alura Oracle One

## GIF do projeto
<p align="center">
  <img src="gif_do_projeto.gif" width="800">
</p>
