# Plataforma de Gestão Associativa

Sistema completo para gestão de associação de ex-alunos, desenvolvido com **Laravel 12**. Portal público com área restrita, painel administrativo avançado, integração de pagamentos e editor visual de e-mails.

---

## 🎯 Sobre o Projeto

Aplicação full-stack para associação com milhares de membros, cobrindo todo o ciclo de vida do associado: cadastro, pagamentos, comunicação, conteúdo e eventos.

**Destaques:**
- **31 módulos administrativos** no painel Filament (CRUDs, relatórios, dashboards)
- **Sistema de pagamentos** integrado a gateways brasileiros (PIX, Boleto, Cartão)
- **Editor visual de e-mails** estilo "Studio Pro" (drag-and-drop, preview responsivo, placeholders dinâmicos)
- **Gestão de conteúdo rica**: artigos com moderação, eventos com confirmação de presença, galerias polimórficas, loja
- **Autenticação híbrida**: Social Login (Facebook/Google) + credenciais próprias
- **Exportações profissionais** em Excel (multi-aba) para relatórios gerenciais

---

## 🛠 Stack Tecnológica

| Categoria | Tecnologias |
|-----------|-------------|
| **Backend** | Laravel 12, PHP 8.3 |
| **Admin Panel** | Filament v3 (ApexCharts, Progressbar, Oops) |
| **Frontend Reativo** | Livewire 3, Alpine.js |
| **Build & Estilo** | Vite 6, Tailwind CSS v4 |
| **Banco de Dados** | MySQL, Eloquent ORM |
| **Autenticação** | Laravel Socialite 5 (Facebook, Google) |
| **Pagamentos** | Asaas API, Mercado Pago SDK |
| **E-mail & Templates** | Sistema próprio dinâmico + SMTP |
| **Exportação** | maatwebsite/excel (XLSX) |
| **Processamento de Imagem** | Intervention/Image |
| **Testes** | PHPUnit 11 |
| **Qualidade de Código** | Laravel Pint |

---

## ✨ Funcionalidades Principais

### Gestão de Associados
Cadastro completo com validação em tempo real, perfil detalhado, controle de acesso por status de plano, histórico de pagamentos e visitas.

### Sistema Editorial
Artigos com fluxo de aprovação, editor rich text, galeria de imagens, curtidas, área do autor para gestão de próprias publicações.

### Eventos & Presenças
Dois tipos de eventos (internos e públicos), confirmação de presença para associados e visitantes, exportação de listas por evento, galerias de mídia com links externos.

### Galerias Institucionais
Sistema polimórfico único gerenciando 6 seções: diretoria, conselhos, presidentes, histórico (imagens/vídeos), turmas — tudo centralizado no painel admin.

### Loja & Assinaturas
Catálogo de produtos com estoque, SKU automático, integração direta para checkout. Planos de assinatura com renovação via gateway de pagamento.

### Documentos
Upload de PDFs institucionais, versionamento e controle de publicação.

### Editor de E-mails (Studio Pro)
Builder visual de blocos (texto, imagem, botão, HTML, divisores), preview desktop/mobile em tempo real, presets de tema, placeholders dinâmicos (`{{ variavel }}`), fallback automático para templates Blade.

### Configuração Centralizada
Singleton de configurações globais: modo manutenção, pop-ups, pixels/analytics (Facebook, Google Ads, GTM), chaves PIX, redes sociais, credenciais de login social.

### SEO & Analytics
Metadados por página (Open Graph, canonical), rastreamento de visitas, dashboard com 7 widgets gráficos (cadastros, artigos, contatos, eventos, visitas).

---

## 🏗 Arquitetura (Resumo)

- **MVC + Service Layer** — serviços desacoplados (pagamentos, renderização de e-mails)
- **Polimorfismo Eloquente** — reutilização de modelos (curtidas, galerias, mídias)
- **Singleton Pattern** — configurações globais, home, blocos institucionais
- **Middleware de Acesso** — controle automático de permissões por status de pagamento
- **Laravel 12 Moderno** — `casts()` method, middleware em `bootstrap/app.php`, providers em `bootstrap/providers.php`

---

## 🎯 Competências Demonstradas

- **Filament Avançado**: Resources polimórficos, edição de singleton, custom pages, widgets com charts, exports multi-sheet, navigation groups
- **Livewire 3**: Componente reativo complexo (drag-and-drop, preview real-time, gestão de estado multi-camada)
- **Integração de Pagamentos**: Implementação completa Asaas (cliente, cobrança Lean PIX/Boleto/Cartão, QR Code, webhooks)
- **Sistema de Templates Dinâmicos**: Separação dados/apresentação, placeholders tipados, fallback graceful
- **Arquitetura Escalável**: Services isolados, middleware centralizado, configuração single-source-of-truth

---

## 📄 Licença

Projeto privado, código não público. Este README serve para fins de portfólio e demonstração de competências técnicas.

---

## 🤝 Contato

**Desenvolvedor Full Stack Laravel**

- LinkedIn: [Gabriel José Silva](https://linkedin.com/in/gabriel-josé-silva-060103255)
- GitHub: [Onrracoutinho](https://github.com/onrracoutinho)
- E-mail: canalgabrieljose@gmail.com

> *Disponível para oportunidades remotas/presenciais (Brasil/Europa).*