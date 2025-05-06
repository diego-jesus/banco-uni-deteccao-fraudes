# 🏦 Projeto Banco UNI: Detecção de Fraudes com SQL + IA

![Badge Projeto](https://img.shields.io/badge/SQL-BigQuery-blue)
![Status](https://img.shields.io/badge/status-em%20desenvolvimento-yellow)

## 🔎 1. Contexto do Problema

O aumento de fraudes em canais digitais exige uma análise mais profunda sobre comportamentos suspeitos dentro das transações. O projeto Banco UNI simula um ambiente realista de prevenção a fraudes com o objetivo de identificar padrões críticos e propor ações baseadas em dados.

## 💡 2. Hipóteses e Perguntas-Chave

* Dispositivos cadastrados recentemente têm maior associação com fraude?
* Existe um canal (app, web, caixa) com taxa de fraude mais alta?
* Há contrapartes (destinatários) que aparecem em múltiplas fraudes?
* O tempo de vida da conta influencia o risco?

## 🛠️ 3. Ferramentas e Técnicas Utilizadas

### 🔧 Arquitetura técnica do projeto

```
Usuário → Simulação de dados (ChatGPT + Python) 
       → Armazenamento no BigQuery (transacoes_analise + transacoes_expandido)
       → Análise via SQL (BigQuery UI)
       → Documentação técnica e insights no Notion
       → Versionamento e portfólio no GitHub
       → Visualização futura no Looker Studio (em construção)
```

Essa arquitetura permite um fluxo completo: da geração e análise de dados até a apresentação e documentação estratégica do projeto.

![Query executada 3](https://raw.githubusercontent.com/diego-jesus/banco-uni-deteccao-fraudes/main/img/arquitetura-projeto.png)

* SQL (BigQuery): JOINs, CTEs, subqueries, filtros temporais e de grupo
* IA (ChatGPT): estruturação de queries, geração de dados sintéticos, storytelling analítico
* Notion: organização de conhecimento e documentação do projeto

## 📊 4. Principais Descobertas

### Exemplo de análise de dispositivo (BigQuery)

![Query executada 1](https://raw.githubusercontent.com/diego-jesus/banco-uni-deteccao-fraudes/main/img/query-dispositivo1.png)

![Query executada 2](https://raw.githubusercontent.com/diego-jesus/banco-uni-deteccao-fraudes/main/img/query-dispositivo2.png)

* Canal app concentrou a maior parte das fraudes analisadas.
* Dispositivos com até 7 dias de cadastramento apresentaram taxa de fraude superior.
* Uma contraparte recebeu valores de múltiplos CPFs diferentes, com fraude confirmada.
* Contas com menos de 70 dias de abertura já registraram fraudes.

## 🎯 5. Próximos passos recomendados

A arquitetura proposta facilita a escalabilidade das análises e a automação dos próximos passos. O uso do BigQuery como base central permite consultas otimizadas e reutilizáveis; o Notion organiza o conhecimento e as descobertas; o GitHub garante versionamento do código e documentação pública; e a integração com Looker Studio permitirá criar dashboards visuais que podem ser atualizados automaticamente a partir das tabelas no BigQuery.

* Criar alerta para transações com dispositivos novos
* Analisar o risco por canal com regras de autenticação diferenciadas
* Monitorar contrapartes com múltiplos remetentes
* Desenvolver dashboards executivos com Looker Studio
* Criar alerta para transações com dispositivos novos
* Analisar o risco por canal com regras de autenticação diferenciadas
* Monitorar contrapartes com múltiplos remetentes
* Desenvolver dashboards executivos com Looker Studio

## ✅ 6. Conclusão

Projeto criado por \Diego Jesus, analista de prevenção a fraudes em transição para dados. Em construção constante.

---

## 👨‍💻 Sobre mim

Sou analista de prevenção a fraudes em transição para a área de dados. Esse projeto foi construído com base em desafios reais do meu dia a dia, usando SQL, IA (ChatGPT) e visualização de hipóteses de risco para gerar valor prático ao negócio.

📬 [Conecte-se comigo no LinkedIn](https://www.linkedin.com/in/diego-jesus-317302178/)
