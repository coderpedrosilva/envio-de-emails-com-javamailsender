# envio-de-emails-com-javamailsender

O código apresentado demonstra como configurar a funcionalidade de envio de e-mails utilizando o 
Spring Framework e a biblioteca JavaMailSender. O sistema é configurado para se comunicar com o 
servidor SMTP do Gmail e enviar e-mails a partir dele. Há uma conexão com o banco de dados PostgreSQL.

## Configuração
### EmailConfig.java
O arquivo **'EmailConfig.java'** contém a configuração necessária para estabelecer a comunicação com o 
servidor SMTP do Gmail. Nele, são definidas propriedades como host, porta, nome de usuário e 
senha, necessárias para autenticação e envio de e-mails.

### mail.properties
O arquivo **'mail.properties'** contém as configurações base para o envio de e-mails. Nele, é possível 
definir o host do servidor SMTP, a porta, o nome de usuário (geralmente seu endereço de e-mail 
Gmail) e a senha de aplicativo gerada no Gmail.

### Configuração no Gmail
1. Para que o sistema possa enviar e-mails pelo Gmail, é necessário seguir as seguintes etapas:

2. Ativar a **'Verificação em Duas Etapas'** na sua conta do Gmail, se ainda não estiver ativada.

3. Gerar uma **'Senha de Aplicativo'** para o sistema. Isso é feito na seção "Senhas de app" nas 
configurações de segurança da sua conta do Google. Selecione a opção "Outro (Personalizado)" 
e, em seguida, escolha "Aplicativo" e "Java" (ou a opção mais adequada para o seu caso).

A senha gerada será usada como a senha de acesso no código do sistema.

## Como Usar
1. Clone este repositório para o seu ambiente de desenvolvimento.

2. Edite o arquivo **'mail.properties'** e substitua as informações pelo seu endereço de e-mail Gmail
e a senha de aplicativo gerada.

3. Configure o envio de e-mails no arquivo **'usuario.http'** substituindo seus campos.

Lembre-se de que a segurança é fundamental ao lidar com credenciais de e-mail. Certifique-se de não 
compartilhar ou expor suas informações de autenticação.

Este exemplo oferece uma base sólida para implementar um sistema de envio de e-mails via Gmail. 
Sinta-se à vontade para adaptá-lo de acordo com as necessidades específicas do seu projeto

Conteúdo desenvolvido com base nas aulas do professor Weberson Rodrigues na Udemy.
