# Python unittest walkthrough

Fork das soluções do Code Institute com três etapas do mesmo exercício de teste de números pares.

[English](README.md)

## Registro do processo

Código revisado em 01/10/2026. O repositório registra um exercício, não um produto publicado. Não foram encontrados planejamento datado, pesquisa com usuários ou wireframes nos arquivos revisados. A arquitetura abaixo descreve o código existente, sem inventar um diário de desenvolvimento.

## Ideia, arquitetura e design

Cada pasta `testing_with_python_01/`, `_02/` e `_03/` contém evens.py e test_evens.py próprios. Etapa 01 é um esqueleto que retorna None, com classe de teste vazia. Etapa 02 conta usando loop; etapa 03 usa comprehension e sum. A sequência existe no material do curso, não comprova design original ou cronologia pessoal. Não há interface, banco ou deploy no diretório raiz revisado.

## Execução e testes

Execute uma etapa por vez para que `from evens import ...` importe o módulo correspondente:

```bash
cd testing_with_python_03
python3 evens.py
python3 -m unittest -v test_evens
```

Os arquivos não importam pacotes externos. Etapas 02 e 03 têm dois métodos de teste cada, cobrindo erro de não-lista, lista vazia, dois pares, um par e nenhum par. Etapa 01 não tem métodos de teste. A demonstração direta da etapa 02 passa 5 e gera o TypeError esperado; use seu comando de teste, sem esperar uma demonstração bem-sucedida. Testes não executados nesta atualização.

## Limites e próximos testes

Lista vazia ou zero pares retorna False; quantidade par e diferente de zero retorna True. Elementos não são validados antes do módulo. Teste tipos misturados, negativos, zero e booleans antes de reutilizar. Código de referência de curso, não uma afirmação de autoria original.

## Capturas

Não há interface de aplicação para capturar. Nenhuma imagem foi adicionada. Se evidência de terminal for útil, salve captura datada do comando e resultado real em `docs/assets/`, sem caminhos ou dados privados. Não invente dashboard ou resultado de testes.

## Créditos e licença

Fork de [Code-Institute-Solutions/unittest-python-testing](https://github.com/Code-Institute-Solutions/unittest-python-testing). Código original mantido. Nenhuma licença nova foi aplicada ao código de curso de terceiros.
