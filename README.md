![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)

# Web Scraper de Diário Oficial

## Descrição do Projeto

Este projeto é um web scraper automatizado desenvolvido em Python para extrair informações do Diário Oficial do Estado de Alagoas. O script busca dados de clientes com base em códigos CACEAL e um intervalo de datas especificado pelo usuário, armazenando os resultados em arquivos Excel.

## Funcionalidades Principais

- Busca automatizada no site do Diário Oficial usando códigos CACEAL
- Armazenamento de resultados em arquivos Excel (formato .xlsx)
- Interface de linha de comando para inserção do período de busca
- Geração de relatórios detalhados usando Pandas e Openpyxl
- Barra de progresso para acompanhamento da execução

## Tecnologias Utilizadas

- **Python** - Linguagem principal do projeto
- **Selenium** - Automação de navegação e extração web
- **Pandas** - Manipulação e exportação de dados
- **Openpyxl** - Manipulação de planilhas Excel
- **Tqdm** - Exibição de barra de progresso
- **webdriver_manager** - Gerenciamento automático do ChromeDriver

## Pré-requisitos

- Python 3.x instalado
- Google Chrome instalado e atualizado
- Arquivo `clientes_caceal.xlsx` com as colunas:
  - `caceal` (códigos CACEAL)
  - `Razao_social` (nomes dos clientes)

## Instalação

1. Clone este repositório:
   ```
   git clone [URL_DO_REPOSITORIO]
   ```

2. Instale as dependências:
   ```
   pip install selenium pandas openpyxl tqdm webdriver_manager
   ```

3. Prepare o arquivo de clientes:
   - Certifique-se que o arquivo `clientes_caceal.xlsx` está no mesmo diretório do script
   - Preencha com os códigos CACEAL e nomes dos clientes conforme o modelo

## Como Usar

1. Execute o script:
   ```
   python nome_do_script.py
   ```

2. Quando solicitado, insira:
   - Data inicial (formato DD/MM/AAAA)
   - Data final (formato DD/MM/AAAA)

3. Aguarde a execução:
   - O script mostrará uma barra de progresso
   - Os resultados serão salvos automaticamente

## Saída

Os arquivos gerados terão o formato:
```
dados_encontrados_dd-mm-YYYY.xlsx
```
Onde `dd-mm-YYYY` representa a data de execução do script.

## Observações Importantes

- Mantenha o Google Chrome atualizado
- O script foi desenvolvido para execução local
- Verifique periodicamente por atualizações que possam afetar o funcionamento do scraper

## Contribuição

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou enviar pull requests.

## Licença

[MIT](https://choosealicense.com/licenses/mit/)
