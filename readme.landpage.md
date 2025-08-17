

# README - Landing Page Fabr

## Descrição

Landing page profissional para o projeto Fabr — Framework de Fabricação Compartilhada. Uma plataforma que conecta pessoas e habilidades para fabricar partes de projetos modulares, funcionando como um "GitHub" do mundo físico.

## Tecnologias Utilizadas

- HTML5 semântico
- CSS3 puro (com variáveis CSS, Grid, Flexbox e animações)
- JavaScript vanilla (ES6+)
- Sem frameworks ou bibliotecas externas
- Design responsivo (mobile-first)
- Modo claro/escuro com persistência no localStorage

## Estrutura de Arquivos

```
├── index.html       # Estrutura HTML semântica da landing page
├── styles.css       # Estilos CSS com variáveis e modo dark
├── app.js           # Funcionalidades JavaScript
└── README.md        # Este arquivo
```

## Funcionalidades

### 1. Design Responsivo
- Layout adaptável para diferentes tamanhos de tela
- Menu mobile com animação
- Grid e Flexbox para alinhamento responsivo

### 2. Modo Claro/Escuro
- Toggle de tema no header
- Persistência da preferência no localStorage
- Cores ajustadas via variáveis CSS

### 3. Seções Implementadas
- **Header fixo** com navegação âncora
- **Hero** com headline, subheadline e ilustração SVG
- **Como funciona** com cards numerados
- **Projetos em destaque** (renderizados dinamicamente via JS)
- **Match de Habilidades** com formulário validado
- **Reputação & Incentivos** com cards explicativos
- **Parceiros & Espaços Makers** com mapa interativo
- **Linha do Tempo** com animação ao scroll
- **Depoimentos** com carrossel automático
- **FAQ** com accordion
- **CTA final** com botão de destaque
- **Footer** com links e informações

### 4. Interações JavaScript
- Validação de formulário com feedback acessível
- Modal de sucesso após envio do formulário
- Carrossel de depoimentos com controles
- Accordion para FAQ
- Tooltips no mapa de parceiros
- Animações ao scroll com IntersectionObserver
- Banner de cookies com persistência

### 5. Acessibilidade
- Semântica HTML5 correta
- Atributos ARIA em componentes interativos
- Contraste de cores AA
- Navegação por teclado
- Foco visível
- Mensagens de erro acessíveis

### 6. Performance
- Nenhum recurso externo (CDNs)
- CSS minificado (versão comentada no final do arquivo)
- SVGs inline para ícones e ilustrações
- Lazy loading implícito para imagens
- Otimização para Core Web Vitals

## Como Executar

1. Clone ou baixe os arquivos do projeto
2. Abra o arquivo `index.html` em um navegador moderno
3. A landing page estará funcionando imediatamente

## Personalização

### Cores
As cores podem ser ajustadas através das variáveis CSS no início do arquivo `styles.css`:

```css
:root {
  --color-primary: #00a896;    /* Cor primária (ciano/esmeralda) */
  --color-secondary: #02c39a;  /* Cor secundária */
  --color-accent: #f0f3bd;     /* Cor de destaque */
  /* ... outras variáveis de cores */
}
```

### Projetos em Destaque
Os projetos são definidos no array `projetos` no arquivo `app.js`. Para adicionar ou modificar projetos:

```javascript
const projetos = [
  {
    id: "id-do-projeto",
    titulo: "Título do Projeto",
    modulos: ["Módulo 1", "Módulo 2"],
    status: "Status",
    prazo: "X semanas",
    dificuldade: "Nível",
    vagas: N,
    descricao: "Descrição do projeto",
    cta: "Texto do botão"
  },
  // ... outros projetos
];
```

### Conteúdo Textual
Todo o conteúdo está em português brasileiro e pode ser editado diretamente no HTML.

## Navegação

A navegação utiliza âncoras para rolagem suave entre as seções:

- `#como-funciona`
- `#projetos`
- `#habilidades`
- `#parceiros`
- `#faq`

## Validação do Formulário

O formulário de match de habilidades valida:
- Nome (obrigatório)
- E-mail (obrigatório, formato válido)
- Cidade/Estado (obrigatório)
- Habilidades (pelo menos uma selecionada)
- Disponibilidade (obrigatório)

## Compatibilidade

- Navegadores modernos (Chrome, Firefox, Safari, Edge)
- Mobile (iOS, Android)
- Respeita preferência de `prefers-reduced-motion`

## Licença

Este projeto está disponível sob a licença MIT. Para projetos criados na plataforma Fabr, recomenda-se:

- **Hardware**: Licença CERN OHL-S
- **Documentação**: Creative Commons CC BY-SA

## Contato

Para mais informações sobre o projeto Fabr, utilize os canais disponíveis no footer da landing page.

---

Desenvolvido com ❤️ para a comunidade de fabricação digital.