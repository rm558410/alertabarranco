# Planejamento do Protótipo Web AlertaBarranco

## Visão Geral
O AlertaBarranco é um sistema de monitoramento e alerta para áreas de risco de deslizamento. O protótipo web simulará todas as funcionalidades principais do sistema, permitindo demonstrar o conceito e a experiência do usuário de forma completa.

## Estrutura de Páginas

### 1. Página Inicial (Landing Page)
- **Objetivo**: Apresentar o sistema e seus benefícios
- **Conteúdo**:
  - Header com logo e navegação
  - Banner principal explicando o sistema
  - Seções sobre o problema dos deslizamentos
  - Como funciona o sistema
  - Benefícios para a população
  - Chamada para cadastro
  - Footer com informações de contato

### 2. Login/Cadastro
- **Objetivo**: Permitir acesso ao sistema e cadastro de novos usuários
- **Funcionalidades**:
  - Formulário de login (email/senha)
  - Opção "Esqueci minha senha"
  - Formulário de cadastro para novos usuários
  - Opção de cadastro para moradores de áreas de risco
  - Validação de campos

### 3. Dashboard (Página Principal após Login)
- **Objetivo**: Mostrar visão geral do status atual e acesso rápido às funcionalidades
- **Conteúdo**:
  - Status de risco atual (baixo, médio, alto)
  - Condições climáticas atuais
  - Últimos alertas recebidos
  - Acesso rápido ao mapa, alertas e configurações
  - Informações sobre a região do usuário

### 4. Mapa de Risco
- **Objetivo**: Visualizar áreas de risco e informações geográficas
- **Funcionalidades**:
  - Mapa interativo da cidade de São Paulo
  - Marcadores de áreas de risco (vermelho, amarelo, verde)
  - Informações detalhadas ao clicar nos marcadores
  - Simulação de rotas de evacuação
  - Filtros por nível de risco
  - Localização do usuário

### 5. Alertas
- **Objetivo**: Listar e gerenciar alertas recebidos
- **Funcionalidades**:
  - Lista de alertas ordenados por data
  - Filtros por nível de risco e status (lido/não lido)
  - Detalhes do alerta ao clicar
  - Opção para marcar como lido
  - Simulação de novos alertas
  - Histórico de alertas anteriores

### 6. Configurações
- **Objetivo**: Personalizar preferências de notificação e perfil
- **Funcionalidades**:
  - Perfil do usuário (nome, endereço, contatos)
  - Configurações de notificação por nível de risco
  - Canais de comunicação (WhatsApp, SMS, app)
  - Gerenciamento de localização
  - Opções de privacidade e segurança

## Componentes Reutilizáveis

1. **Header/Navbar**
   - Logo
   - Links de navegação
   - Indicador de status de risco
   - Botão de perfil/logout

2. **Footer**
   - Links institucionais
   - Contato
   - Redes sociais
   - Informações legais

3. **Cartão de Alerta**
   - Nível de risco (cor)
   - Título
   - Descrição
   - Data/hora
   - Ações disponíveis

4. **Indicador de Risco**
   - Visual colorido (verde, amarelo, vermelho)
   - Texto descritivo
   - Ícone correspondente

5. **Formulários**
   - Campos de entrada padronizados
   - Validação visual
   - Mensagens de erro/sucesso
   - Botões de ação

## Fluxos Principais

1. **Cadastro e Primeiro Acesso**
   - Usuário acessa landing page
   - Clica em "Cadastre-se"
   - Preenche formulário de cadastro
   - Recebe confirmação
   - É direcionado ao dashboard

2. **Recebimento de Alerta**
   - Simulação de novo alerta
   - Notificação visual no dashboard
   - Usuário acessa lista de alertas
   - Visualiza detalhes do alerta
   - Verifica rota de evacuação (se alto risco)

3. **Configuração de Preferências**
   - Usuário acessa configurações
   - Ajusta preferências de notificação
   - Atualiza informações de contato
   - Salva alterações
   - Recebe confirmação

## Tecnologias e Ferramentas

- **Frontend**: React com TypeScript
- **Estilização**: Tailwind CSS
- **Componentes**: shadcn/ui
- **Ícones**: Lucide icons
- **Gráficos**: Recharts
- **Mapas**: Leaflet ou Google Maps API
- **Gerenciamento de Estado**: React Context API
- **Simulação de Backend**: Dados mockados em JSON

## Responsividade

O design será totalmente responsivo, adaptando-se a:
- Desktops (1200px+)
- Tablets (768px - 1199px)
- Smartphones (320px - 767px)

Elementos específicos como o mapa terão versões otimizadas para cada tamanho de tela.

## Simulações e Mocks

1. **Login/Autenticação**
   - Simulação de autenticação com dados mockados
   - Persistência de sessão via localStorage

2. **Alertas**
   - Dados pré-definidos para histórico
   - Simulação de novos alertas com temporizador

3. **Mapa e Geolocalização**
   - Dados mockados de áreas de risco
   - Simulação de rotas de evacuação

4. **Notificações**
   - Simulação visual de notificações push
   - Demonstração de formatos para WhatsApp e SMS
