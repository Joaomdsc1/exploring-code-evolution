# Explorando evolução de código

Neste exercício, iremos explorar a evolução de código em sistemas reais.

Iremos utilizar a ferramenta [GitEvo](https://github.com/andrehora/gitevo).
Essa ferramenta analisa a evolução de código em repositórios Git nas seguintes linguagens: Python, JavaScript, TypeScript e Java.

Você deve submeter via Moodle apenas o link do seu `fork`, conforme descrito abaixo.

# Passo 1: Selecionar repositório a ser analisado

Selecione um repositório relevante na linguagem de sua preferência (Python, JavaScript, TypeScript ou Java).
Você pode encontrar projetos interessantes nos links abaixo:

- Python: https://github.com/topics/python?l=python
- JavaScript: https://github.com/topics/javascript?l=javascript
- TypeScript: https://github.com/topics/typescript?l=typescript
- Java: https://github.com/topics/java?l=java

# Passo 2: Instalar e rodar a ferramenta GitEvo

Instale a ferramenta [GitEvo](https://github.com/andrehora/gitevo) com o comando:

```
pip install gitevo
```

Rode a ferramenta no repositório selecionado através do seguinte comando (dependendo da linguagem do projeto que escolheu):

```shell
# Python
$ gitevo -r python <git_url>

# JavaScript
$ gitevo -r js <git_url>

# TypeScript
$ gitevo -r ts <git_url>

# Java
$ gitevo -r java <git_url>
```

Onde `<git_url>` é URL do repositório a ser analisado.
Por exemplo, para analisar o projeto Flask escrito em Python:

```
$ gitevo -r python https://github.com/pallets/flask
```

# Passo 3: Explorar os gráficos de evolução de código (`index.html`)

Ao rodar a ferramenta [GitEvo](https://github.com/andrehora/gitevo), o arquivo `index.html` é gerado com diversos gráficos de evolução de código.

Abra o arquivo `index.html` e observe com atenção os gráficos gerados.

# Passo 4: Explicar um gráfico de evolução de código

Selecione um dos gráficos de evolução e explique-o com suas palavras.
Por exemplo, você pode:

- Detalhar a evolução ao longo do tempo, 
- Detalhar se as curvas estão de acordo com boas práticas,
- Explicar grandes alterações nas curvas,
- Explorar a documentação do repositório em busca de explicações para grandes alterações
- Etc.

Seja criativo!

# Exercício

Para responder este exercício, primeiramente, você deve fazer um `fork` deste repositório.
No Moodle, você deve submeter apenas a URL do seu `fork`.

Em seguida, adicione o arquivo gerado `index.html` no seu fork.

Por fim, responda as questões abaixo no seu `fork`: 

1. Repositório selecionado: [https://github.com/fastapi/fastapi](https://github.com/fastapi/fastapi)

2. Gráfico selecionado: Lines of code (LOC)
  
3. Explicação: 
O gráfico de LOC mostra uma evolução expressiva da base de código do FastAPI ao longo dos anos, partindo de 26.591 linhas em 2020 para 113.778 em 2025. Essa curva crescente indica uma expansão significativa da funcionalidade e da complexidade do projeto.

Entre 2023 e 2024, houve o maior salto, com um aumento de aproximadamente 81% nas linhas de código (de 60.374 para 109.466). Esse crescimento pode estar relacionado a grandes mudanças no core do framework, adição de novas funcionalidades ou refatorações estruturais. De fato, ao analisar os releases do repositório, nota-se que o projeto teve várias atualizações importantes nesse período, incluindo melhorias de compatibilidade com novas versões do Python e extensões no sistema de validação.

Apesar do aumento acelerado, não há evidência de redução de código (refatorações para simplificação), o que pode indicar crescimento contínuo sem foco claro em redução técnica de dívida. Essa tendência deve ser observada com atenção, pois o acúmulo de LOC pode dificultar a manutenção futura se não for acompanhado por boas práticas de modularização e testes.

Em resumo, o gráfico mostra um projeto em crescimento ativo, com picos que coincidem com marcos importantes de desenvolvimento, refletindo uma comunidade engajada e uma evolução constante da base de código.



