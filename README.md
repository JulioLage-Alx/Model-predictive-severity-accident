# Projeto de Análise de Dados e Criação de Modelo de Previsão

Bem-vindo ao projeto de Análise de Dados e Criação de Modelo de Previsão! Este repositório contém todo o código, dados e documentação necessários para entender, executar e expandir as análises e previsões realizadas.

## Sumário

- [Descrição](#descrição)
- [Estrutura do Projeto](#estrutura-do-projeto)
- [Instalação](#instalação)
- [Uso](#uso)
- [Dados](#dados)
- [Modelos](#modelos)
- [Contribuição](#contribuição)
- [Licença](#licença)

## Descrição

Este projeto foi desenvolvido para analisar um conjunto de dados específico e construir um modelo preditivo baseado nesses dados. O objetivo é fornecer insights úteis e previsões que possam ajudar na tomada de decisões.

## Estrutura do Projeto

A estrutura de diretórios do projeto é a seguinte:

```
.
├── data
│   ├── raw                # Dados brutos não processados
│   ├── processed          # Dados processados e prontos para análise
├── notebooks              # Notebooks Jupyter para análise exploratória
├── scripts
│   ├── data_processing.py # Script para processamento de dados
│   ├── model_training.py  # Script para treinamento do modelo
│   ├── model_evaluation.py# Script para avaliação do modelo
├── models                 # Modelos treinados e suas versões
├── results                # Resultados de análises e previsões
├── requirements.txt       # Dependências do projeto
└── README.md              # Documentação do projeto
```

## Instalação

Para instalar e executar este projeto localmente, siga os passos abaixo:

1. Clone o repositório:
   ```bash
   git clone https://github.com/JulioLage-Alx/Model-predictive-severity-accident
   ```

2. Navegue até o diretório do projeto:
   ```bash
   cd Model-predictive-severity-accident
   ```

3. Crie um ambiente virtual:
   ```bash
   python -m venv venv
   ```

4. Ative o ambiente virtual:
   - No Windows:
     ```bash
     venv\Scripts\activate
     ```
   - No Unix ou MacOS:
     ```bash
     source venv/bin/activate
     ```

5. Instale as dependências:
   ```bash
   pip install -r requirements.txt
   ```

## Uso

### Processamento de Dados

Para processar os dados brutos, utilize o script `data_processing.py`:

```bash
python scripts/data_processing.py
```

### Treinamento do Modelo

Para treinar o modelo, utilize o script `model_training.py`:

```bash
python scripts/model_training.py
```

### Avaliação do Modelo

Para avaliar o desempenho do modelo, utilize o script `model_evaluation.py`:

```bash
python scripts/model_evaluation.py
```

### Notebooks Jupyter

Você também pode explorar os dados e executar análises nos notebooks Jupyter disponíveis na pasta `notebooks`. Para iniciar o Jupyter Notebook, utilize:

```bash
jupyter notebook
```

## Dados

Os dados utilizados neste projeto estão localizados na pasta `data`. Os dados brutos devem ser colocados na pasta `raw`, enquanto os dados processados estarão na pasta `processed` após a execução dos scripts de processamento.

## Modelos

Os modelos treinados são salvos na pasta `models`. Cada modelo é versionado e armazenado para possíveis comparações e melhorias futuras.

## Contribuição

Contribuições são bem-vindas! Se você deseja contribuir com este projeto, por favor, siga os passos abaixo:

1. Faça um fork deste repositório.
2. Crie uma branch para sua feature ou correção de bug (`git checkout -b feature/nova-feature`).
3. Commit suas alterações (`git commit -m 'Adiciona nova feature'`).
4. Envie para o branch (`git push origin feature/nova-feature`).
5. Abra um Pull Request.

## Licença

Este projeto está licenciado sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

---

Esperamos que este projeto seja útil e que você possa aprender e contribuir com ele. Se você tiver alguma dúvida, sinta-se à vontade para abrir uma issue ou entrar em contato.

Boas análises e boas previsões!



# DICIONARIO DE DADOS

## Descrição:
Este conjunto de dados abrangente fornece informações detalhadas sobre acidentes rodoviários comunicados ao longo de vários anos. O conjunto de dados engloba vários atributos relacionados ao status do acidente, referências de veículos e vítimas, demografia e gravidade das vítimas. Ele inclui fatores essenciais, como detalhes do pedestre, tipos de vítimas, envolvimento do trabalhador de manutenção de estradas e o decil do Índice de Privação Múltipla (IMD) para as áreas de residência das vítimas.

# Colunas:

**Status**: O status do acidente (por exemplo, relatado, sob investigação)

**Accident_Index**: Um identificador exclusivo para cada acidente relatado

**Accident_Year**: O ano em que ocorreu o acidente

**Accident_Reference**: Um número de referência associado ao acidente

**Vehicle_Reference**: Um número de referência para o veículo envolvido no acidente

**Casualty_Reference**: Um número de referência para a vítima envolvida no acidente

**Casualty_Class**: Indica a classe da vítima (por exemplo, motorista, passageiro, pedestre)

**Sex_of_Casualty**: O sexo da vítima (masculino ou feminino)

**Age_of_Casualty**: A idade da vítima

**Age_Band_of_Casualty**: Faixa etária à qual a vítima pertence (por exemplo, 0-5, 6-10, 11-15)

**Casualty_Severity**: A gravidade dos ferimentos da vítima (por exemplo, fatal, grave, leve)

**Pedestrian_Location**: A localização do pedestre no momento do acidente

**Pedestrian_Movement**: O movimento do pedestre durante o acidente

**Car_Passenger**: Indica se a vítima era passageira de carro no momento do acidente (sim ou não)

**Bus_or_Coach_Passenger**: Indica se a vítima foi passageira de ônibus (sim ou não)

**Pedestrian_Road_Maintenance_Worker**: Indica se o acidentado foi um trabalhador de manutenção de estradas (sim ou não)

**Casualty_Type**: O tipo de vítima (por exemplo, motorista/motociclista, passageiro, pedestre)

**Casualty_Home_Area_Type**: O tipo de área em que a vítima reside (por exemplo, urbana, rural)

**Casualty_IMD_Decile**: O decil IMD da área onde a vítima reside (uma medida de privação)

**LSOA_of_Casualty**: A Área de Super Saída de Camada Inferior (LSOA) associada à localização da vítima

> [!NOTE]
>Este conjunto de dados fornece informações valiosas para analisar acidentes rodoviários, identificar tendências e implementar medidas de segurança para reduzir vítimas e melhorar a segurança rodoviária. Pesquisadores, formuladores de políticas e analistas podem aproveitar esse conjunto de dados para a tomada de decisões baseadas em evidências e melhorar os sistemas gerais de transporte rodoviário.