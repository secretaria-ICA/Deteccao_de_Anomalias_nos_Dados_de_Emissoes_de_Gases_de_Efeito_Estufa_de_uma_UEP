# Detecção de Anomalias nos Dados de Emissões de Gases de Efeito Estufa de uma UEP (Unidade Estacionária de Produção de Óleo e Gás)

#### Aluno: [Cláudio Orlando Bridi](https://github.com/cobridi).
#### Orientador: [Leonardo Forero Mendonza](https://github.com/leofome8).

---

Trabalho apresentado ao curso [BI MASTER](https://ica.puc-rio.ai/bi-master) como pré-requisito para conclusão de curso e obtenção de crédito na disciplina "Projetos de Sistemas Inteligentes de Apoio à Decisão".

- [Link para o código](deteção_anomalia_emissoes.ipynb).

---

### Resumo

Este trabalho implementou modelos estatísticos de processos, modelos autorregressivos e modelo CUSUM para detecção de anomalias em séries temporais de emissões de gases de efeito estufa por equipamentos de uma plataforma de petróleo. O mesmo foi elaborado a partir das seguintes etapas:
- Carregar, preparar e analisar dados
- Pré-Processar os dados
- Controle estatístico do processo (CEP) para detectar anomalias
- Modelos autorregressivos
- Avaliação dos modelos
- Conclusão final
    
#### Aplicabilidade:

Este algoritmo poderá ser utilizado na industria de óleo e gás, mais especificamente, e também para empresas que precisem registrar, inventariar, divulgar e trabalhar com dados de emissões de gases de efeito estufa. Para detecção e correção das anomalias em dados, na maioria das vezes inseridos manualmente em sistema ou planilha específica, também costumamente são verificados no olho por algum profissional todos o anos, antes de comporem as informações do inventário e relatório de emissões, divulgado tanto internamente quanto para stakeholders externos. Isto é, por serem muitos dados e de muitas fontes, anomalias podem passar despercebidas, prejudicando a análise de dados, atendimento de compromissos assumidos e perda de credibilidade.

#### Resultados:

O modelo detectou as duas anomalias inseridas bem como um outro registro (2017-07-01). O resultado reflete a diferença nos algoritmos de CUSUM e Tabela de Controle. A tabela de controle está procurando pontos únicos e anômalos. CUSUM é sensível a alterações no comportamento dos dados. Como resultado, sinaliza pontos como anômalos até que o comportamento da série temporal retorne ao normal. De fato, CUSUM é usado para detecção de pontos de mudança: encontrar quando a distribuição subjacente da série temporal mudou.

#### Conclusão:

Os modelos estudados (controle estatístico de processos, modelos autorregressivos e modelo CUSUM) detectaram possíveis anomalias bem como as anomalias implantadas para verificação, com melhor detecção pelo CUSUM. É possível utilizá-los para esta aplicação proposta, no entanto devemos trabalhar com o modelo para cada fonte de emissão e não para a Unidade Estacionária de Produção como um todo.

---

Matrícula: 192.190.107

Pontifícia Universidade Católica do Rio de Janeiro

Curso de Pós Graduação *Business Intelligence Master*
