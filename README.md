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
| `whatsapp-mensagens-mhs.zip` | WhatsApp e WhatsApp Business | Cada mensagem de uma conversa é lida como um item só, com as ações dela no menu Ações; ajuda com mensagens de voz, documentos, "Ler mais", o botão do microfone e o viva-voz nas ligações. |
| `aquamail-mhs.zip` | AquaMail | Cada e-mail da lista é lido de forma curta (quem enviou, assunto, hora, anexos); o menu Ações seleciona, exclui, arquiva e responde, e o foco fica na mensagem selecionada. |
| `gravar-e-compartilhar-mhs.zip` | Todos os apps | Um comando grava áudio em estéreo e, ao ser usado de novo, para e abre o compartilhamento com a gravação. |
| `descrever-com-ia-mhs.zip` | Todos os apps | Comandos que mandam o item em foco, ou a tela inteira, ao Be My Eyes ou ao Seeing AI, que descrevem a imagem. |

## O que cada script faz

### WhatsApp mensagens (MHS), para o WhatsApp e o WhatsApp Business

- **Uma mensagem, um item.** Cada mensagem é lida com quem enviou, o conteúdo, a mensagem que ela responde e a hora. Na lista de conversas, deslizar pula a foto de cada conversa, que abre o perfil pelo menu Ações da conversa.
- **Menu Ações de cada mensagem.** Tocar, a velocidade de reprodução e os outros botões da mensagem ficam no menu Ações, junto com as ações do próprio WhatsApp: responder, encaminhar, compartilhar e outras.
- **Mensagens de voz.** Dois toques tocam a mensagem, mesmo as que você enviou ou que citam outra mensagem. Dois dedos para a direita avançam e dois dedos para a esquerda voltam.
- **Gravar mensagem de voz.** Ao começar a gravar tocando no microfone, sem segurar, o foco vai para o Enviar em vez do Pausar, sem o leitor falar.
- **Documentos.** Dois toques abrem o documento, em vez de apertar Encaminhar.
- **Mensagens longas.** O "Ler mais" abre sozinho quando a mensagem recebe o foco. Um toque com três dedos aperta o "Ler mais" da mensagem em foco e lê tudo.
- **Botão do microfone.** Diz só "Gravar". As instruções dele só são faladas com as dicas de uso do SandFly ligadas.
- **Ligações do WhatsApp.** Afastar o celular da orelha liga o viva-voz; aproximar de novo volta para o fone de ouvido. Só uma vibração curta avisa, sem o leitor falar.
- **Idiomas.** Funciona com o WhatsApp em português do Brasil e em inglês.

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
- **WhatsApp, viva-voz ao afastar da orelha:** o script usa o sensor de proximidade e o botão de viva-voz da tela da ligação, por isso pede a permissão **Java**, reservada a scripts de confiança, e fica carregado o tempo todo (a configuração **Viva-voz ao afastar da orelha** liga e desliga o recurso). Para funcionar com a tela apagada, ligue **Manter em execução com a tela desligada** na página do script. Só vale para ligações do WhatsApp; nas ligações comuns o SandFly já tem a sua opção própria.
- **Gravar e compartilhar:** o SandFly precisa da permissão de **Microfone** do Android (Configurações do Android > Apps > SandFly > Permissões). O script pede a permissão **Java**, reservada a scripts de confiança, porque usa o gravador e o compartilhamento do Android. Depois de instalar, atribua o comando **Gravar áudio e compartilhar** a um gesto em **Comandos** > **Scripts**.
- **Descrever com IA:** atribua os quatro comandos a gestos em **Comandos** > **Scripts**. O script pede as permissões **Java** e **Tela**, porque tira uma foto da tela e a envia ao outro app. A imagem é guardada na pasta temporária do SandFly e sai do celular só para o app que você escolheu. Telas protegidas, como as de alguns bancos, saem pretas. É preciso ter o Be My Eyes ou o Seeing AI instalado.
- **AquaMail:** não pede a permissão Java. Foi feito e testado com o AquaMail em português do Brasil; os textos em inglês dos menus são palpites. Para o controle de leitura ir para Ações ao abrir um e-mail, o script usa o comando do próprio SandFly que seleciona esse controle (dá para desligar na opção **Selecionar o controle de leitura Ações quando uma mensagem abre**). Excluir pode pedir confirmação no app; ela fica por sua conta.
- **Conversão para MP3:** o Android não tem codificador de MP3, então a gravação é em M4A (AAC). Para MP3, converta no computador.

## Novidades por versão

O que mudou em cada versão fica aqui, e não na descrição dos scripts.

- **WhatsApp mensagens:** 3.9 viva-voz ao afastar o celular da orelha nas ligações. 3.8 o microfone diz só "Gravar" e as instruções viram a dica de uso. 3.7 "Ler mais" mais tolerante e toque com três dedos para apertar o "Ler mais". 3.6.x ações do WhatsApp no menu Ações, textos do WhatsApp em português, mensagens de voz (avançar, voltar e dois toques, também nas que citam outra mensagem ou que você enviou), foco no Enviar ao gravar e dois toques que abrem documento.
- **AquaMail:** 1.2.0 Responder como nova e controle de leitura Ações ao abrir o e-mail. 1.1.0 a caixa de selecionar deixa de ser um item separado, o e-mail aberto ganha menu Ações e o menu passa a responder mais rápido. 1.0.0 primeira versão.
- **Gravar e compartilhar:** 1.3 vibra direto pelo Android e só fala "Gravando em estéreo" se a opção estiver ligada. 1.2 avisa quando falta a permissão do microfone. 1.0 primeira versão.
- **Descrever com IA:** 1.1 funciona com o item em foco e com a tela inteira, no Be My Eyes e no Seeing AI. 1.0 primeira versão.

## Créditos e licença

- **WhatsApp mensagens (MHS)** é uma versão modificada do script *WhatsApp messages*, de Aaron Hewitt, publicado em [aaron-gh/sandfly-scripts](https://github.com/aaron-gh/sandfly-scripts) sob a licença Apache 2.0. As modificações são de Michel Henrique: ações do WhatsApp no menu Ações, suporte ao WhatsApp em português do Brasil, gestos de avançar e voltar mensagem de voz, foco no Enviar ao gravar, dois toques que abrem documento e tocam mensagem de voz, e tradução. Como o arquivo foi modificado, ele não leva mais a assinatura do SandFly, e o diálogo de instalação não mostra "Assinado pelo SandFly".
- **Gravar e compartilhar (MHS)** é da MHS Softwares, a partir de um plugin para o leitor de telas JieShuo.
- **Descrever com IA (MHS)** é da MHS Softwares, a partir de plugins para o leitor de telas JieShuo. Be My Eyes e Seeing AI são marcas dos respectivos donos; este script não tem relação com eles e só envia a imagem aos apps instalados.
- **AquaMail (MHS)** é da MHS Softwares. AquaMail é marca dos respectivos donos; este script não tem relação com eles e só ajuda o leitor de telas a usar o app instalado.

Os scripts estão sob a licença Apache 2.0. Veja [LICENSE](LICENSE).

---

**In English:** Lua scripts for the SandFly screen reader for Android, in Brazilian Portuguese. Add the repository as a script source with `github.com/MHS-Softwares/Scripts-MHS-para-Sandfly`. It has a modified WhatsApp script (based on Aaron Hewitt's, Apache 2.0), a script for the AquaMail e-mail app (short reading of the message list, Actions menu with selection and reply, focus kept after selecting), a record-and-share command, and commands that send the focused item or the whole screen to Be My Eyes or Seeing AI. Apache License 2.0.
