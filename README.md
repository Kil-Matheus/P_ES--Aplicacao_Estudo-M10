# P_ES--Aplicacao_Estudo-M10
A atividade escolhida foi a local_notifications

## Integrantes (Grupo 6)
Alberto
Daniel
Igor
João
Kil 
Luíz

## Processo de criação

O pacote `awesome_notifications` é uma ferramenta poderosa para lidar com notificações no Flutter. Ele fornece uma série de recursos para criar e gerenciar notificações de uma forma altamente personalizável e eficiente.

Algumas das principais características do `awesome_notifications` incluem:

1. **Canais de Notificação Personalizados**: Permite criar canais de notificação personalizados para agrupar e gerenciar diferentes tipos de notificações.

2. **Notificações Personalizadas**: Oferece suporte a uma ampla variedade de tipos de notificações personalizadas, como texto, imagem, vídeo, ações interativas e muito mais.

3. **Agendamento de Notificações**: Permite agendar notificações para serem exibidas em momentos específicos no futuro, facilitando a implementação de lembretes e alertas.

4. **Compatibilidade com Plataformas**: Funciona em várias plataformas, incluindo Android e iOS, garantindo uma experiência consistente para os usuários em diferentes dispositivos.

5. **Gerenciamento Avançado de Notificações**: Fornece métodos para gerenciar notificações, como cancelar, atualizar e agendar novamente, oferecendo controle total sobre o ciclo de vida das notificações.

O `awesome_notifications` é inicializado na função `main()` do aplicativo, onde é definido um canal de notificação básico. Além disso, no método `initState()` da classe `MyApp`, é verificado se as notificações estão permitidas e, se não estiverem, é solicitada permissão para enviá-las. Isso demonstra como o pacote é integrado ao aplicativo para lidar com notificações de forma eficaz e responsável.

## local_notifications.dart

### Descrição
Este arquivo contém a implementação de uma tela que permite ao usuário agendar notificações locais para serem exibidas após um determinado período de tempo.

### Funções e Classes

#### `toScheduleNotification(int value)`

- **Descrição**: Uma função assíncrona que aguarda um determinado período de tempo especificado em segundos e, em seguida, cria e exibe uma notificação local utilizando o pacote `awesome_notifications`.
  
- **Parâmetros**:
  - `value`: Um inteiro representando o tempo em segundos para agendar a notificação.

#### `LocalNotifications`

- **Descrição**: Um StatefulWidget que representa a tela de agendamento de notificações locais.

- **Widgets Principais**:
  - `Scaffold`: Um widget que fornece uma estrutura básica para construir a interface do usuário, incluindo uma AppBar e um corpo centralizado.
  - `AppBar`: Uma barra de aplicativo que exibe o título "Agendamento de Notificações".
  - `Text`: Um widget para exibir um texto informativo sobre o propósito da tela.
  - `TextField`: Um campo de entrada de texto onde o usuário pode digitar o tempo em segundos para agendar a notificação.
  - `IconButton`: Um botão de ícone que, quando pressionado, lê o valor digitado no `TextField` e chama a função `toScheduleNotification` para agendar a notificação.
  
- **Estado**:
  - `_LocalNotificationsState`: O estado da tela que mantém o controle do texto digitado pelo usuário no `TextField`.

### Observações
- A função `toScheduleNotification` utiliza o pacote `awesome_notifications` para criar e exibir uma notificação local após um determinado período de tempo.
- A tela permite ao usuário digitar o tempo desejado em segundos e agendar a notificação pressionando um botão de ícone.
- Um ícone de tomate é exibido ao lado do botão de agendamento como um elemento visual adicional.