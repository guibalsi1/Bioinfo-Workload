# Trabalho 01 - Alinhamento de Sequências

## Abordagem e técnicas utilizadas

Foi utilizado o código do @pshwetank que pode ser conferido aqui no [GitHub](https://github.com/pshwetank/BLAST-Python), além da base de dados da GEO (cod. AF117241.1) do vírus _Influenza_ (A/South Carolina/1/18) da hemaglutinina.

## Descrição dos Arquivos

- **hsp.py**: Arquivo principal com o código.
- **word.py**: Arquivo que implementa apenas a parte de fragmentação em w-mers.
- **query.txt**: Arquivo contendo uma sequência de exemplo do genoma da *H5N1*.
- **assembly.txt**: Arquivo contendo uma sequência de banco de dados de uma parte do genoma da *H5N1*. Como esse algoritmo tem complexidade de tempo O(n²), não é viável realizar uma busca completa em um banco de dados genômico em computadores pessoais.
