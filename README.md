Repositório com o arquivo para fazer a conexão do GitHub com o servidor.

Instruções:
- Gerar uma chave .ssh no servidor
  - ssh-keygen -t ed25519 -C "mail@xample.com"
- Fazer um arquivo **config** para adicionar a chave ao ssh-agent
  - IdentityFile ~/.ssh/chave-ssh
- Adicionar a chave .ssh às chaves SSH do usuário no Github
- Inserir as variáveis secretas do projeto      

No projeto desejado, definir como Secrets as seguintes variáveis:

**SSH_PRIVATE_KEY**: chave privada do .ssh 

**SSH_PUBLIC_KEY**: chave publica '.pub' do .ssh

**SSH_HOST**: host do servidor. ex:dominio.com

**SSH_USER**: usuário do servidor

**WORK_DIR**: path do diretório a ser feito o pull.

**SSH_BRANCH**: branch para ser feita o pull.

