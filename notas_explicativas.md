## Notas Explicativas

* A API do IBGE foi consumida uma única vez e armazenada em memória para evitar múltiplas requisições.
* Foi utilizado tratamento de normalização de texto com remoção de acentos e padronização para lowercase.
* A correspondência aproximada de municípios foi realizada com difflib.get_close_matches.
* O município "Santoo Andre" foi tratado como NAO_ENCONTRADO para evitar falso positivo duplicado.
* O programa gera automaticamente o resultado.csv e calcula as estatísticas solicitadas.
* Os resultados foram enviados para a API de correção utilizando ACCESS_TOKEN JWT obtido via autenticação Supabase.
