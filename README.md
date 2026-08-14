# RaulXP 🖥️

Site pessoal em formato de "desktop" retrô, inspirado na estética Windows XP / Y2K. É um **arquivo HTML único**, sem backend, sem build, sem dependências — é só abrir `index.html` num navegador (ou hospedar em qualquer lugar) e usar.

Inspirado no visual do [nandomp4.com](https://www.nandomp4.com/).

## ✨ Funcionalidades

- **Área de trabalho estilo XP**: ícones, janelas arrastáveis, barra de tarefas, menu Iniciar, tela de boot/shutdown e filtro CRT opcional.
- **Login local por usuário**: cada pessoa que usa o navegador cria um perfil (nome, e-mail, senha) e tem seu próprio desktop, papel de parede, bio, links e ordem/nomes dos apps.
- **Sobre mim**: perfil com foto, tagline, bio e links editáveis.
- **Internet**: mini navegador com iframe + botão "abrir em nova aba".
- **Blog**: posts com título, data e conteúdo, organizáveis em pastas.
- **Projetos**: explorador de arquivos — mostra as pastas criadas e os posts/recados guardados nelas.
- **Recados**: seus recados pessoais (escritos no Bloco de Notas, com imagem) + livro de visitas público pros visitantes deixarem mensagem.
- **Bloco de Notas**: escreve recados com texto e imagem anexada, e já salva direto numa pasta.
- **Paint**: editor de desenho com pincel, borracha, linha, retângulo, círculo, balde de tinta, 2 camadas, desfazer/refazer, controle de opacidade e exportação em PNG.
- **Calculadora**: calculadora simples com layout em grade.
- **Prompt de Comando**: terminalzinho com mais de 20 comandos (`ajuda`, `abrir`, `fechar`, `listar`, `cor`, `matrix`, `sorte`, etc.).
- **Configurações**: trocar foto de perfil, trocar papel de parede, reordenar/renomear apps e gerenciar usuários.
- **Lixeira**: posts e recados apagados vão pra lá antes de sumir de vez — dá pra restaurar ou excluir de vez.
- **Apoie**: seção com QR code ilustrativo pra Pix/doação.
- **Modo Edição**: ativa pelo menu Iniciar e permite editar praticamente qualquer texto clicando em cima.
- **Exportar/Importar dados**: salva todo o conteúdo em um `.json` e recarrega depois (ou em outro navegador/perfil).

## 🚀 Como usar

1. Baixe o `index.html`.
2. Abra direto no navegador **ou** hospede em qualquer serviço estático (GitHub Pages, Netlify, Vercel, etc).
3. No primeiro acesso, crie seu usuário (nome, e-mail, senha).
4. Ative o **Modo Edição** no menu Iniciar pra personalizar tudo: bio, links, posts, pastas, papel de parede, etc.

### Hospedando no GitHub Pages

```bash
# dentro do repositório
git add index.html
git commit -m "site RaulXP"
git push
```

Depois, em **Settings → Pages**, escolha a branch e a pasta (`/root`) e o site fica no ar em `https://SEU-USUARIO.github.io/SEU-REPOSITORIO/`.

## 🛠️ Tecnologia

Um único arquivo `index.html` com HTML, CSS e JavaScript puro (vanilla) — sem frameworks, sem build step, sem dependências externas (além de uma imagem de wallpaper padrão). Todos os dados (posts, recados, pastas, usuários, configurações) ficam salvos no **localStorage do navegador**.

## ⚠️ Sobre o sistema de login

O "login" com usuário/senha é **só um separador de perfis dentro do mesmo navegador** — não é um sistema de contas seguro de verdade. Como o site é estático (sem servidor), a senha fica salva sem criptografia no `localStorage` do próprio navegador. É ótimo pra dar um desktop personalizado pra cada pessoa que usa aquele computador/navegador, mas **não deve ser usado pra guardar informação sensível**.

Os dados também não são sincronizados entre dispositivos ou navegadores diferentes — cada navegador tem seu próprio conjunto de perfis. Use "Exportar dados" no menu Iniciar pra fazer backup ou levar o conteúdo pra outro lugar.

## 📁 Estrutura

Tudo vive em um único arquivo:

```
index.html   ← HTML + CSS + JS, tudo junto
```

## 📄 Licença

Sinta-se à vontade pra usar como base pro seu próprio site pessoal — só troque o conteúdo, o wallpaper e os links pelos seus.
