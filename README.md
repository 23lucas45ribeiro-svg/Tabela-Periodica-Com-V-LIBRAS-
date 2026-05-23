# 🧪 Tabela Periódica Interativa e Acessível (com VLibras)

![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/tailwindcss-%2338B2AC.svg?style=for-the-badge&logo=tailwind-css&logoColor=white)
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)
![Acessibilidade](https://img.shields.io/badge/Acessibilidade-VLibras-blue.svg?style=for-the-badge)

Este é um projeto escolar de caráter inclusivo e interdisciplinar. Trata-se de uma **Tabela Periódica Interativa** projetada especificamente para ser acessível a pessoas com deficiência auditiva, integrando a ferramenta oficial **VLibras** para tradução de conteúdos textuais em tempo real para a Língua Brasileira de Sinais.

A aplicação permite a exploração dinâmica dos elementos químicos, fornecendo propriedades detalhadas de forma visualmente rica e totalmente adaptada.

---

## ♿ Foco em Acessibilidade e Recursos

- **Integração Nativa com VLibras**: O widget oficial do governo está acoplado no canto da tela, permitindo que usuários surdos traduzam as descrições dos elementos químicos instantaneamente.
- **Visualização Responsiva Inteligente**: O layout da tabela foi travado no CSS em uma largura mínima legível para evitar que a estrutura clássica de 18 colunas quebre ou fique incompreensível em dispositivos móveis, permitindo scroll horizontal suave no celular.
- **Suporte a Dark Mode**: Configuração de tema escuro integrada via Tailwind CSS para melhorar o conforto visual de usuários com fotossensibilidade ou preferências estéticas específicas.

---

## 🚀 Funcionalidades do Sistema

- **Exploração Dinâmica**: Ao passar o mouse (*hover*), as células dos elementos aumentam de tamanho discretamente em profundidade (`scale(1.1)`), indicando interatividade.
- **Modal de Detalhes Completo**: Ao clicar em um elemento, um modal centralizado é disparado revelando informações essenciais mapeadas diretamente de uma base estruturada:
  - Número Atômico
  - Nome e Símbolo do Elemento
  - Massa Atômica
  - Estado Físico (Gasoso, Líquido, Sólido ou Desconhecido)
  - Pontos de Fusão e Ebulição
  - Eletronegatividade
  - Descrição contextual detalhada da aplicação/curiosidade do elemento.
- **Identificação por Cores (Paleta Química)**: Classificação visual intuitiva dos elementos com base em suas famílias químicas (Metais Alcalinos, Alcalinoterrosos, Transição, Gases Nobres, Ametais, etc.).

---

## 🛠️ Estrutura Técnica do Código

O projeto foi dividido de maneira limpa entre estrutura, estilização e dados:

- **`index.html`**: Contém a malha estrutural do grid químico, as chamadas do script do VLibras e a estrutura semântica do modal.
- **`styles.css`**: Gerencia o algoritmo do grid (`grid-template-columns: repeat(18, minmax(60px, 1fr))`) e armazena as variáveis cromáticas exatas das categorias químicas.
- **`data.js`**: Funciona como a base de dados interna do projeto, estruturada em um array de objetos contendo dados científicos e descrições personalizadas para todos os elementos.
- **`script.js`**: Controla as interações de abertura/fechamento do modal, injeção dinâmica de dados no DOM, efeitos de animação e as configurações globais de estilo (Tailwind config).

---

## 🔧 Como Executar o Projeto

Como o software foi projetado usando arquitetura estática *Client-Side* com o Tailwind via CDN:

1. Clone este repositório:
   ```bash
   git clone [https://github.com/23lucas45ribeiro-svg/tabela-periodica-acessivel.git](https://github.com/23lucas45ribeiro-svg/tabela-periodica-acessivel.git)

2.Navegue até a pasta do projeto.

3.Abra o arquivo index.html em qualquer navegador moderno com conexão à internet (necessária para carregar os componentes do Tailwind e do VLibras).
