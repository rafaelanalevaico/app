# App Rafaela Nalevaico: como colocar no ar

O app é um PWA: um site que se instala no celular como aplicativo, no iPhone e no Android, sem passar pela App Store nem pela Play Store.

Para funcionar no celular das pessoas, ele precisa estar hospedado na internet. A hospedagem sugerida é o GitHub Pages, que é gratuito e é onde a "Área da Rafaela" grava os áudios.

## 1. Publicar o app (uma vez só, cerca de 10 minutos)

1. Crie uma conta gratuita em github.com (de preferência no nome da Rafaela).
2. Clique em **New repository**. Dê o nome `app`, marque **Public** e clique em **Create repository**.
3. Na página do repositório, clique em **uploading an existing file**. Arraste para lá **tudo o que está dentro desta pasta** (não a pasta em si) e clique em **Commit changes**.
4. Vá em **Settings → Pages**. Em "Branch", escolha `main` e a pasta `/ (root)`. Clique em **Save**.
5. Em um ou dois minutos o app estará em `https://SEU-USUARIO.github.io/app/`.

## 2. Criar a chave de acesso da Rafaela (uma vez só)

1. No GitHub: foto do perfil → **Settings → Developer settings → Personal access tokens → Fine-grained tokens → Generate new token**.
2. Em "Repository access", escolha **Only select repositories** e marque o repositório `app`.
3. Em "Permissions → Repository permissions", coloque **Contents** como **Read and write**.
4. Gere a chave e copie. Ela funciona como uma senha: não compartilhe e não publique.

## 3. Como a Rafaela publica um áudio

1. Abrir o app no celular ou no computador.
2. Na tela Início, rolar até o fim e tocar em **Área da Rafaela**.
3. Na primeira vez: preencher usuário, repositório e a chave de acesso, e tocar em **Conectar**. Fica salvo só naquele aparelho.
4. Tocar em **Enviar** (ou **Trocar**) na sessão desejada e escolher o arquivo.
5. O áudio entra no ar em alguns minutos, para todo mundo.

Para criar um áudio que não está na lista, use **Nova sessão** no fim da mesma tela e depois envie o arquivo.

Formato: MP3 ou M4A, até 95 MB por arquivo. Sugestão: MP3 a 128 kbps (30 minutos ficam com cerca de 29 MB).

## 4. Grupo do WhatsApp (tela Comunidade)

A tela **Comunidade** tem um botão que leva a pessoa para o grupo de WhatsApp dos workshops gratuitos.

1. No WhatsApp, abra o grupo → **Convidar via link** → copie o link (começa com `https://chat.whatsapp.com/`).
2. No app, abra a **Área da Rafaela**, cole o link em **Grupo do WhatsApp** e toque em **Salvar link**.

Enquanto não houver link, o botão aparece como "Grupo em breve". Para trocar de grupo, basta salvar um link novo.

## 5. Como as pessoas instalam

- **iPhone:** abrir o link no Safari, tocar em Compartilhar e depois em "Adicionar à Tela de Início".
- **Android:** abrir o link no Chrome e tocar em "Instalar app".

O próprio app mostra essa instrução na tela Início.

## Importante saber

- **Os 4 áudios que já estão na pasta `audios` são demonstrações com voz sintética.** Servem só para testar o player. Eles aparecem marcados como "Demonstração" e somem quando a Rafaela enviar o áudio dela na mesma sessão. Para lançar sem eles, apague os arquivos da pasta `audios` antes de publicar.
- **Os áudios ficam públicos.** Qualquer pessoa com o link do app consegue ouvir. Não há login nem pagamento. Se os áudios forem vendidos, será preciso outra solução, com área de membros.
- **Os áudios precisam de internet para tocar.** O app abre sem internet, mas não guarda os áudios no aparelho.
- **O envio pela Área da Rafaela foi testado só com um GitHub simulado.** O primeiro envio de verdade vale como teste final.
- **App Store e Play Store:** para aparecer nas lojas é preciso conta de desenvolvedor (Apple: US$ 99 por ano; Google: US$ 25 uma vez) e empacotar este mesmo app. Dá para fazer depois, sem refazer nada.

## Arquivos

- `index.html`: o app inteiro (telas, player e Área da Rafaela).
- `sessoes.json`: a lista de sessões (nome, frase de apoio, categoria).
- `config.json`: o link do grupo do WhatsApp.
- `audios/`: os áudios. O nome do arquivo é o "slug" da sessão, por exemplo `04-corpo-em-harmonia.mp3`.
- `img/`: logo e ícones.
- `manifest.webmanifest` e `sw.js`: o que torna o app instalável e o faz abrir sem internet.
