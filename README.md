# Juju Maria — Nossa História

Álbum de família privado, local-first, para guardar e reviver memórias da Júlia.

## Princípios

- **Local-first**: tudo fica no seu computador (SQLite + pasta `media/`). Nada sobe para nuvem por padrão.
- **Privacidade**: fotos, vídeos e vozes da família **nunca** entram neste repositório.
- **Simples**: monolito FastAPI + `index.html` puro. Sem frameworks de SPA, sem bundler.
- **Afetivo**: fotos grandes, textos curtos, voz, datas especiais e um cantinho para brincar com a personagem "Ju".

## Como rodar (Windows)

```bash
cd juju-maria
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
python app.py
```

Abra o navegador em http://127.0.0.1:8000.

## Estrutura esperada

```
juju-maria/
├── index.html      ← toda a interface
├── app.py          ← backend FastAPI + SQLite
├── requirements.txt
├── README.md
├── data/           ← criado automaticamente (juju.sqlite3)
└── media/          ← arquivos enviados (nomes UUID)
```

## O que NÃO vai para o GitHub

- `data/`
- `media/`
- qualquer foto, áudio ou vídeo real da família
- chaves de API

Este repositório guarda apenas o código do álbum. As memórias ficam com você.
