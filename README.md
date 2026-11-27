# Scripts MHS para SandFly

Scripts em Lua para o leitor de telas [SandFly](https://github.com/aaron-gh/SandFly), no Android, feitos para uso em português do Brasil por quem é cego ou tem baixa visão. Cada script vem com os textos traduzidos para o português.

## Como usar

Adicione este repositório como fonte de scripts. Nas configurações do SandFly, vá em **Scripts** > **Fontes de script** > **Adicionar fonte** e digite:

```
github.com/MHS-Softwares/Scripts-MHS-para-Sandfly
```

Depois escolha a fonte na lista, selecione o script, revise o diálogo de instalação e toque em **Instalar**. O SandFly verifica uma vez por dia se há versão nova e avisa ou atualiza, conforme a opção **Atualizar scripts automaticamente**.

Também dá para baixar o arquivo `.zip` daqui e usar **Scripts** > **Importar script**.

## Scripts

| Script | App | O que faz |
|---|---|---|
| `whatsapp-mensagens-mhs.zip` | WhatsApp e WhatsApp Business | Cada mensagem de uma conversa é lida como um item só, com as ações dela no menu Ações; ajuda com mensagens de voz (velocidade de reprodução no menu Ações, o foco acompanha a que está tocando e a tela fica ligada), vídeos e álbuns (dois toques baixam ou reproduzem), documentos, "Ler mais", links, o botão do microfone e conversas com muitas mensagens não lidas. |
| `viva-voz-whatsapp-mhs.zip` | WhatsApp e WhatsApp Business | Nas ligações, afastar o celular da orelha liga o viva-voz e aproximar de novo volta para o fone de ouvido. |
| `instagram-mhs.zip` | Instagram | Reels, stories, publicações do feed, Explorar, perfil, notificações e o Direct (lista de conversas e conversa aberta) mais fáceis de usar com o leitor de telas, com os botões no menu Ações e comandos para ir ao próximo e ao anterior. |
| `youtube-mhs.zip` | YouTube e YouTube Morphe | Versão em português do script *YouTube video actions*, de Aaron Hewitt: cada vídeo das listas é um item só, com os botões no menu Ações, e a página do vídeo fica limpa, com as ações do player (curtir, não gostei, compartilhar, perguntar, salvar, inscrever-se, comentários, tradução de voz, reprodução automática e mais opções) no menu Ações. |
| `zello-mhs.zip` | Zello | Dois toques no botão de falar apertam o botão com um toque na tela, como um dedo, que é o único jeito de ele responder. |
| `google-mensagens-mhs.zip` | Google Mensagens | Fixar, arquivar, excluir, adiar, bloquear, marcar como não lida e selecionar conversas e mensagens pelo menu Ações. |
| `cliques-automaticos-mhs.zip` | Todos os apps | Monta uma lista de botões que são apertados em sequência, um depois do outro, com comandos para criar, rodar e guardar sequências. |
| `aquamail-mhs.zip` | AquaMail | Cada e-mail da lista é lido de forma curta (quem enviou, assunto, hora, anexos); o menu Ações seleciona, exclui, arquiva e responde, e o foco fica na mensagem selecionada. |
| `gravar-e-compartilhar-mhs.zip` | Todos os apps | Um comando grava áudio em estéreo e, ao ser usado de novo, para e abre o compartilhamento com a gravação. |
| `descrever-com-ia-mhs.zip` | Todos os apps | Comandos que mandam o item em foco, ou a tela inteira, ao Be My Eyes ou ao Seeing AI, que descrevem a imagem. |

## O que cada script faz

### WhatsApp mensagens (MHS), para o WhatsApp e o WhatsApp Business

- **Uma mensagem, um item.** Cada mensagem é lida com quem enviou, o conteúdo, a mensagem que ela responde e a hora. Na lista de conversas, deslizar pula a foto de cada conversa, que abre o perfil pelo menu Ações da conversa.
- **Menu Ações de cada mensagem.** Tocar, a velocidade de reprodução e os outros botões da mensagem ficam no menu Ações, junto com as ações do próprio WhatsApp: responder, encaminhar, compartilhar e outras.
- **Mensagens de voz.** Dois toques tocam a mensagem, mesmo as que você enviou ou que citam outra mensagem. Dois dedos para a direita avançam e dois dedos para a esquerda voltam.
- **Gravar mensagem de voz.** Ao começar a gravar tocando no microfone, sem segurar, o foco vai para o Enviar em vez do Pausar, sem o leitor falar.
- **Velocidade de reprodução.** O menu Ações da mensagem de voz tem a velocidade de reprodução, que troca sem parar a mensagem. Também há um comando para atribuir a um gesto.
- **Vídeos.** Dois toques baixam o vídeo que ainda não foi baixado e reproduzem o que já foi, também em grupos e em mensagens que o WhatsApp mostra sem identificação. O menu Ações tem as mesmas opções.
- **Álbuns de fotos e vídeos.** Cada foto e vídeo do álbum é um item só, com as ações no menu Ações. No reprodutor de vídeo, o leitor não fica lendo o progresso a cada instante.
- **Documentos.** Dois toques abrem o documento, em vez de apertar Encaminhar.
- **Mensagens longas.** O "Ler mais" abre sozinho quando a mensagem recebe o foco. Um toque com três dedos aperta o "Ler mais" da mensagem em foco e lê tudo.
- **Botão do microfone.** Diz só "Gravar". As instruções dele só são faladas com as dicas de uso do SandFly ligadas.
- **Links, e-mails e telefones.** No menu Ações da mensagem, cada link, endereço de e-mail e número de telefone dela pode ser copiado.
- **Conversas com muitas mensagens não lidas.** O WhatsApp tem um bug: às vezes você abre uma conversa com muitas mensagens não lidas e ele te leva para mensagens de vários dias atrás, antes das não lidas. O comando **Encontrar a linha das mensagens não lidas** rola a conversa, direto e sem parar, até achar a linha que diz quantas mensagens não foram lidas, mesmo longe da tela, e põe o foco nela. O comando **Ir para a última mensagem** vai ao fim da conversa e põe o foco na mensagem mais nova, sem o foco voltar para onde estava. Nenhum dos dois tem gesto até você atribuir um em **Comandos** > **Scripts**.
- **Mensagem de voz tocando.** Enquanto uma mensagem de voz toca, o foco vai para ela, e a tela não apaga, porque o WhatsApp para de tocar quando a tela apaga. Cada uma das duas coisas tem uma opção nas configurações do script. O tempo de tela que você tinha volta quando a reprodução termina.
- **Ir para a mensagem respondida.** No menu Ações de uma resposta, essa opção aperta a citação, o WhatsApp rola a conversa até a mensagem original, e o foco do leitor vai para ela, que é lida. Quando a citação é de áudio, voz, foto, vídeo ou documento, a mensagem é achada pelo autor. Uma opção nas configurações do script ajusta quanto esperar o WhatsApp rolar a tela antes de procurar a mensagem (250 milissegundos).
- **Idiomas.** Funciona com o WhatsApp em português do Brasil e em inglês.

### Viva-voz do WhatsApp (MHS), para o WhatsApp e o WhatsApp Business

- Em uma ligação, afastar o celular da orelha liga o viva-voz; aproximar de novo volta para o fone de ouvido. Só uma vibração curta avisa, sem o leitor falar.
- Aperta o botão de viva-voz da tela da ligação só quando o áudio não está como deveria, o que ele pergunta ao Android. Fone de ouvido, com fio ou Bluetooth, fica como está.
- O comando **Dizer o estado do áudio da ligação** diz o que o script está vendo. Era parte do script de mensagens do WhatsApp (versão 3.9) e virou um script à parte, para o de mensagens funcionar só no WhatsApp e sem a permissão Java.

### Instagram (MHS), para o Instagram

- **Reels.** Os comandos **Próximo reel** e **Reel anterior** rolam e põem o foco no reel. O menu Ações de um reel tem Curtir, Comentários, Compartilhar, Salvar, Seguir, Mais opções e um resumo (quem fez, do que trata, quantas curtidas e comentários). Na aba Reels, deslizar com dois dedos para cima vai ao próximo e para baixo ao anterior.
- **Stories.** Próximo e anterior, a história da próxima e da anterior pessoa, pausar ou tocar, curtir, responder, comentários, compartilhar e um resumo (quem postou, há quanto tempo, o que é a imagem e quem foi mencionado).
- **Feed.** O menu Ações de uma publicação tem Curtir, Comentar, Repostar, Compartilhar, Salvar, Mais opções, Mostrar a legenda inteira, Ir ao perfil de quem postou, Tocar ou pausar o vídeo, Ligar ou desligar o som, Abrir a música e, nos anúncios, o botão do anúncio. Esses botões saem da varredura, para o leitor não parar em cada um (uma opção desliga isso).
- **Notificações e pessoas sugeridas.** Cada uma é lida como um item só, com o que ela diz e o estado do botão; os botões, como Seguir e Ir ao perfil, ficam no menu Ações.
- **Perfil.** Os números de publicações, seguidores e seguindo são lidos com um espaço entre o número e a palavra; o painel do perfil e as abas (grade, Reels, repostados, fotos com você) ficam mais limpos, sem itens soltos.
- **Explorar.** Cada publicação da grade é um item só, sem os botões pequenos que o Instagram põe em cima dela.
- **Direct.** Cada conversa da lista é um item só, com notas, filtros e botões sem nome deixados de lado. Em uma conversa aberta, cada mensagem é uma linha só, sem as peças soltas (texto, reação, story, botão da transcrição), e as ações dela (responder, reagir, mais opções, encaminhar, ver transcrição) ficam no menu Ações. As opções da conversa abrem pelo menu Ações.
- Quando um reel ou story abre, o controle de leitura vai para Ações, para deslizar para cima ou para baixo passar por elas.

### YouTube (MHS), para o YouTube e o YouTube Morphe

- **Listas.** Cada vídeo, mix, lista de reprodução, comentário e resposta das listas é um item só, e os botões dentro dele ficam no menu Ações. Isso é o que o script original faz.
- **Atalhos do teclado do YouTube.** Os comandos, como K, J, L, M, F e C, controlam o player e podem ser atribuídos a gestos em **Comandos** > **Scripts**.
- **Página do vídeo.** O menu Ações do player tem Curtir, Não gostei, Compartilhar, Perguntar, Salvar, Inscrever-se, Comentários, Tradução de voz, Reprodução automática e Mais opções, e esses botões saem da varredura. A lista de vídeos abaixo do player é lida uma linha por vez, com os botões de cada linha no menu Ações. Uma opção desliga essa limpeza.
- **Descrição do vídeo.** Ao abrir a descrição, o script aperta "Mostrar mais" sozinho, e os links dela ficam no menu Ações, também quando o YouTube os mostra como botões dentro do texto. Uma opção desliga a descrição já expandida.
- **Aviso do início.** Uma opção faz o script dizer, ao começar, quantas regras o SandFly aceitou, para achar problemas. Dá para desligar quando tudo estiver funcionando.

### Zello (MHS), para o Zello

- **Botão de falar.** O botão de falar do Zello ignora o duplo toque do leitor de telas, que aperta sem encostar na tela, e só responde a um toque de verdade. Com o script, dois toques nele fazem um toque na tela, no meio do botão. Com o botão no modo de alternar, os dois toques começam e param a fala. Em qualquer outro item, o duplo toque faz o que sempre faz.
- **Tempo.** O SandFly espera um pouco antes de tocar na tela, então o botão responde cerca de um terço de segundo depois dos dois toques. Dois números nas configurações do script ajustam o tempo do toque e essa espera; a espera só diminui num SandFly que aceite a opção de espera nos gestos de toque, que ainda não está no SandFly oficial.

### Google Mensagens (MHS), para o Google Mensagens

- No menu Ações de cada conversa da lista: Fixar, Marcar como não lida, Arquivar, Excluir, Adiar, Bloquear, Adicionar contato e Selecionar conversa. Dentro de uma conversa, o menu Ações de cada mensagem tem Selecionar mensagem.
- Dá para selecionar várias conversas ou mensagens e excluir ou arquivar de uma vez. Uma opção mantém o foco no que foi selecionado.
- Funciona com o Google Mensagens em português do Brasil e em inglês.

### Cliques automáticos (MHS), para todos os apps

- Monta uma lista de botões apertados um depois do outro. Em cada tela, adicione o item em foco, ou um nome que você copiou, como um passo. Ao rodar a sequência, o script espera cada botão aparecer e aperta.
- Um `*` no nome de um passo vale por qualquer texto, e o comando que ignora números faz isso por você, para botões como "Limpar conversa (723,2 MB)". Um passo pode ser um toque longo.
- Cada sequência pertence ao app onde foi feita e pode ganhar uma vaga, que é um comando próprio para atribuir a um gesto. Comandos para criar, escolher, gerenciar, remover o último passo e rodar (usado de novo, para).

### AquaMail (MHS), para o AquaMail

- **Lista de e-mails.** Cada e-mail é lido de forma curta: o estado (conversa, selecionada, não lida), quem enviou, o assunto, a hora e quantos anexos tem. O começo do texto fica numa opção. A caixa que seleciona a mensagem não é um item separado.
- **Menu Ações de cada e-mail.** Selecionar, Excluir, Marcar como lida ou não lida, Marcar com estrela e Mover para pasta. Com mensagens selecionadas, o menu age em todas elas, e há também Selecionar todas.
- **Foco.** Depois de selecionar ou desmarcar um e-mail, o foco fica nele. A próxima varrida vai para o e-mail de baixo.
- **E-mail aberto.** O menu Ações e comandos, para atribuir a gestos, têm Responder, Responder a todos, Encaminhar, Responder como nova, Mover para Excluídas, Marcar com estrela, Mostrar anexos e Dizer quem enviou. Ao abrir a mensagem, o controle de leitura vai para Ações, para que deslizar para cima ou para baixo passe por elas.

### Gravar e compartilhar (MHS), para todos os apps

- Um comando começa a gravar áudio em estéreo (AAC, 192 kbps, M4A). Usado de novo, para a gravação e abre o compartilhamento com o arquivo.
- Vibra ao começar e ao terminar. As gravações ficam em Música, na pasta `MHS_Recordings`.

### Descrever com IA (MHS), para todos os apps

- Quatro comandos: descrever o item em foco e descrever a tela inteira, cada um com o Be My Eyes e com o Seeing AI.
- A imagem vai direto ao app escolhido, sem lista de compartilhamento no meio. No item em foco, ela é recortada só nele.
- Vibra ao começar. Se o app não estiver instalado, abre a página dele na loja. No Be My Eyes, o comando da tela inteira volta em vez de descrever.

## Observações

- **WhatsApp, gestos de dois dedos:** para o SandFly entregar o deslize de dois dedos ao script, ligue **Tratar no SandFly os deslizes com dois dedos** nas configurações de Gestos (Android 11 ou mais novo).
- **WhatsApp mensagens, tela ligada:** para a tela não apagar enquanto uma mensagem de voz toca, o SandFly precisa ter permissão para **modificar as configurações do sistema**; o script sobe o tempo de tela para o máximo que o SandFly consegue pôr (30 minutos) e devolve o seu valor quando a mensagem termina ou quando você sai do WhatsApp. Sem a permissão, o script avisa uma vez e o resto continua funcionando. O script também pede a permissão **Área de transferência**, para copiar links, e-mails e telefones.
- **Viva-voz do WhatsApp:** o script usa o sensor de proximidade e o botão de viva-voz da tela da ligação, por isso pede a permissão **Java**, reservada a scripts de confiança, e fica carregado o tempo todo (a configuração **Viva-voz ao afastar da orelha** liga e desliga o recurso). Para funcionar com a tela apagada, ligue **Manter em execução com a tela desligada** na página do script. Só vale para ligações do WhatsApp; nas ligações comuns o SandFly já tem a sua opção própria. Quem tinha o script de mensagens 3.9 e usava o viva-voz deve instalar este também, porque ele saiu do script de mensagens.
- **Instagram:** para os dois dedos para cima e para baixo trocarem de reel, ligue **Tratar no SandFly os deslizes com dois dedos** nas configurações de Gestos (Android 11 ou mais novo). Os comandos de reels e stories não têm gesto até você atribuir um em **Comandos** > **Scripts**. Foi feito com o Instagram em português do Brasil; os textos em inglês são palpites.
- **YouTube:** o script tem um id próprio e não substitui o *YouTube video actions* original: se os dois estiverem instalados, as regras se repetem. Desative ou remova o original ao instalar este. Funciona com o YouTube e com o YouTube Morphe, em português do Brasil. O script não copia o endereço dos links da descrição, porque o YouTube não entrega o endereço inteiro ao leitor de telas.
- **Zello:** o script só mexe no botão de falar. Foi feito com o Zello em português do Brasil.
- **Cliques automáticos:** só roda quando você usa um dos comandos; atribua os que for usar a gestos em **Comandos** > **Scripts**.
- **Gravar e compartilhar:** o SandFly precisa da permissão de **Microfone** do Android (Configurações do Android > Apps > SandFly > Permissões). O script pede a permissão **Java**, reservada a scripts de confiança, porque usa o gravador e o compartilhamento do Android. Depois de instalar, atribua o comando **Gravar áudio e compartilhar** a um gesto em **Comandos** > **Scripts**.
- **Descrever com IA:** atribua os quatro comandos a gestos em **Comandos** > **Scripts**. O script pede as permissões **Java** e **Tela**, porque tira uma foto da tela e a envia ao outro app. A imagem é guardada na pasta temporária do SandFly e sai do celular só para o app que você escolheu. Telas protegidas, como as de alguns bancos, saem pretas. É preciso ter o Be My Eyes ou o Seeing AI instalado.
- **AquaMail:** não pede a permissão Java. Foi feito e testado com o AquaMail em português do Brasil; os textos em inglês dos menus são palpites. Para o controle de leitura ir para Ações ao abrir um e-mail, o script usa o comando do próprio SandFly que seleciona esse controle (dá para desligar na opção **Selecionar o controle de leitura Ações quando uma mensagem abre**). Excluir pode pedir confirmação no app; ela fica por sua conta.
- **Conversão para MP3:** o Android não tem codificador de MP3, então a gravação é em M4A (AAC). Para MP3, converta no computador.

## Novidades por versão

O que mudou em cada versão fica aqui, e não na descrição dos scripts.

- **WhatsApp mensagens:** 4.9 Ir para a mensagem respondida no menu Ações das respostas, também para citações de áudio, foto, vídeo e documento, com a espera ajustável. 4.8 dois toques baixam e reproduzem vídeos, também os sem identificação e os baixados em grupos. 4.7 álbuns de fotos e vídeos e o reprodutor de vídeo sem a leitura do progresso. 4.6 dois toques em vídeos. 4.5 velocidade de reprodução da mensagem de voz no menu Ações e rolagem da conversa mais fluida. 4.4 o foco acompanha a mensagem de voz que está tocando e a tela não apaga enquanto ela toca; a busca pela linha das mensagens não lidas rola direto, sem parar. 4.1 a 4.3 comandos Ir para a última mensagem e Encontrar a linha das mensagens não lidas (mesmo fora da tela), com a explicação do bug do WhatsApp na descrição. 4.0 copiar link, e-mail e telefone da mensagem; o viva-voz sai deste script e vira o Viva-voz do WhatsApp. 3.9 viva-voz ao afastar o celular da orelha nas ligações. 3.8 o microfone diz só "Gravar" e as instruções viram a dica de uso. 3.7 "Ler mais" mais tolerante e toque com três dedos para apertar o "Ler mais". 3.6.x ações do WhatsApp no menu Ações, textos do WhatsApp em português, mensagens de voz (avançar, voltar e dois toques, também nas que citam outra mensagem ou que você enviou), foco no Enviar ao gravar e dois toques que abrem documento.
- **Viva-voz do WhatsApp:** 2.0.0 passa a ser um script só dele, com o comando que diz o estado do áudio da ligação.
- **Instagram:** 2.3.0 perfil com o painel e as abas mais limpos. 2.0 a 2.2 Explorar, lista de conversas do Direct e mensagens de uma conversa aberta como uma linha só, com as ações no menu Ações. 1.8.0 mais botões da publicação no menu Ações (legenda inteira, perfil, vídeo, som, música, anúncio) e fora da varredura, sem números soltos. 1.x reels, stories, notificações, pessoas sugeridas, perfil e menu Ações do feed.
- **YouTube:** 1.5.0 a descrição do vídeo abre já expandida e os links dela ficam no menu Ações. 1.3.0 primeira versão publicada: o script de Aaron Hewitt em português, com a página do vídeo limpa.
- **Zello:** 1.3.1 primeira versão publicada: dois toques no botão de falar viram um toque na tela.
- **Google Mensagens:** 1.3.0 Selecionar mensagem no menu Ações das mensagens de uma conversa, menus em português e foco mantido no que foi selecionado.
- **Cliques automáticos:** 1.5 passos que ignoram números, toque longo, vagas de comando por sequência.
- **AquaMail:** 1.2.0 Responder como nova e controle de leitura Ações ao abrir o e-mail. 1.1.0 a caixa de selecionar deixa de ser um item separado, o e-mail aberto ganha menu Ações e o menu passa a responder mais rápido. 1.0.0 primeira versão.
- **Gravar e compartilhar:** 1.3 vibra direto pelo Android e só fala "Gravando em estéreo" se a opção estiver ligada. 1.2 avisa quando falta a permissão do microfone. 1.0 primeira versão.
- **Descrever com IA:** 1.1 funciona com o item em foco e com a tela inteira, no Be My Eyes e no Seeing AI. 1.0 primeira versão.

## Créditos e licença

- **WhatsApp mensagens (MHS)** é uma versão modificada do script *WhatsApp messages*, de Aaron Hewitt, publicado em [aaron-gh/sandfly-scripts](https://github.com/aaron-gh/sandfly-scripts) sob a licença Apache 2.0. As modificações são de Michel Henrique: ações do WhatsApp no menu Ações, suporte ao WhatsApp em português do Brasil, gestos de avançar e voltar mensagem de voz, foco no Enviar ao gravar, dois toques que abrem documento e tocam mensagem de voz, e tradução. Como o arquivo foi modificado, ele não leva mais a assinatura do SandFly, e o diálogo de instalação não mostra "Assinado pelo SandFly".
- **YouTube (MHS)** é uma versão adaptada do script *YouTube video actions*, de Aaron Hewitt, publicado em [aaron-gh/sandfly-scripts](https://github.com/aaron-gh/sandfly-scripts) sob a licença Apache 2.0. O código do original não foi mudado. As adaptações são de Michel Henrique: português do Brasil, um id próprio e as regras da página do vídeo. Como o arquivo foi modificado, ele não leva mais a assinatura do SandFly. YouTube é marca dos respectivos donos; este script não tem relação com ele.
- **Google Mensagens (MHS)** é uma versão adaptada do script *Google Messages conversation actions*, de Surendra, sob a licença Apache 2.0. As adaptações são de Michel Henrique: português do Brasil, os menus do Google Mensagens em português e Selecionar mensagem no menu Ações das mensagens de uma conversa. Google Mensagens é marca dos respectivos donos; este script não tem relação com ele.
- **Viva-voz do WhatsApp (MHS)**, **Instagram (MHS)**, **Zello (MHS)** e **Cliques automáticos (MHS)** são da MHS Softwares. WhatsApp, Instagram e Zello são marcas dos respectivos donos; estes scripts não têm relação com eles e só ajudam o leitor de telas a usar os apps instalados.
- **Gravar e compartilhar (MHS)** é da MHS Softwares, a partir de um plugin para o leitor de telas JieShuo.
- **Descrever com IA (MHS)** é da MHS Softwares, a partir de plugins para o leitor de telas JieShuo. Be My Eyes e Seeing AI são marcas dos respectivos donos; este script não tem relação com eles e só envia a imagem aos apps instalados.
- **AquaMail (MHS)** é da MHS Softwares. AquaMail é marca dos respectivos donos; este script não tem relação com eles e só ajuda o leitor de telas a usar o app instalado.

Os scripts estão sob a licença Apache 2.0. Veja [LICENSE](LICENSE).

---

**In English:** Lua scripts for the SandFly screen reader for Android, in Brazilian Portuguese. Add the repository as a script source with `github.com/MHS-Softwares/Scripts-MHS-para-Sandfly`. It has a modified WhatsApp script (based on Aaron Hewitt's, Apache 2.0; it also finds the unread-messages line in long chats, follows the voice message that is playing and keeps the screen on, changes the voice message speed from the Actions menu and plays or downloads videos with a double tap), a separate script that turns the speaker on in WhatsApp calls when you move the phone from your ear, a script for Instagram (reels, stories, feed posts, Explore, profile, notifications and Direct messages), an adapted YouTube script (based on Aaron Hewitt's, Apache 2.0; the buttons of the video page go to the Actions menu), an adapted Google Messages script (based on Surendra's, Apache 2.0), automatic clicks (a sequence of buttons pressed one after another), a script for the AquaMail e-mail app (short reading of the message list, Actions menu with selection and reply, focus kept after selecting), a record-and-share command, and commands that send the focused item or the whole screen to Be My Eyes or Seeing AI. Apache License 2.0.
