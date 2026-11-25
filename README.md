# 🌐 Portfólio Pessoal — Nilton Alves

## 📌 Sobre o Projeto

Este projeto consiste no desenvolvimento de um portfólio pessoal e profissional, criado com o objetivo de apresentar minha trajetória acadêmica, experiência profissional, rotina, interesses pessoais e projetos desenvolvidos durante minha formação em Engenharia de Software.

O portfólio foi desenvolvido utilizando **HTML5, CSS3 e JavaScript**, aplicando conceitos fundamentais de desenvolvimento Front-End, organização de código, responsividade, acessibilidade e interação com o usuário.

Além de apresentar informações pessoais e acadêmicas, o site funciona como uma vitrine profissional, permitindo que visitantes conheçam meus projetos e entrem em contato comigo.

## 🎯 Objetivos

- Apresentar minha trajetória acadêmica e profissional.
- Compartilhar projetos desenvolvidos durante a faculdade.
- Demonstrar conhecimentos em desenvolvimento Front-End.
- Aplicar conceitos de HTML, CSS e JavaScript.
- Desenvolver uma interface moderna, responsiva e acessível.
- Criar um espaço de apresentação para futuras oportunidades profissionais.

---

## 🛠️ Tecnologias Utilizadas

### HTML5 — Estrutura do Site

O HTML (HyperText Markup Language) é responsável por estruturar e organizar todo o conteúdo apresentado no portfólio.

Neste projeto, o HTML define os elementos que compõem cada seção da página, como textos, imagens, títulos, links, botões e cartões de apresentação.

Entre os principais elementos utilizados estão:

| Elemento | Função |
|---|---|
| `<header>` | Define o cabeçalho e a área de navegação. |
| `<nav>` | Organiza os links do menu principal. |
| `<main>` | Representa o conteúdo principal da página. |
| `<section>` | Divide o conteúdo em seções temáticas. |
| `<article>` | Organiza conteúdos independentes, como cartões de projetos. |
| `<h1>` até `<h4>` | Definem títulos e subtítulos. |
| `<p>` | Apresenta textos e descrições. |
| `<img>` | Exibe imagens do portfólio. |
| `<a>` | Cria links internos e externos. |
| `<button>` | Permite ações interativas, como alternar o tema. |
| `<footer>` | Define o rodapé da página. |

### Organização das Seções HTML

O conteúdo principal foi dividido em diferentes seções:

- **Home:** apresentação inicial e acesso ao GitHub.
- **Sobre mim:** informações pessoais e trajetória.
- **Minha Rotina:** apresentação de hábitos e interesses.
- **Formação Acadêmica & Projetos:** informações sobre a faculdade e projetos desenvolvidos.
- **Experiência Profissional:** apresentação da experiência no mercado de trabalho.
- **Contato:** links para comunicação e redes profissionais.

Essa organização facilita a navegação e permite que o visitante encontre rapidamente as informações desejadas.

### HTML Semântico

O projeto utiliza elementos semânticos, como `<header>`, `<main>`, `<section>`, `<article>` e `<footer>`.

Esses elementos ajudam a identificar a finalidade de cada parte da página, tornando o código mais organizado e facilitando sua interpretação por navegadores, mecanismos de busca e tecnologias assistivas.

Também foram utilizados atributos como:

- `alt`: descreve imagens para leitores de tela.
- `aria-label`: fornece informações adicionais sobre elementos interativos.
- `aria-labelledby`: relaciona uma seção ao seu título.
- `aria-expanded`: informa se o menu mobile está aberto ou fechado.
- `loading="lazy"`: permite carregar determinadas imagens somente quando necessário.

---

### CSS3 — Estilização e Layout

O CSS (Cascading Style Sheets) é responsável pela aparência visual do portfólio.

Enquanto o HTML define a estrutura e o conteúdo, o CSS controla cores, fontes, espaçamentos, tamanhos, alinhamentos, efeitos visuais e adaptação da interface para diferentes dispositivos.

#### 1. Variáveis CSS

O projeto utiliza variáveis personalizadas para armazenar valores de cores, bordas, sombras e transições.

Exemplo:

```css
:root {
  --bg: #0d1117;
  --text: #e6edf3;
  --accent: #58a6ff;
  --border: #30363d;
  --radius: 12px;
}
```

Essas variáveis facilitam a manutenção do código, pois permitem modificar características visuais em diferentes partes do site sem precisar alterar cada propriedade individualmente.

#### 2. Reset e Estilização Base

O CSS possui uma configuração inicial que remove margens e espaçamentos padrão dos elementos.

```css
*, *::before, *::after {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
```

Essa configuração ajuda a manter um comportamento mais consistente entre os elementos da página.

Também são definidos estilos gerais para o corpo do documento, imagens, fontes, cores e comportamento de rolagem.

#### 3. Layout com Flexbox e CSS Grid

O projeto utiliza dois recursos importantes para organizar os elementos:

**Flexbox**

Utilizado em áreas como:

- Barra de navegação.
- Botões de apresentação.
- Cartões de formação acadêmica.
- Cabeçalhos de experiência profissional.
- Links de contato.

**CSS Grid**

Utilizado principalmente para organizar:

- Seção inicial do portfólio.
- Cartões da rotina.
- Cartões dos projetos acadêmicos.

Esses recursos permitem distribuir os elementos de maneira organizada e adaptável.

#### 4. Cards e Efeitos Visuais

O CSS estiliza os cartões de apresentação, projetos, rotina, formação e experiência profissional.

Os cartões possuem características como:

- Bordas arredondadas.
- Espaçamento interno.
- Cores de fundo.
- Bordas personalizadas.
- Sombras.
- Efeitos de hover.

Os efeitos de `hover` permitem que alguns elementos mudem de aparência quando o usuário passa o cursor sobre eles.

#### 5. Responsividade

O portfólio utiliza Media Queries para adaptar sua estrutura a diferentes tamanhos de tela.

```css
@media (max-width: 700px) {
  .menu-toggle {
    display: grid;
  }
}
```

As Media Queries permitem modificar o layout conforme a largura da tela, proporcionando uma experiência adequada em computadores, tablets e smartphones.

No projeto, elas são utilizadas para:

- Transformar a navegação em um menu mobile.
- Alterar a disposição da apresentação inicial.
- Organizar os cartões em uma única coluna.
- Ajustar espaçamentos e tamanhos.
- Melhorar a visualização em dispositivos menores.

#### 6. Acessibilidade e Animações

O CSS também inclui recursos voltados à acessibilidade.

A propriedade `:focus-visible` destaca elementos que recebem foco durante a navegação por teclado.

Além disso, a regra `prefers-reduced-motion` reduz as animações para usuários que configuraram o sistema operacional para minimizar movimentos na interface.

---

### JavaScript — Interatividade e Funcionalidades

O JavaScript é responsável por adicionar comportamentos dinâmicos ao portfólio.

Diferentemente do HTML, que estrutura o conteúdo, e do CSS, que define sua aparência, o JavaScript permite que a página responda às ações do usuário.

O arquivo `script.js` foi organizado em funções e eventos responsáveis por diferentes funcionalidades.

#### 1. Atualização Automática do Ano

O JavaScript identifica o elemento `year` no rodapé e insere automaticamente o ano atual.

```javascript
document.getElementById('year').textContent =
  new Date().getFullYear();
```

Isso evita a necessidade de atualizar manualmente o ano do copyright.

#### 2. Gerenciamento de Tema Claro e Escuro

O portfólio possui um botão que permite alternar entre os temas claro e escuro.

O JavaScript utiliza:

- `localStorage`: armazena a preferência de tema do usuário.
- `getPreferredTheme()`: identifica o tema salvo ou o tema preferido do sistema.
- `applyTheme()`: aplica o tema selecionado à página.
- `addEventListener()`: identifica o clique no botão de alternância.

A preferência é salva no navegador, permitindo que o tema escolhido seja mantido durante visitas futuras.

Caso o usuário não tenha escolhido um tema manualmente, o site utiliza a preferência configurada no sistema operacional.

#### 3. Menu Responsivo para Dispositivos Móveis

O JavaScript controla a abertura e o fechamento do menu mobile.

A função `closeMenu()`:

- Remove a classe `open` do menu.
- Atualiza o atributo `aria-expanded`.
- Altera o ícone do botão.
- Atualiza o texto acessível do botão.

O evento de clique permite abrir ou fechar o menu.

Além disso, o menu é fechado automaticamente quando:

- O usuário seleciona um link de navegação.
- O usuário clica fora da área do menu.

Essa funcionalidade melhora a experiência de navegação em dispositivos com telas menores.

#### 4. Rolagem Suave com Foco

O JavaScript identifica links internos que apontam para seções da página.

Quando o usuário seleciona um desses links, o código utiliza:

```javascript
target.scrollIntoView({
  behavior: 'smooth',
  block: 'start'
});
```

Esse recurso realiza uma rolagem suave até a seção desejada.

O código também adiciona temporariamente o atributo `tabindex="-1"` ao elemento de destino, permitindo que ele receba foco.

Essa implementação contribui para a acessibilidade, especialmente para pessoas que navegam utilizando teclado ou tecnologias assistivas.

#### 5. Animações de Entrada

O portfólio possui animações que fazem determinados elementos aparecerem gradualmente durante a rolagem.

Para isso, o JavaScript utiliza a API `IntersectionObserver`.

Essa API permite identificar quando elementos entram na área visível da página.

Quando um elemento aparece na tela, o código modifica suas propriedades de opacidade e posição, criando um efeito de entrada suave.

Após a animação, o elemento deixa de ser observado, evitando processamento desnecessário.

A animação também respeita a configuração `prefers-reduced-motion`, reduzindo movimentos para usuários que preferem uma experiência com menos animações.

---

## 📁 Estrutura do Projeto

A estrutura recomendada para organizar os arquivos do portfólio é:

```text
portfolio/
│
├── index.html
├── style.css
├── script.js
│
└── IMG/
    ├── ft_perfil.jpeg
    ├── Livro.jpeg
    ├── jogo.jpeg
    ├── assistir.jpeg
    ├── estudando.jpeg
    ├── igreja.jpeg
    └── amigos.jpeg
```

### Descrição dos Arquivos

| Arquivo | Responsabilidade |
|---|---|
| `index.html` | Estrutura e conteúdo do portfólio. |
| `style.css` | Estilização, layout, cores e responsividade. |
| `script.js` | Funcionalidades interativas e comportamento dinâmico. |
| `IMG/` | Armazena as imagens utilizadas no site. |

---

## 🚀 Como Executar o Projeto

Para visualizar o portfólio localmente:

1. Faça o download ou clone o repositório.
2. Abra a pasta do projeto.
3. Certifique-se de que os arquivos HTML, CSS, JavaScript e imagens estejam organizados corretamente.
4. Abra o arquivo `index.html` em um navegador.

Também é possível utilizar extensões de desenvolvimento, como o **Live Server** do Visual Studio Code, para visualizar o site durante a edição.

## 📚 Conceitos Aplicados

Durante o desenvolvimento do projeto, foram aplicados conceitos importantes de desenvolvimento Front-End:

- HTML semântico.
- Organização estrutural de páginas.
- Seletores e propriedades CSS.
- Variáveis CSS.
- Flexbox e CSS Grid.
- Media Queries.
- Manipulação do DOM.
- Eventos JavaScript.
- Funções.
- Armazenamento local com `localStorage`.
- API `IntersectionObserver`.
- Acessibilidade digital.
- Design responsivo.

## 👨‍💻 Desenvolvedor

**Nilton Alves**

Estudante de Engenharia de Software na UDF, interessado em tecnologia, desenvolvimento de software e aprimoramento contínuo de conhecimentos em programação.

O portfólio representa uma etapa da minha trajetória acadêmica e profissional, reunindo experiências, aprendizados e projetos desenvolvidos ao longo da minha formação.

---

*Desenvolvido com HTML5, CSS3 e JavaScript.*
