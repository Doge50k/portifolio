# Portfólio Profissional - Elias | Soluções Digitais & IA

Landing page moderna e responsiva desenvolvida com **Astro** e **Tailwind CSS**.

## 📋 Estrutura do Projeto

```
portifolio/
├── src/
│   ├── pages/
│   │   └── index.astro          # Página principal da landing page
│   ├── components/
│   │   ├── Navbar.astro         # Barra de navegação fixa
│   │   ├── Hero.astro           # Seção de apresentação com CTA
│   │   ├── Services.astro       # Seção de serviços (3 cards)
│   │   ├── CaseStudies.astro    # Seção de casos de uso
│   │   └── Footer.astro         # Rodapé com links e informações
│   ├── layouts/
│   │   └── Layout.astro         # Layout principal (meta, fonts, estrutura HTML)
│   └── styles/
│       └── global.css           # Estilos globais e variáveis personalizadas
├── public/                       # Arquivos estáticos (imagens, ícones, etc)
├── astro.config.mjs             # Configuração do Astro com Tailwind
├── tailwind.config.mjs          # Temas e extensões personalizadas
├── tsconfig.json                # Configuração TypeScript
├── package.json                 # Dependências do projeto
└── README.md                    # Este arquivo
```

## 🚀 Início Rápido

### Instalação

```bash
# Clone ou navegue até o diretório do projeto
cd portifolio

# Instale as dependências
npm install
```

### Desenvolvimento

Inicie o servidor de desenvolvimento com:

```bash
npm run dev
```

O site estará disponível em `http://localhost:3000`.

### Construção para Produção

```bash
npm run build
```

Os arquivos otimizados serão gerados em `dist/`.

### Preview da Build

```bash
npm run preview
```

## 🎨 Componentes

### Navbar
Barra de navegação fixa no topo com:
- Logo e branding
- Links de navegação
- Botão CTA "Contratar"

**Arquivo:** `src/components/Navbar.astro`

### Hero
Seção de destaque com:
- Título principal com gradiente
- Descrição/pitch
- Botão CTA principal
- Badge de disponibilidade
- Imagem de perfil

**Arquivo:** `src/components/Hero.astro`

### Services
Grid com 3 cards de serviços:
1. **Sistemas Web Sob Medida** - Python + Django
2. **Inteligência Artificial Aplicada** - LLMs
3. **Infraestrutura que não para** - Docker

**Arquivo:** `src/components/Services.astro`

### CaseStudies
Grid com 2 casos reais de sucesso:
- **Biipp** - Automação de afiliados
- **Integração de IA** - RAG e LLMs

**Arquivo:** `src/components/CaseStudies.astro`

### Footer
Rodapé com:
- Informações da empresa
- Links de redes sociais
- Copyright

**Arquivo:** `src/components/Footer.astro`

## 🎯 Seções da Página

| Seção | ID | Descrição |
|-------|----|----|
| **Início** | #inicio | Apresentação com imagem de perfil |
| **Serviços** | #servicos | Grid com 3 serviços principais |
| **Casos de Uso** | #casos | Portfolio com 2 projetos reais |

## 🛠️ Stack Tecnológico

- **Framework:** Astro (SSG/SSR estático)
- **Estilos:** Tailwind CSS 3.4.0
- **Fontes:** Plus Jakarta Sans (Google Fonts)
- **Ícones:** Font Awesome 6.4.0
- **Linguagem:** Astro + HTML

## 🎨 Design System

### Cores
- **Fundo:** `#050505` (dark-bg)
- **Secundário:** `#080808` (dark-secondary)
- **Primária:** `#10B981` (emerald-500)
- **Destaque:** `#06B6D4` (cyan-500)

### Componentes Reutilizáveis (CSS)

#### `.glass`
Efeito glassmorphism com blur e transparência.

```css
.glass {
  @apply bg-white/3 backdrop-blur-[10px] border border-white/5;
}
```

#### `.text-gradient`
Gradient de texto em verde → ciano.

```css
.text-gradient {
  @apply bg-gradient-to-r from-emerald-500 to-cyan-500 bg-clip-text text-transparent;
}
```

#### `.btn-primary`
Botão CTA com gradient e shadow.

```css
.btn-primary {
  @apply bg-gradient-to-r from-emerald-500 to-emerald-600 shadow-lg shadow-emerald-500/30;
}
```

#### `.card-hover`
Animação de hover para cards.

```css
.card-hover {
  @apply transition-all duration-300 hover:-translate-y-1 hover:border-emerald-500/40;
}
```

#### `.blob`
Shapes decorativas blurradas.

```css
.blob {
  @apply absolute w-[300px] h-[300px] rounded-full blur-[80px] -z-10;
}
```

## 📝 Personalização

### Alterar Informações de Contato

No componente **Navbar** e **Hero**, altere:
```astro
href="https://wa.me/seu-numero"
```

### Alterar Email de Contato

No componente **Footer**:
```astro
href="mailto:seu-email@dominio.com"
```

### Mudar CNPJ

No componente **Footer**, atualize:
```html
<p class="text-gray-600 text-[10px] mt-4 font-bold tracking-widest uppercase">CNPJ: 00.000.000/0001-00</p>
```

### Adicionar Redes Sociais

Links no **Footer**:
```astro
<a href="seu-link-linkedin" class="hover:text-emerald-500 transition">
  <i class="fab fa-linkedin"></i>
</a>
```

### Mudar Imagem de Perfil

No componente **Hero**:
```astro
<img src="seu-url-imagem" alt="Seu Nome" class="..." />
```

## 🚀 Deploy

A landing page pode ser deployada em:
- **Vercel:** [vercel.com](https://vercel.com)
- **Netlify:** [netlify.com](https://netlify.com)
- **GitHub Pages:** Com `astro build` → push `dist/`

### Deploy Vercel (Recomendado)

```bash
npm install -g vercel
vercel
```

## 📚 Recursos

- [Documentação Astro](https://docs.astro.build)
- [Tailwind CSS](https://tailwindcss.com)
- [Font Awesome Icons](https://fontawesome.com)

## 📄 Licença

Todos os direitos reservados © 2026 Elias.
