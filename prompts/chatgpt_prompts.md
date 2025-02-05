1️⃣ Primeiro Prompt:

Solicitei à IA que "criasse uma tabela de resumo de vendas por países e produtos".

🔹 Durante a análise, a IA identificou três arquivos com colunas semelhantes, contendo informações sobre produtos vendidos, países de entrega e valores.
🔹 Para obter um panorama consolidado, foi necessário realizar a consolidação dos dados, agrupando as vendas por país.

📜 Script de Pesquisa:
A seguir, apresento o script utilizado, detalhando os caminhos percorridos durante o processamento e a consolidação dos dados.
import pandas as pd

# Caminhos dos arquivos
files = {
    "AliExpress": "/mnt/data/Meganium_Sales_Data_-_AliExpress.csv",
    "Etsy": "/mnt/data/Meganium_Sales_Data_-_Etsy.csv",
    "Shopee": "/mnt/data/Meganium_Sales_Data_-_Shopee.csv",
}

# Carregar os arquivos para inspecionar as primeiras linhas
dataframes = {name: pd.read_csv(path) for name, path in files.items()}

# Exibir as primeiras linhas de cada arquivo
{key: df.head() for key, df in dataframes.items()}

#####################################################################
#####################################################################

2- "Qual a idade media por produto de cada país "
3- "Qual o produto mais vendido em cada país?"
