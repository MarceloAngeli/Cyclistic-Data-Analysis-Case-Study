# Cyclistic-Data-Analysis-Case-Study

## Capstone do Certificado Profissional Google Data Analyst

### 1. Introdução

Este projeto é um estudo de caso realizado como o capstone para o Certificado Profissional Google Data Analyst. A análise foca nos dados de uso de compartilhamento de bicicletas de uma empresa fictícia, a Cyclistic, para entender as principais diferenças entre seus dois segmentos de clientes: ciclistas casuais e membros anuais. O objetivo final é fornecer recomendações baseadas em dados para uma campanha de marketing que visa converter ciclistas casuais em membros anuais, que são mais lucrativos.

### 2. A Tarefa de Negócio

A Diretora de Marketing encarregou a equipe de análise de dados de responder à seguinte questão principal: **"Como os membros anuais e os ciclistas casuais utilizam as bicicletas da Cyclistic de forma diferente?"**. Os insights derivados desta análise serão usados para moldar uma nova estratégia de marketing projetada para aumentar a taxa de conversão de ciclistas casuais para membros anuais, uma vez que as assinaturas anuais são significativamente mais lucrativas para a empresa.

### 3. Fonte de Dados

O conjunto de dados utilizado para esta análise são dados reais de viagem da empresa de compartilhamento de bicicletas Divvy, com sede em Chicago. Para o propósito deste estudo de caso, esses dados são tratados como se pertencessem à Cyclistic. O conjunto de dados abrange 12 meses, de julho de 2024 a junho de 2025, e contém informações sobre viagens individuais, incluindo horários de início/fim, locais das estações de início/fim, tipo de usuário e tipo de veículo.

* Os dados podem ser acessados [aqui](https://divvy-tripdata.s3.amazonaws.com/index.html).

### 4. Ferramentas Utilizadas

* **R & RStudio:** Para limpeza, transformação e análise dos dados.
* **Pacotes R:**
    * `tidyverse`: Para manipulação e tratamento geral de dados.
    * `ggplot2`: Para a criação de visualizações de dados.
    * `scales`: Para formatação das escalas das visualizações.

### 5. O Processo de Análise

A análise seguiu os seis passos do framework de análise de dados: **Perguntar, Preparar, Processar, Analisar, Compartilhar e Agir.**

1.  **Preparar:** Dados de 12 arquivos `.csv` separados (um para cada mês) foram coletados, avaliados quanto à consistência e unidos em um único dataframe abrangente.
2.  **Processar:** Os dados foram minuciosamente limpos para garantir sua integridade. Isso incluiu:
    * Criação de novas colunas para análise, como duração da viagem, mês e dia da semana.
    * Remoção de viagens com duração negativa ou zero.
    * Remoção de entradas duplicadas.
    * Validação de que as colunas categóricas continham apenas os valores esperados.
3.  **Analisar:** Os dados limpos foram analisados para identificar as principais tendências e diferenças entre os ciclistas casuais e os membros.
4.  **Compartilhar e Agir:** As principais descobertas foram visualizadas usando `ggplot2`, e um conjunto final de recomendações acionáveis foi desenvolvido com base nesses insights.

### 6. Principais Descobertas

A análise revelou várias diferenças comportamentais claras entre os dois segmentos de clientes:

* **Sazonalidade e Uso por Dia da Semana:**
    * Membros anuais usam o serviço de forma consistente ao longo do ano, com um ligeiro aumento no verão. O uso é maior durante os dias de semana, sugerindo um padrão de deslocamento para o trabalho.
    * Ciclistas casuais são altamente sazonais, com o uso atingindo um pico dramático nos meses quentes (junho a outubro). Eles preferem esmagadoramente andar nos fins de semana (sábados e domingos), indicando um uso recreativo.

* **Duração da Viagem:**
    * Ciclistas casuais fazem viagens significativamente mais longas em média, com aproximadamente 24 minutos por viagem.
    * Membros anuais fazem viagens mais curtas e diretas, com uma duração média de cerca de 13 minutos.

* **Preferência de Veículo:**
    * Ambos os grupos mostram uma forte preferência por bicicletas elétricas em detrimento das bicicletas clássicas.
    * A preferência por veículos elétricos é ainda mais pronunciada entre os ciclistas casuais.

### 7. Recomendações

Com base nas descobertas, as seguintes recomendações são propostas para a campanha de marketing:

1.  **Direcionar o Marketing para os Finais de Semana na Alta Temporada:** Concentrar os esforços de publicidade nos sábados e domingos entre a primavera e o verão (junho a novembro), quando os ciclistas casuais estão mais ativos.
2.  **Promover Benefícios para o Deslocamento Diário:** Criar campanhas que destaquem a economia e a conveniência de uma assinatura anual para o deslocamento diário, visando potenciais clientes durante os dias de semana.
3.  **Destacar Bicicletas Elétricas nos Anúncios:** Como as bicicletas elétricas são muito populares entre os ciclistas casuais, os materiais de marketing devem destacá-las para capturar seu interesse.

### 8. Conteúdo do Repositório

* **`Cyclistic_Estudo_de_Caso_Versao_Portuguesa.pdf`:** O relatório final e detalhado do estudo de caso, incluindo visualizações e a narrativa das descobertas.
* **`Cyclistic_Estudo_de_Caso_Versao_Portuguesa.Rmd`:** O R Markdown contendo todo o código usado para limpeza de dados, análise e visualização.
* **`README.pt.md`:** Este arquivo explicativo.
