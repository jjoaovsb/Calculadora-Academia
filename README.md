# Calculadora de Índice de Massa Corporal (IMC)

Este repositório contém uma aplicação web de página única (SPA) para o cálculo do Índice de Massa Corporal (IMC). O projeto foca em uma interface de usuário responsiva e lógica de processamento em tempo real via JavaScript para auxiliar na avaliação rápida de categorias de peso com base nos parâmetros da Organização Mundial da Saúde (OMS).



## Especificações Técnicas

A aplicação foi desenvolvida utilizando tecnologias front-end fundamentais para garantir leveza e compatibilidade entre navegadores:

1. **HTML5:** Estruturação semântica da calculadora e dos campos de entrada.
2. **CSS3:** Estilização baseada em Flexbox para centralização dinâmica, aplicação de gradientes lineares e transições suaves de estado (hover e focus).
3. **JavaScript (ES6):** Implementação da lógica matemática para o cálculo e estruturas condicionais para a classificação dos resultados.

## Funcionalidades e Lógica de Cálculo

O sistema processa as informações inseridas pelo usuário seguindo as seguintes etapas:

* **Validação de Inputs:** O script verifica se os valores de peso e altura são positivos e se a altura está dentro de um intervalo humano plausível.
* **Processamento Matemático:** Utiliza a fórmula padrão:
  $$IMC = \frac{peso}{altura^2}$$
* **Classificação Dinâmica:** O resultado é categorizado automaticamente em:
    * Abaixo do peso (IMC < 18.5)
    * Peso normal (18.5 <= IMC < 24.9)
    * Sobrepeso (25 <= IMC < 29.9)
    * Obesidade (IMC >= 30)
* **Interface Responsiva:** O layout se adapta a diferentes dimensões de tela (viewport) utilizando unidades relativas e Box Model (border-box).

## Design e Experiência do Usuário (UX)

* **Tipografia:** Integração com Google Fonts (Poppins) para melhorar a legibilidade.
* **Feedback Visual:** Uso de sombras projetadas (box-shadow) e transformações de translação (translateY) para indicar interatividade nos elementos de input e botões.
* **Tratamento de Erros:** Exibição de mensagens de aviso caso o usuário insira caracteres inválidos ou campos vazios.

## Como Executar o Projeto

Por ser uma aplicação baseada inteiramente em tecnologias client-side, não é necessário um servidor de aplicação ou gerenciadores de pacotes.

1. Clone o repositório ou baixe o arquivo HTML.
2. Abra o arquivo `index.html` em qualquer navegador moderno.

## Estrutura do Arquivo

* **Head:** Definições de meta tags, títulos e importação de fontes externas.
* **Style:** Definições de CSS incorporadas para carregamento rápido.
* **Body:** Estrutura DOM da calculadora.
* **Script:** Lógica funcional isolada para facilitar a manutenção.
