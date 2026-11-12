# 🚗 Autoescuelas Argente (Valencia & Torrent)

> Landing page profissional e de alta conversão para a **Autoescuelas Argente**, centro de formação de condutores com mais de 50 anos de história em Valencia e Torrent (Espanha). Especializada em Permiso B, Motocicletas em pista de práticas própria homologada, Permissões Profissionais (C, C+E, D), Transporte Pesado (CAP) e Recuperação Oficial de Pontos DGT.

---

## 🌟 Principais Recursos

- **Design Editorial & Alto Contraste**: Interface moderna em estética dark/editorial de alta fidelidade visual, tipografia refinada (Plus Jakarta Sans, Inter Tight, JetBrains Mono) e microinterações fluidas.
- **Estrutura 100% Otimizada**: Arquivos estáticos sem dependências desnecessárias em tempo de execução, imagens nomeadas no padrão web e otimizadas para carregamento veloz.
- **SEO & Metadados Completos**: Meta tags Open Graph, robots, esquema semântico, `robots.txt` e `sitemap.xml` prontos para indexação rápida no Google.
- **Segurança & Boas Práticas**: Links externos seguros (`rel="noopener noreferrer"`), cabeçalhos e permissões mínimas no pipeline, e `.gitignore` rigoroso.
- **CI/CD Automatizado**: Workflow de deploy contínuo integrado via GitHub Actions para publicação instantânea e segura no GitHub Pages com HTTPS.

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
└── sitemap.xml                 # Mapa do site para indexação
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

## 🌐 Deploy no GitHub Pages

O projeto já conta com o fluxo de integração e entrega contínua (**CI/CD**) configurado em `.github/workflows/deploy.yml`:

1. No repositório no GitHub (`ahk2001/autoescuela-argente`):
   - Vá até **Settings** > **Pages**.
   - Na seção **Build and deployment** > **Source**, selecione **GitHub Actions**.
2. A cada novo `git push` na branch `main`, o GitHub Actions efetuará o build e publicação automáticos no link seguro:
   👉 **`https://ahk2001.github.io/autoescuela-argente/`**
