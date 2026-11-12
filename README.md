# 🚗 Autoescuelas Argente (Valencia & Torrent)

> Landing page profissional e de alta conversão para a **Autoescuelas Argente**, centro de formação de condutores com mais de 50 anos de história em Valencia e Torrent (Espanha). Especializada em Permiso B, Motocicletas em pista de práticas própria homologada, Permissões Profissionais (C, C+E, D), Transporte Pesado (CAP) e Recuperação Oficial de Pontos DGT.

---

## 🌟 Principais Recursos

- **Design Editorial & Alto Contraste**: Interface moderna em estética dark/editorial de alta fidelidade visual, tipografia refinada (Plus Jakarta Sans, Inter Tight, JetBrains Mono) e microinterações fluidas.
- **Estrutura 100% Otimizada**: Arquivos estáticos sem dependências desnecessárias em tempo de execução, imagens nomeadas no padrão web e otimizadas para carregamento veloz.
- **SEO & Metadados Completos**: Meta tags Open Graph, robots, esquema semântico, `robots.txt` e `sitemap.xml` prontos para indexação rápida no Google.
- **Segurança Reforçada (Vercel & Headers)**:
  - Proteção contra Clickjacking (`X-Frame-Options: SAMEORIGIN`)
  - Proteção contra MIME-type sniffing (`X-Content-Type-Options: nosniff`)
  - Política de proteção contra XSS (`X-XSS-Protection: 1; mode=block`)
  - Política de Referrer restrita (`Referrer-Policy: strict-origin-when-cross-origin`)
  - Restrição de recursos de hardware desnecessários (`Permissions-Policy`)
  - HSTS ativado para comunicação 100% HTTPS segura
  - Cache imutável de 1 ano para arquivos estáticos em `/assets/`
- **Deploy Multi-Plataforma**: Compatível tanto com deploy automatizado via **Vercel** quanto **GitHub Pages** (CI/CD via GitHub Actions).

---

## 📁 Estrutura do Projeto

```text
argente/
├── .github/
│   └── workflows/
│       └── deploy.yml          # Pipeline CI/CD automático para GitHub Pages
├── assets/                     # Recursos visuais e mídias otimizadas
│   ├── alumna-aprobada-l.png   # Fotos reais de alunas aprovadas com placa L
│   ├── alumna-coche-argente.png
│   ├── alumno-l-coche.png
│   ├── alumno-sonriente.png
│   ├── aula-dgt.png            # Instalações de formação teórica homologada DGT
│   ├── favicon.webp            # Ícone de favoritos oficial
│   ├── home-desktop.jpeg       # Hero institucional desktop
│   ├── home-mobile.jpeg        # Hero institucional mobile
│   ├── logo.png                # Logomarca oficial da Autoescuelas Argente
│   ├── moto-kawasaki.png       # Frota e instrução de motos em circuito
│   ├── pista-motos.png         # Circuito próprio homologado para práticas
│   ├── trailer-articulado.png  # Veículos pesados para C+E e CAP
│   └── vehiculo-profesor.png   # Instrutores qualificados
├── docs/                       # Documentação interna de inteligência e pesquisa
│   ├── dados.txt               # Contatos, telefones e endereços das filiais
│   └── dossie_autoescola.md    # Dossiê de pesquisa, histórico e diferenciais
├── .gitignore                  # Exclusões de segurança e caches
├── index.html                  # Landing page completa, semântica e responsiva
├── README.md                   # Documentação do repositório
├── robots.txt                  # Regras para motores de busca
├── sitemap.xml                 # Mapa do site para indexação
└── vercel.json                 # Configurações de segurança e cache para Vercel
```

---

## 🚀 Como Executar Localmente

Como o projeto é construído em HTML5, CSS3 moderno e Vanilla JavaScript puros, nenhuma instalação pesada ou compilação é requerida:

1. Clone o repositório:
   ```bash
   git clone https://github.com/ahk2001/autoescuela-argente.git
   cd autoescuela-argente
   ```
2. Abra o arquivo `index.html` em qualquer navegador web moderno ou utilize uma extensão como o *Live Server* do VS Code.

---

## 🌐 Hospedagem e Deploy

### 1. Deploy na Vercel
O projeto conta com o arquivo `vercel.json` configurado com cabeçalhos de segurança estritos e cache agressivo para assets estáticos.
- Se o seu repositório estiver vinculado à Vercel através do dashboard (`vercel.com`), todo commit na branch `main` gera uma nova publicação em produção automaticamente.
- Para deploy via terminal:
  ```bash
  vercel --prod
  ```

### 2. Deploy no GitHub Pages
O projeto também conta com o fluxo de integração contínua em `.github/workflows/deploy.yml`:
1. No repositório GitHub (`ahk2001/autoescuela-argente`):
   - Vá até **Settings** > **Pages**.
   - Na seção **Build and deployment** > **Source**, selecione **GitHub Actions**.
2. O site estará disponível em:
   👉 **`https://ahk2001.github.io/autoescuela-argente/`**
