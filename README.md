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

| Arquivo | App | O que faz |
|---|---|---|
| `whatsapp-mensagens-mhs.zip` | WhatsApp e WhatsApp Business | Lê cada mensagem como um item só (quem enviou, conteúdo, mensagem respondida e hora). As ações do WhatsApp, como responder, encaminhar e compartilhar, ficam no menu Ações. Dois toques tocam a mensagem de voz, mesmo as que você enviou ou que citam outra mensagem, e abrem o documento, em vez de apertar Encaminhar. Dois dedos para a direita avançam e para a esquerda voltam a mensagem de voz. Ao gravar uma mensagem de voz tocando no microfone, o foco vai para o Enviar, sem falar. Mensagens longas abrem o "Ler mais" sozinhas ao receber o foco, e um toque com três dedos aperta o "Ler mais" da mensagem em foco. O botão do microfone diz só "Gravar", e as instruções dele só são faladas com as dicas de uso do SandFly ligadas. Nas ligações do WhatsApp, afastar o celular da orelha liga o viva-voz e aproximar de novo volta para o fone de ouvido, só com uma vibração curta, sem o leitor falar. |
| `gravar-e-compartilhar-mhs.zip` | Todos os apps | Um comando que começa a gravar áudio em estéreo (AAC, 192 kbps, M4A) e, ao ser usado de novo, para e abre o compartilhamento com a gravação. Vibra ao começar e ao terminar. As gravações ficam em Música, na pasta `MHS_Recordings`. |
| `descrever-com-ia-mhs.zip` | Todos os apps | Quatro comandos que mandam uma imagem direto ao **Be My Eyes** ou ao **Seeing AI**, que a descrevem: descrever o item em foco (a imagem é recortada só nele) e descrever a tela inteira, em cada um dos dois apps. Sem lista de compartilhamento no meio. Vibra ao começar. Se o app não estiver instalado, abre a página dele na loja. No Be My Eyes, o comando da tela inteira volta em vez de descrever. |
| `aquamail-mhs.zip` | AquaMail | Na lista de mensagens, cada e-mail é lido de um jeito curto: o estado, quem enviou, o assunto, a hora e quantos anexos tem (o começo do texto fica numa opção). A caixa que seleciona a mensagem não é um item separado. O menu Ações de cada e-mail tem Selecionar, Excluir, Marcar como lida ou não lida, Marcar com estrela e Mover para pasta, e, com mensagens selecionadas, age em todas elas (inclusive Selecionar todas). Depois de selecionar, o foco fica na mensagem. Com um e-mail aberto, o menu Ações e comandos (para atribuir a gestos) têm Responder, Responder a todos, Encaminhar, Responder como nova, Mover para Excluídas, Marcar com estrela, Mostrar anexos e Dizer quem enviou; e, ao abrir a mensagem, o controle de leitura vai para Ações. |

### Observações

- **WhatsApp, gestos de dois dedos:** para o SandFly entregar o deslize de dois dedos ao script, ligue **Tratar no SandFly os deslizes com dois dedos** nas configurações de Gestos (Android 11 ou mais novo).
- **WhatsApp, viva-voz ao afastar da orelha:** o script usa o sensor de proximidade e o botão de viva-voz da tela da ligação, por isso pede a permissão **Java**, reservada a scripts de confiança, e fica carregado o tempo todo (a configuração **Viva-voz ao afastar da orelha** liga e desliga o recurso). Para funcionar com a tela apagada, ligue **Manter em execução com a tela desligada** na página do script. Só vale para ligações do WhatsApp; nas ligações comuns o SandFly já tem a sua opção própria.
- **Gravar e compartilhar:** o SandFly precisa da permissão de **Microfone** do Android (Configurações do Android > Apps > SandFly > Permissões). O script pede a permissão **Java**, reservada a scripts de confiança, porque usa o gravador e o compartilhamento do Android. Depois de instalar, atribua o comando **Gravar áudio e compartilhar** a um gesto em **Comandos** > **Scripts**.
- **Descrever com IA:** atribua os quatro comandos a gestos em **Comandos** > **Scripts**. O script pede as permissões **Java** e **Tela**, porque tira uma foto da tela e a envia ao outro app. A imagem é guardada na pasta temporária do SandFly e sai do celular só para o app que você escolheu. Telas protegidas, como as de alguns bancos, saem pretas. É preciso ter o Be My Eyes ou o Seeing AI instalado.
- **AquaMail:** não pede a permissão Java. Foi feito e testado com o AquaMail em português do Brasil; os textos em inglês dos menus são palpites. Para o controle de leitura ir para Ações ao abrir um e-mail, o script usa o comando do próprio SandFly que seleciona esse controle (dá para desligar na opção **Selecionar o controle de leitura Ações quando uma mensagem abre**). Excluir pode pedir confirmação no app; ela fica por sua conta.
- **Conversão para MP3:** o Android não tem codificador de MP3, então a gravação é em M4A (AAC). Para MP3, converta no computador.

## Créditos e licença

- **WhatsApp mensagens (MHS)** é uma versão modificada do script *WhatsApp messages*, de Aaron Hewitt, publicado em [aaron-gh/sandfly-scripts](https://github.com/aaron-gh/sandfly-scripts) sob a licença Apache 2.0. As modificações são de Michel Henrique: ações do WhatsApp no menu Ações, suporte ao WhatsApp em português do Brasil, gestos de avançar e voltar mensagem de voz, foco no Enviar ao gravar, dois toques que abrem documento e tocam mensagem de voz, e tradução. Como o arquivo foi modificado, ele não leva mais a assinatura do SandFly, e o diálogo de instalação não mostra "Assinado pelo SandFly".
- **Gravar e compartilhar (MHS)** é da MHS Softwares, a partir de um plugin para o leitor de telas JieShuo.
- **Descrever com IA (MHS)** é da MHS Softwares, a partir de plugins para o leitor de telas JieShuo. Be My Eyes e Seeing AI são marcas dos respectivos donos; este script não tem relação com eles e só envia a imagem aos apps instalados.

- **AquaMail (MHS)** é da MHS Softwares. AquaMail é marca dos respectivos donos; este script não tem relação com eles e só ajuda o leitor de telas a usar o app instalado.

Os scripts estão sob a licença Apache 2.0. Veja [LICENSE](LICENSE).

---

**In English:** Lua scripts for the SandFly screen reader for Android, in Brazilian Portuguese. Add the repository as a script source with `github.com/MHS-Softwares/Scripts-MHS-para-Sandfly`. It has a modified WhatsApp script (based on Aaron Hewitt's, Apache 2.0) and a record-and-share command, commands that send the focused item or the whole screen to Be My Eyes or Seeing AI, and a script for the AquaMail e-mail app (short reading of the message list, Actions menu with selection and reply, focus kept after selecting). Apache License 2.0.
