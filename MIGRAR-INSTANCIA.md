# Migrando de uma instância para outra

Este é o passo-a-passo de como migrar sua conta no mastodon de uma instância para outra. Você pode migrar tudo (seguidores, seguidos, silenciados e bloqueados) exceto seus toots e mídia, você pode exportá-los mas não pode importá-los na nova instância.

Primeiro de tudo, para migrar de uma instância para outra, você deve fazer uma nova conta na instância para a qual você quer mudar, então siga os passos abaixo:

1.  **Na nova instância** vá em `Preferências` > `Conta` > `Configurações da conta`

    ![migrate-1](images/screenshots/migrar-instancia/migrate-1.png)

    Role a página, e em `Migrando de outra conta`, clique em `Criar um alias`

    ![migrate-1](images/screenshots/migrar-instancia/migrate-2.png)

2.  Coloque o seu nome de usuário da instância que você está saindo (você encontra ele logo abaixo da sua foto no seu perfil)

    ![migrate-1](images/screenshots/migrar-instancia/migrate-3.png)

3.  **Na instância antiga** faça **backup** dos seus dados em `Preferências` > `Importar e exportar` > `Exportar dados`

    ![Exportar dados](images/screenshots/migrar-instancia/migrate-4.png)

    Salve cada um dos arquivos disponíveis (não é possível salvar toots e seguidores nesse formato)

    ![Exportar dados](images/screenshots/migrar-instancia/migrate-5.png)

5. Em seguida **importe** esses aquivos **na nova instância** em `Preferências` > `Importar e exportar` > `Importar`.

    ![Exportar dados](images/screenshots/migrar-instancia/migrate-6a.png)

    Selecione o tipo de arquivo no menu `Tipo de importação`.

    ![Exportar dados](images/screenshots/migrar-instancia/migrate-6.png)

    Escolha o arquivo a ser importado e então selecione se você quer `Juntar` ou `Sobrescrever` o arquivo existente. 

    Ao `Juntar` você **adiciona** o que tinha na instância antiga com o que tem na nova.

    Ao `Sobrescrever` você **apaga** o que tem na nova e mantém **apenas** o que estava na antiga.

    Clique `Enviar`.
    
    Repita o procedimento para cada arquivo:
    -   Pessoas que você segue: `following_accounts.csv`
    -   Lista de bloqueio: `blocked_accounts.csv`
    -   Lista de silenciados: `muted_accounts.csv`
    -   Lista de dominios bloqueados: `blocked_domains.csv`


6. Agora voltando para **a instância antiga**, vá em `Preferências` > `Conta` > `Configurações da conta`

    ![migrate-1](images/screenshots/migrar-instancia/migrate-1.png)

    Role a página e em `Mudar-se para outra conta`, clique em `configurar isso aqui`.

    ![Exportar dados](images/screenshots/migrar-instancia/migrate-7.png)

7. Coloque seu nome de usuário **da nova instância** e clique em `Migrar seguidores`.

    ![Exportar dados](images/screenshots/migrar-instancia/migrate-8.png)
    
    Existe a possibilidade deste último passo não funcionar, pois a instância antiga ainda não sabe da existência do alias da nova, caso aconteça tente novamente mais tarde.

Pronto! Você migrou para uma nova instância!
