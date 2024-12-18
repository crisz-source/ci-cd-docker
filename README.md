# Acessando do dockerhub atraves de um token

- vá no dockerhub e siga esses passos: **perfil > Account Settings > Personal access tokens > Generate new token**
- Adicione uma descrição ao token
- Adicione uma validação ao token
- Em permissão, adicione: **Read, Write, Delete** > generate
- copie o token e siga esses passos abaixo


# No GitHub Actions
- Vá no seu repositório e siga esses passos: settings > Secrets and variables (no menu lateral esquerdo) > Acitons 
- Adicione um nome para variavel que vai ser seu login no docker hub: **DOCKER_USERNAME** e em secret, coloque o seu **usuário** e depois clique em **Add secret**
- Agora adicione um nome para variavel que vai acessar o token no dockerhub: **DOCKERHUB_TOKENACCESS** e em secret, coloque o token gerado anteriormente e clique em **Add secret**
- Todas essas screts já estão sendo usadas no arquivo de workflow
