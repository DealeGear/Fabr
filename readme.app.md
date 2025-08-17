

```markdown
# Fabr - Framework de Fabricação Compartilhada

Um aplicativo web para conectar pessoas em projetos colaborativos de fabricação, permitindo que usuários compartilhem habilidades e participem de projetos de inovação.

## 🚀 Funcionalidades

### 📋 Dashboard
- Visão geral com cards informativos:
  - Projetos disponíveis (filtrados por habilidades)
  - Projetos em andamento
  - Contribuições realizadas

### 👤 Autenticação de Usuários
- Sistema de login e cadastro
- Validação de formulários no frontend
- Persistência de dados no localStorage

### 🔧 Gerenciamento de Habilidades
- Adicionar e remover habilidades
- Busca inteligente na lista de habilidades disponíveis
- Habilidades pré-definidas: Soldagem, CAD, Impressão 3D, Eletrônica, Química de Materiais, etc.

### 📂 Listagem de Projetos
- Exibição em cards com informações relevantes
- Filtro dinâmico por habilidades do usuário
- Modal com detalhes completos do projeto
- Sistema de participação em projetos

### 🏆 Perfil do Usuário
- Informações pessoais editáveis
- Sistema de reputação baseado em contribuições
- Gestão de módulos e status (pendente, prototipagem, entregue, validado)
- Visualização dos projetos em que participa

### 🌓 Modo Claro/Escuro
- Toggle persistente entre temas
- Transições suaves
- Preservação da preferência do usuário

## 🛠️ Tecnologias Utilizadas

- **HTML5**: Estrutura semântica e acessível
- **CSS3**: Estilização com variáveis, flexbox, grid e animações
- **JavaScript (ES6+)**: Lógica do aplicativo sem frameworks externos
- **LocalStorage**: Persistência de dados no navegador

## 📁 Estrutura do Projeto

```
├── index.html          # Estrutura principal da aplicação
├── styles.css          # Estilos com design responsivo e modo escuro
├── app.js             # Lógica do aplicativo
└── README.md          # Documentação do projeto
```

## 🚀 Como Executar

1. **Clone o repositório**:
   ```bash
   git clone <URL-do-repositorio>
   cd fabr
   ```

2. **Abra o aplicativo**:
   - Abra o arquivo `index.html` em um navegador moderno
   - Ou utilize um servidor local (como Live Server no VS Code)

3. **Comece a usar**:
   - Crie uma conta ou faça login
   - Adicione suas habilidades
   - Explore os projetos disponíveis
   - Participe dos projetos que combinam com seu perfil

## 📱 Responsividade

O aplicativo é totalmente responsivo e se adapta a diferentes tamanhos de tela:

- **Mobile**: Layout otimizado para telas pequenas
- **Tablet**: Ajuste de grid e espaçamentos
- **Desktop**: Layout completo com todas as funcionalidades

## ♿ Acessibilidade

- Navegação por teclado (Tab, Enter, Esc)
- Estados de foco visíveis
- Contraste adequado para modo claro e escuro
- Estrutura semântica HTML5
- Labels associados aos inputs

## 🎨 Design

### Paleta de Cores
- **Primária**: Ciano (#00b4d8)
- **Secundária**: Esmeralda (#00f5d4)
- **Destaque**: Azul claro (#90e0ef)
- **Neutros**: Tons de cinza para textos e fundos

### Tipografia
- Fonte system font stack para melhor performance
- Tamanhos responsivos com unidades rem
- Hierarquia visual clara

## 🔧 Configuração

### Variáveis CSS
O projeto utiliza variáveis CSS no `:root` para fácil customização:

```css
:root {
    --primary-color: #00b4d8;
    --secondary-color: #00f5d4;
    --background-color: #f8f9fa;
    --text-primary: #212529;
    /* ... */
}
```

### Dados Iniciais
Os projetos e habilidades são definidos no `app.js`:

```javascript
const projetos = [
    {
        id: 1,
        titulo: "Máquina de Reciclagem de Plásticos",
        /* ... */
    }
];

const habilidadesDisponiveis = [
    "Soldagem", "CAD", "Impressão 3D", /* ... */
];
```

## 📊 Persistência de Dados

Todos os dados são salvos no `localStorage` do navegador:

- **Usuários cadastrados**
- **Sessão de login**
- **Habilidades do usuário**
- **Projetos em participação**
- **Preferência de tema (claro/escuro)**

## 🔄 Fluxo de Navegação

1. **Tela de Login/Cadastro**
   - Validação de e-mail e senha
   - Cadastro com informações básicas e habilidades

2. **Dashboard**
   - Visão geral das atividades
   - Acesso rápido para outras seções

3. **Projetos**
   - Listagem filtrada por habilidades
   - Detalhes e participação

4. **Habilidades**
   - Gerenciamento das competências
   - Busca e adição de novas habilidades

5. **Perfil**
   - Informações pessoais
   - Reputação e contribuições
   - Projetos ativos

## 🐛 Limitações

Como o projeto é 100% frontend sem backend:

- Os dados são persistidos apenas no navegador do usuário
- Não há sincronização entre dispositivos
- Não há autenticação real (simulada no frontend)
- Não há comunicação entre usuários

## 🚀 Melhorias Futuras

1. **Backend Real**
   - API RESTful para persistência de dados
   - Banco de dados (MongoDB, PostgreSQL)
   - Autenticação com JWT

2. **Funcionalidades Adicionais**
   - Sistema de mensagens entre colaboradores
   - Upload de arquivos e imagens
   - Histórico de versões dos projetos
   - Sistema de notificações

3. **Melhorias de UI/UX**
   - Animações mais elaboradas
   - Drag and drop para reorganização
   - Gráficos de progresso dos projetos

4. **Mobile App**
   - Versão nativa para iOS e Android
   - Notificações push
   - Acesso offline

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

## 👨‍💻 Desenvolvedor

Desenvolvido como parte do projeto Fabr - Framework de Fabricação Compartilhada.

---

**Nota**: Este é um projeto puramente demonstrativo, desenvolvido para fins educacionais e de portfólio. Todos os dados são simulados e persistidos localmente no navegador do usuário.
```