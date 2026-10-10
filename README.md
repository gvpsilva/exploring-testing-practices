# Explorando Práticas de Teste

Neste exercício, vamos explorar práticas de teste em sistemas reais utilizando a ferramenta [TestMiner](https://andrehora.github.io/testminer).

O TestMiner permite visualizar e analisar testes de software em repositórios do GitHub, fornecendo dados sobre como os projetos organizam seus testes, como eles evoluem entre versões e quais bibliotecas de teste são utilizadas.
Explore a ferramenta antes de começar para se familiarizar com seu funcionamento.

Mais detalhes no GitHub da ferramenta: https://github.com/andrehora/testminer.

---

## Passo 1: Selecionar um repositório

Escolha um repositório real que possua testes de software.
Abaixo estão alguns links para ajudá-lo a encontrar projetos interessantes:

- Python: https://github.com/topics/python?l=python
- JavaScript: https://github.com/topics/javascript?l=javascript
- TypeScript: https://github.com/topics/typescript?l=typescript
- Java: https://github.com/topics/java?l=java

- Tópicos: [ai](https://andrehora.github.io/testminer/#topic:ai), [llm](https://andrehora.github.io/testminer/#topic:llm), [api](https://andrehora.github.io/testminer/#topic:api), [nodejs](https://andrehora.github.io/testminer/#topic:nodejs), [android](https://andrehora.github.io/testminer/#topic:android)

- Por organização: [Google](https://andrehora.github.io/testminer/#google), [Microsoft](https://andrehora.github.io/testminer/#microsoft), [Apple](https://andrehora.github.io/testminer/#apple), [Facebook](https://andrehora.github.io/testminer/#facebook), [Netflix](https://andrehora.github.io/testminer/#netflix), 
[GitHub](https://andrehora.github.io/testminer/#github), [Apache](https://andrehora.github.io/testminer/#apache), [HuggingFace](https://andrehora.github.io/testminer/#huggingface)

## Passo 2: Explorar o repositório selecionado

Busque o repositório escolhido no [TestMiner](https://andrehora.github.io/testminer) e analise os dados de teste gerados pela ferramenta.

## Passo 3: Explicar uma prática de teste

Escolha uma prática ou dado de teste relevante e explique com suas próprias palavras.

---

## Instruções de entrega

1. Faça um `fork` deste repositório (saiba mais sobre forks [aqui](https://docs.github.com/pt/pull-requests/collaborating-with-pull-requests/working-with-forks/fork-a-repo)).
2. Responda às questões abaixo diretamente neste arquivo `README.md` do seu fork. Pode adicionar imagens para enriquecer sua explicação.
3. No Moodle, submeta apenas a URL do seu fork.

---

## Respostas

Repositório: `https://github.com/spring-projects/spring-boot`

URL TestMiner: `https://andrehora.github.io/testminer/#spring-projects/spring-boot`

Explicação: <img width="2871" height="1289" alt="image" src="https://github.com/user-attachments/assets/c47b9ec6-fbac-4aac-80c5-553e33757094" />
Usando a ferramenta, selecionei o seguinte teste para analisar:
<img width="2123" height="1339" alt="image" src="https://github.com/user-attachments/assets/56158970-4cfc-4a1c-99b1-06f73de9b752" />
O código desse teste é pequeno, mas podemos fazer a seguinte análise:

<img width="1995" height="1603" alt="image" src="https://github.com/user-attachments/assets/ef3c380f-f826-4290-99a4-7c446f8ee9f5" />


É um teste unitário, utilizando o teste de caixa-preta baseada em especificação, ou seja isolando uma unidade de código e comparando sua saída com um oráculo de teste.
Está testando a integridade e a corretude do método  FileUtils.sha1Hash(...). 
O teste valida se o método lê corretamente o conteúdo físico de um arquivo em disco e calcula exatamente o hash criptográfico SHA-1 correspondente em formato hexadecimal.
