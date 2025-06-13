
---

# Análise de Sentimentos com Linguagem Studio no Azure AI

Projeto consiste descrever a utilização de dois recurso do Azure AI, onde estara sendo usado os recursos Speech Playground e AI Azure language

## Explorando a conversão de fala para texto no Azure AI Foundryetts Speech Playground

Vamos experimentar o recurso de conversão de fala em texto usando o Azure AI Foundryetts Speech Playground.

Na página **Fala**, role até a seção **Experimente os recursos de fala** e selecione a opção **Transcrição em tempo real**. Isso o levará diretamente ao *Speech Playground*.

Acesse o link [https://aka.ms/mslearn-speech-files](https://aka.ms/mslearn-speech-files) para baixar o arquivo `discurso.zip` e, em seguida, extraia seu conteúdo.

Na área **Carregar arquivos**, clique em **Procurar arquivos** e navegue até a pasta onde você salvou o arquivo extraído. Escolha o arquivo `O queAICanDo.m4a` e clique em **Abrir**.

### Visualização e revisão da transcrição em tempo real

O serviço de fala transcreve e exibe o texto à medida que o áudio é reproduzido, em tempo real. Se você tiver o áudio salvo no seu computador, é possível escutá-lo enquanto acompanha a transcrição sendo gerada simultaneamente.

Após a reprodução, revise o resultado: o sistema deverá ter reconhecido e convertido corretamente o conteúdo falado em texto.

Neste exercício, você experimentou os serviços de fala do Azure AI por meio do *Speech Playground* disponível no Azure AI Foundry. Você utilizou o recurso de **transcrição em tempo real** para converter uma gravação de áudio, observando o texto aparecer progressivamente conforme o áudio era reproduzido.

### Encerramento e limpeza de recursos

Se pretende continuar com outros exercícios, é recomendável excluir os recursos que não serão mais utilizados, evitando assim custos desnecessários.

#### Para isso:

1. Acesse o **Portal do Azure**.
2. Localize e selecione o **grupo de recursos** que contém os elementos criados.
3. Clique no **recurso** desejado.
4. Selecione **Excluir** e, em seguida, confirme em **Sim**.

O recurso será então removido do ambiente.

---


# Analisar texto no portal Azure AI Foundry

## Processamento de Linguagem Natural (NLP)
Processamento de Linguagem Natural (NLP) é um ramo da IA que lida com linguagem escrita e falada. Você pode usar a PNL para construir soluções que:
- Extraem significado semântico de texto ou fala
- Formulam respostas significativas em linguagem natural

O serviço **Azure AI Language** inclui o **Text Analytics**, com recursos como:
- **Reconhecimento de entidade**
- **Extração de frase-chave**
- **Sumarização**
- **Análise de sentimento**

Por exemplo, suponha que o agente de viagens fictício *Margie' Travel* incentive os clientes a enviar comentários para estadias em hotéis. Você pode usar o **Azure AI Language** para:
- Extrair entidades nomeadas
- Identificar frases-chave
- Resumir texto
- Muito mais

---

## Criar um projeto no portal Azure AI Foundry
1. Em um navegador da web, abra o **Portal Azure AI Foundry** em [https://ai.azure.com](https://ai.azure.com) e entre com suas credenciais do Azure.
2. Feche todas as dicas ou painéis de início rápido que forem abertos na primeira vez que você entrar.
3. Navegue para [https://ai.azure.com/managementCenter/allResources](https://ai.azure.com/managementCenter/allResources) e selecione **Criar**.
4. Escolha a opção para **criar um novo recurso** no Azure AI Foundry.
5. No assistente de **Criar um projeto**, insira um nome válido para o seu projeto.
6. Expanda **Opções avançadas** para especificar as seguintes configurações:
   - **Assinatura**: Sua assinatura do Azure
   - **Grupo de recursos**: Criar ou selecionar um grupo de recursos
   - **Região**: Selecione um dos seguintes locais:
     - Leste dos EUA
     - França Central
     - Coreia Central
     - Europa Ocidental
     - Oeste dos EUA
7. Aguarde até que seu projeto e hub sejam criados.

---

## Extrair entidades nomeadas
Entidades nomeadas são palavras que descrevem pessoas, lugares e objetos com nomes próprios. O **Azure AI Language** usa a capacidade de **extração de entidade nomeada** para identificar tipos de informações em uma revisão.

### Passos:
1. No **playground Linguagem**, selecione **Extrair informações**.
2. Escolha **Extrair entidades nomeadas**.
3. Sob **Amostra**, copie e cole a seguinte revisão:
#
**Tired hotel with poor service The Royal Hotel, London, United Kingdom 5/6/2018 This is an old hotel (has been around since 1950's) and the room furnishings are average...**
#
4. Selecione **Abrir** e reveja as frases extraídas.

---

## Resumir texto
O **Azure AI Language** possui recursos de **sumarização** para extrair informações essenciais.

### Passos:
1. No **playground Linguagem**, selecione **Resuma informações**.
2. Escolha **Resumir texto**.
3. Sob **Amostra**, copie e cole a seguinte revisão:
#
**Very noisy and rooms are tiny The Lombard Hotel, San Francisco, USA 9/5/2018 Hotel is located on Lombard street which is a very busy SIX lane street...**
#
4. Selecione **Abrir** e reveja o resumo gerado.

---

## Limpeza de recursos
Caso não pretenda continuar os exercícios, exclua os recursos para evitar custos desnecessários.

### Passos:
1. Acesse o **Portal do Azure** em [https://portal.azure.com](https://portal.azure.com).
2. Selecione o grupo de recursos que contém os recursos criados.
3. Escolha os recursos e clique em **Excluir**.
4. Confirme a exclusão selecionando **Sim**.


