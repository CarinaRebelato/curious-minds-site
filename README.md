# Curious Minds — site pronto para publicar

Site estático (HTML + imagens), sem build. Basta hospedar a pasta inteira.

```
curious-minds-site/
├── index.html
├── favicon-32.png
├── apple-touch-icon.png
├── CLAUDE.md            ← contexto do projeto para o Claude Code
└── assets/img/          ← logos, foto da Teacher Carina, og-image
```

Para ver localmente: abra `index.html` no navegador.

## Pendências antes de publicar

Já resolvido: WhatsApp (11) 98540-7230 nos botões, link de envio do Google Forms, botão "Conheça minha história" removido, botão "Quero conhecer as turmas" apontando direto para o WhatsApp, domínio `curiousminds.com.br` (canonical e og:image já apontam para ele). O link do Instagram no rodapé está oculto (comentado no HTML) até o perfil existir.

| O quê | Onde no `index.html` | O que fazer |
|---|---|---|
| Fotos | comentários `TODO` | Foto de fundo do hero, faixa de 3 fotos da Mostra Cultural (está comentada) e fundo da chamada final |

## Como publicar com o Claude Code

1. Descompacte esta pasta e abra o terminal dentro dela.
2. Rode `claude` e cole o prompt abaixo.

### Prompt para colar no Claude Code

```
Este diretório é o site estático da Curious Minds (leia o CLAUDE.md e o README.md).
Quero publicá-lo online. Por favor:

1. Revise as pendências da tabela do README e me pergunte o que faltar
   (se houver). Aplique as respostas no index.html.
2. Inicialize um repositório git, faça o primeiro commit e crie um repositório
   no meu GitHub chamado curious-minds-site.
3. Publique o site gratuitamente (sugestão: Netlify, Vercel ou GitHub Pages;
   me pergunte qual prefiro e me guie no login se for preciso).
4. Configure o domínio curiousminds.com.br (e o www) para o site: me diga
   exatamente quais registros DNS criar no Registro.br e confirme o HTTPS.
5. Ao final, me passe o link publicado.

Não altere textos, cores ou layout sem me perguntar.
```

## Observações

- Na seção "Prazer, sou a Teacher Carina" ficou de fora a nota interna *"(Você pode inserir links nos nomes das escolas direcionando para os perfis no Instagram)"*. Se quiser os links, passe os perfis das escolas (Tigrinhos/Golden Tigers, Red House, Villare).
- Os quadros de "Projetos que ganharam vida" são ilustrações clicáveis que abrem as postagens no Instagram. Para mostrar a foto real de cada postagem, salve uma imagem de cada uma em `assets/img/` e troque o bloco colorido por `<img>`.
