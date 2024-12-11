# Análisando o engajamento de um perfil no Instagram

## Contexto do Projeto
Este projeto foi desenvolvido com o objetivo de analisar o engajamento do perfil do Instagram de uma empresa, com base nos dados coletados desde o início das postagens até o dia 27 de março. A análise foca em identificar quais tipos de conteúdo geram maior interação com os seguidores e explorar o impacto das tags utilizadas nas publicações.

### Questões que Guiaram a Análise
1. **Qual tipo de conteúdo mais engaja no Instagram da empresa?**
2. **Quais tags mais contribuem para o engajamento das publicações?**

## Direcionamentos da Análise
Para responder às questões acima, foram seguidos os seguintes direcionamentos:

- **Dados Considerados:**
  - Curtidas, comentários e interações foram as métricas principais analisadas.
  - A coluna de visualizações foi ignorada, pois não estava no escopo da análise.

- **Tratamento de Dados:**
  - As publicações sem tags tiveram os valores tratados como "vazio" para manter a consistência na análise.
  
## Metodologia
1. **Coleta de Dados:**
   - Os dados foram extraídos do histórico de postagens no Instagram da empresa.
   
2. **Tratamento e Limpeza:**
   - As tags foram padronizadas, preenchendo campos vazios como "sem tag".
   - Os dados foram filtrados para excluir colunas e métricas não relevantes.

3. **Exploração de Dados:**
   - Foi realizada uma análise exploratória para identificar padrões de engajamento associados ao tipo de conteúdo e às tags utilizadas.

4. **Resultados Esperados:**
   - Identificar o formato de conteúdo que mais gera engajamento.
   - Determinar quais tags são mais eficazes para atrair curtidas, comentários e interações.

## Próximos Passos
Com base nos resultados desta análise, serão definidas estratégias de otimização para as publicações futuras no Instagram, priorizando os formatos e tags que demonstraram maior potencial de engajamento. 


## Organização do projeto

```

├── .gitignore         <- Arquivos e diretórios a serem ignorados pelo Git
├── ambiente.yml       <- O arquivo de requisitos para reproduzir o ambiente de análise
├── LICENSE            <- Licença de código aberto (MIT)
├── README.md          <- README principal para desenvolvedores que usam este projeto.
|
├── dados              <- Arquivos de dados para o projeto.
|
|
├── notebooks          <- Jupyter Notebooks. 
│                         
│
|   └──src             <- Código-fonte para uso neste projeto.
|      │
|      ├── __init__.py  <- Torna um módulo Python
|      ├── config.py    <- Configurações básicas do projeto
|      
|
├── referencias        <- Dicionários de dados
|
├── relatorios         <- Análises geradas em HTML, PDF, LaTeX, etc.
│   └── imagens        <- Gráficos e figuras gerados para serem usados em relatórios
```

## Configuração do ambiente

1. Faça o clone do repositório.

    ```bash
    git clone git@github.com:DanFalcari/Analisando_engajamento_de_um_perfil_do_Instagram.git
    ```

2. Crie um ambiente virtual para o seu projeto utilizando o `conda`.

   ```bash
        conda env create -f ambiente.yml -- name Instagram_engajamento
        conda env export > ambiente.yml
   ```
      