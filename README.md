# Linux-desktop-launch-app
Crie lançadores para seus executáveis e os torne aplicativos visíveis com ícones.
> O [Desktop Entry] é uma seção em um arquivo .desktop, que é usado para definir as informações de um aplicativo para ambientes desktop Linux. Ele contém informações sobre o aplicativo, como o nome, comentário, ícone, categoria e comando para executar o aplicativo. Quando um arquivo .desktop é instalado em um sistema, essas informações são usadas para criar um atalho para o aplicativo no menu do ambiente desktop, permitindo que os usuários iniciem facilmente o aplicativo a partir daí. 

> Além disso, o [Desktop Entry] também pode conter outras informações, como ações personalizadas que podem ser executadas no aplicativo, parâmetros para serem usados na execução do aplicativo, informações sobre o autor e muito mais. Em geral, é uma parte fundamental na criação e distribuição de aplicativos Linux, permitindo que os desenvolvedores especifiquem todas as informações necessárias para que o aplicativo seja exibido corretamente no menu do ambiente desktop e seja facilmente acessível pelos usuários.

Aqui está um exemplo de um `arquivo.desktop`:
```.desktop
[Desktop Entry]
Name=Nome do aplicativo
StartupWMClass=Nome do aplicativo
Comment=Comentário sobre o app
Exec=Diretório onde o executável se encontra
Icon=Diretório onde o ícone .png ou .svg se econtra
Type=Application
Categories=Categoria1;Categoria2;etc
```
Basta editar os valores adequados ao seu app e inserir o `arquivo.desktop` no seguinte diretório:

```bash
/usr/share/applications
```

## Principais parâmetros [Desktop Entry]
- **Name:** Especifica o nome do aplicativo que será exibido no menu do ambiente desktop.

- **Exec:** Especifica o comando necessário para executar o aplicativo. Esse comando pode incluir caminhos para executáveis, arquivos de script e parâmetros.

- **Icon:** Especifica o ícone que será usado para representar o aplicativo no menu do ambiente desktop.

- **Type:**  Especifica o tipo de arquivo, que é "Application" para aplicativos.

- **Categories:** Especifica as categorias nas quais o aplicativo deve ser listado no menu do ambiente desktop, como "Internet" ou "Multimídia". As categorias são separadas por ponto-e-vírgula.

- **Comment:** Especifica uma descrição curta do aplicativo que será exibida no menu do ambiente desktop.

- **Terminal:** Especifica se o aplicativo deve ser executado em um terminal. Se for definido como "true", o terminal será aberto quando o aplicativo for executado.

- **StartupNotify:** Especifica se o ambiente desktop deve mostrar uma mensagem de notificação quando o aplicativo for iniciado.

- **Actions:** Especifica as ações que o usuário pode executar para um determinado tipo de arquivo. Por exemplo, um editor de texto pode ter ações para "Abrir" ou "Salvar".

- **Keywords:** Especifica palavras-chave que ajudam a descrever o aplicativo e que podem ser usadas para pesquisá-lo no menu do ambiente desktop.
