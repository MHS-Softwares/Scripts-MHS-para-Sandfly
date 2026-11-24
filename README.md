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
| `whatsapp-mensagens-mhs.zip` | WhatsApp e WhatsApp Business | Lê cada mensagem como um item só (quem enviou, conteúdo, mensagem respondida e hora). As ações do WhatsApp, como responder, encaminhar e compartilhar, ficam no menu Ações. Dois toques tocam a mensagem de voz, mesmo as que você enviou ou que citam outra mensagem, e abrem o documento, em vez de apertar Encaminhar. Dois dedos para a direita avançam e para a esquerda voltam a mensagem de voz. Ao gravar uma mensagem de voz tocando no microfone, o foco vai para o Enviar, sem falar. |
| `gravar-e-compartilhar-mhs.zip` | Todos os apps | Um comando que começa a gravar áudio em estéreo (AAC, 192 kbps, M4A) e, ao ser usado de novo, para e abre o compartilhamento com a gravação. Vibra ao começar e ao terminar. As gravações ficam em Música, na pasta `MHS_Recordings`. |

### Observações

- **WhatsApp, gestos de dois dedos:** para o SandFly entregar o deslize de dois dedos ao script, ligue **Tratar no SandFly os deslizes com dois dedos** nas configurações de Gestos (Android 11 ou mais novo).
- **Gravar e compartilhar:** o SandFly precisa da permissão de **Microfone** do Android (Configurações do Android > Apps > SandFly > Permissões). O script pede a permissão **Java**, reservada a scripts de confiança, porque usa o gravador e o compartilhamento do Android. Depois de instalar, atribua o comando **Gravar áudio e compartilhar** a um gesto em **Comandos** > **Scripts**.
- **Conversão para MP3:** o Android não tem codificador de MP3, então a gravação é em M4A (AAC). Para MP3, converta no computador.

## Créditos e licença

- **WhatsApp mensagens (MHS)** é uma versão modificada do script *WhatsApp messages*, de Aaron Hewitt, publicado em [aaron-gh/sandfly-scripts](https://github.com/aaron-gh/sandfly-scripts) sob a licença Apache 2.0. As modificações são de Michel Henrique: ações do WhatsApp no menu Ações, suporte ao WhatsApp em português do Brasil, gestos de avançar e voltar mensagem de voz, foco no Enviar ao gravar, dois toques que abrem documento e tocam mensagem de voz, e tradução. Como o arquivo foi modificado, ele não leva mais a assinatura do SandFly, e o diálogo de instalação não mostra "Assinado pelo SandFly".
- **Gravar e compartilhar (MHS)** é da MHS Softwares, a partir de um plugin para o leitor de telas JieShuo.

Os scripts estão sob a licença Apache 2.0. Veja [LICENSE](LICENSE).

---

**In English:** Lua scripts for the SandFly screen reader for Android, in Brazilian Portuguese. Add the repository as a script source with `github.com/MHS-Softwares/Scripts-MHS-para-Sandfly`. It has a modified WhatsApp script (based on Aaron Hewitt's, Apache 2.0) and a record-and-share command. Apache License 2.0.
