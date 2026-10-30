# Prévia — Telma Elisa · Psicóloga

Protótipo estático de site para **Telma Elisa da Silva Souza** (CRP 04/70625), psicóloga em Juiz de Fora/MG.
Feito como prévia de apresentação, sem publicar nada no domínio atual da cliente.

## O que é

Site de uma página, 100% estático (sem build, sem dependências), com identidade própria:
vinho, creme e dourado; tipografia editorial (Instrument Serif + DM Sans).

## Estrutura

```
index.html            página completa (SEO, Open Graph, JSON-LD Psychologist)
assets/css/style.css  estilos
assets/js/main.js     menu mobile, scrollspy, reveal, voltar ao topo
assets/img/           fotos otimizadas (hero, sobre, OG) e favicon
```

## Rodar localmente

```bash
python -m http.server 4174
# http://127.0.0.1:4174
```

## Publicar

Arraste a pasta em qualquer host estático (Vercel, Netlify, GitHub Pages).
Não precisa de build: root do projeto = esta pasta, output = `index.html`.

## Origem das informações

- **Perfil no Google (Maps):** 5,0 · 45 avaliações; endereço e horário (seg–sex, 8h–21h).
- **Site atual** (`telmaelisapsi.com.br`): bio, formações, mídia, depoimentos, FAQ, contatos.
- **Doctoralia:** CRP 04/70625, 113 opiniões, especialidades.
- **Base de prospecção** (`leads.md` / `leads.csv`): lead nº 7, contato e diagnóstico técnico.

## Diagnóstico do site atual (medido)

- O preloader fica travado em **0–12%** mesmo depois de 42 s, com vídeo e imagens já carregados.
- Imagens servidas em **3989 px** e **4424 px** de largura (604 KB só a foto principal).
- Aplicação Nuxt/Vue: ~1 MB de JS antes de qualquer conteúdo aparecer.
- Rodapé estourando a largura da tela no celular (relatado na prospecção).

## O que foi feito nesta prévia

- Página única, ~360 KB no total, sem framework.
- Fotos redimensionadas: 604 KB → 65 KB (hero) e 52 KB → 48 KB (sobre).
- Zero rolagem horizontal de **280 px a 1024 px**, inclusive com fonte do sistema em **130% e 200%**.
- Lighthouse: **100** em acessibilidade, boas práticas e SEO.
- Alvos de toque ≥ 44 px, menu mobile com rolagem própria e foco/ESC.

## Melhorias de conversão (2ª versão)

- **Barra fixa de agendamento** no mobile, sempre visível no rodapé da tela.
- **Faixa de selos de confiança** (CRP, Google 5,0 · 45 avaliações, 113 opiniões no Doctoralia, atendimento online).
- **Oferta explícita**: primeira conversa de 15 minutos, sem custo, no hero, em "Como começar", no contato e no FAQ.
- **Filtro de intenção** — seção "Pode fazer sentido / Talvez não seja o momento" (`#faz-sentido`), com cuidado ético (sem promessa de resultado).
- **WhatsApp contextual** por especialidade: cada card abre a conversa já com o tema.
- **Galeria do consultório** (`#espaco`): recortes reais das fotos existentes + card de citação.
- **Assinatura manuscrita**, contadores animados (45 avaliações, 5,0, 113 opiniões) e textura de papel.
- **Headline com revelação em máscara** e molduras nas fotos, mantendo leitura e contraste.
- Conteúdo ético conforme CFP: sem antes/depois, sem promessa de cura; CVV 188 e CAPS em caso de crise.

## A confirmar com a cliente

- Oferta da primeira conversa de 15 minutos sem custo (texto e condições).
- Horário de atendimento (hoje: seg–sex, 8h–21h, segundo o Google).
- E-mail e Instagram usados no site atual.
- Valores de sessão e área de cursos (fora do escopo desta prévia).

## Links

- Prévia publicada: https://srthiagobor13.github.io/telma-elisa/
- WhatsApp: https://wa.me/5532984111185
- Doctoralia: https://www.doctoralia.com.br/telma-elisa-da-silva-souza/psicologo/juiz-de-fora
- Instagram: https://www.instagram.com/telmaelisa.psi/
