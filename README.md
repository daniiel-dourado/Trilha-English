> ⚠️ Este projeto foi desenvolvido exclusivamente para dispositivos móveis e não possui suporte para visualização em computadores.


# Trilha-English

Trilha de aprendizado de inglês (PWA) construída sob medida para estudo autodidata de pronúncia e fonética do inglês americano, usando a playlist **"Where to Start"** do canal **Rachel's English** como espinha dorsal.

O projeto nasceu de um plano de estudo estruturado com base em métodos reais de aquisição de idiomas (input compreensível, repetição espaçada, shadowing) combinados com neurociência da aprendizagem, e evoluiu para uma plataforma completa que o usuário pode instalar no celular.

---

## O que o projeto faz

Para cada aula da playlist "Where to Start", a plataforma oferece:

- **Vídeo incorporado** — reprodução direta do YouTube, sem sair da plataforma
- **Resumo do tema** — texto original escrito de forma independente sobre o assunto do vídeo (não é transcrição do que a Rachel fala)
- **Dicionário IPA da aula** — palavras-chave do tema com símbolo fonético e áudio clicável (via Web Speech API)
- **Atividade/quiz** — perguntas de múltipla escolha e de digitação, com feedback imediato e explicação
- **Trilha de progresso** — barra lateral com os marcadores numerados de cada aula, preenchendo conforme o usuário marca como concluída

---

## Estrutura de arquivos

```
trilha-english/
├── index.html          # Estrutura da trilha + lógica
├── styles.css           # Estilos visuais e animações
├── manifest.json         # Manifesto PWA
├── sw.js                 # Service worker (cache offline)
├── icon-192.png           # Ícone do app (192x192)
├── icon-512.png           # Ícone do app (512x512)
└── README.md
```

---

## Tecnologias usadas

- **HTML + CSS + JavaScript puro** — sem frameworks, sem build step
- **Web Speech API** (`speechSynthesis`) — geração de áudio de pronúncia direto no navegador, sem custo de API externa
- **Service Worker + Web App Manifest** — instalação como PWA (ícone na tela inicial, funcionamento offline após primeiro carregamento)
- **YouTube iframe embed** — reprodução dos vídeos da playlist diretamente na plataforma
- **Fonte Sora** (Google Fonts) — identidade visual em tema escuro

---

## Como instalar no celular (PWA)

1. Abra o link gerado no Chrome do celular
2. Menu (⋮) → "Adicionar à tela inicial"
3. Pronto — o app abre em tela cheia, com ícone próprio, funcionando offline depois do primeiro carregamento

---

## Fundamentação pedagógica

O conteúdo e a estrutura seguem princípios de métodos reconhecidos de aquisição de idiomas:

- **Input compreensível** (Stephen Krashen) — prioriza exposição a conteúdo levemente acima do nível atual, sem depender de tradução
- **Shadowing** (Alexander Arguelles, Luca Lampariello) — repetição imitativa de áudio nativo para treinar ritmo e articulação
- **Repetição espaçada e active recall** — aplicados nos quizzes de cada aula
- **Trilha sequencial** — a ordem das aulas segue a curadoria da própria Rachel's English para iniciantes, sem pular etapas

---

## Aviso sobre direitos autorais

Os resumos de cada aula são **conteúdo original**, escrito de forma independente com base no tema geral de cada vídeo — **não são transcrições** do que Rachel's English efetivamente fala. Os vídeos em si são incorporados via player oficial do YouTube (embed), sem download ou redistribuição do conteúdo audiovisual, projeto independente da Rachel’s English.

---

## Autor

Projeto desenvolvido por **Daniel Dourado**, com Claude (Anthropic) utilizado como ferramenta de desenvolvimento e mentor técnico e de idiomas ao longo do processo.
