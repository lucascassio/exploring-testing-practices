# Explorando Práticas de Teste

Neste exercício, vamos explorar práticas de teste em sistemas reais utilizando a ferramenta [TestMiner](https://andrehora.github.io/testminer).

O TestMiner permite visualizar e analisar testes de software em repositórios do GitHub, fornecendo dados sobre como os projetos organizam seus testes, como eles evoluem entre versões e quais bibliotecas de teste são utilizadas.
Explore a ferramenta antes de começar para se familiarizar com seu funcionamento.

---

## Passo 1: Selecionar um repositório

Escolha um repositório real que possua testes escritos na linguagem de sua preferência.
Abaixo estão alguns links para ajudá-lo a encontrar projetos interessantes:

- **Python:** https://github.com/topics/python?l=python
- **JavaScript:** https://github.com/topics/javascript?l=javascript
- **TypeScript:** https://github.com/topics/typescript?l=typescript
- **Java:** https://github.com/topics/java?l=java

## Passo 2: Explorar o repositório selecionado

Busque o repositório escolhido no [TestMiner](https://andrehora.github.io/testminer) e analise os dados de teste gerados pela ferramenta.

## Passo 3: Explicar uma prática de teste

Com base nos dados obtidos, selecione uma prática ou dado de teste relevante e explique-o com suas próprias palavras.

---

## Instruções de entrega

1. Faça um `fork` deste repositório (saiba mais sobre forks [aqui](https://docs.github.com/pt/pull-requests/collaborating-with-pull-requests/working-with-forks/fork-a-repo)).
2. Responda às questões abaixo diretamente neste arquivo `README.md` do seu fork. Pode adicionar imagens para enriquecer sua explicação.
3. No Moodle, submeta apenas a URL do seu fork.

---

## Respostas

**1. Repositório selecionado:** `https://github.com/vercel/next.js`

<img width="1572" height="1314" alt="image" src="https://github.com/user-attachments/assets/7393a19a-7404-46a6-8848-52c36d38c92a" />

**2. Explicação:** 

O repositório Next.js adota a prática de **testes em múltiplas camadas com separação clara entre tipos de teste**. Analisando através do TestMiner, observa-se que o projeto utiliza uma estratégia bem definida:

- **Testes unitários**: Focam em componentes e funções isoladas usando Jest, testando lógica pura sem dependências externas
- **Testes de integração**: Verificam interações entre múltiplos componentes e módulos, incluindo comportamento end-to-end com Playwright
- **Organização por diretórios**: Testes estão colocados próximos ao código fonte (padrão `__tests__/` ou `*.test.js`), facilitando manutenção

Uma prática particularmente relevante é o uso de **fixtures e mocks reutilizáveis**. O Next.js mantém um conjunto de cenários de teste padronizados que são aplicados consistentemente, reduzindo duplicação de código de teste e melhorando a cobertura. Além disso, o projeto usa **cobertura de teste controladas** para garantir que mudanças críticas sejam sempre testadas.

Essa abordagem garante confiabilidade em um projeto grande e complexo, permitindo que a equipe identifique regressões rapidamente e mantenha alta qualidade ao longo de múltiplas versões.


