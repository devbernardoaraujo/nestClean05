Antes de começar, você precisará ter as seguintes ferramentas na sua máquina: Docker, pnpm, Node.js

Primeiramente, realize a configuração do Docker, no terminal, use o comando:

"docker-compose up -d"


### Instalação de dependencias 

Com o Node.js instalado, use o comando 'npm' para instalar o 'pnpm', um gerenciador de pacotes rápido e eficiente: 

"npm install -g pnpm"

Em seguida, instale dependencias do projeto com:

"pnpm install"

Com o  banco de dados rodando, e o '.env' configurado, aplique as migrations para estruturar o banco de dados:

"pnpm prisma generate"

"pnpm prisma migrate dev"


é necessário também ter o arquivo .env, caso queria as configurações, entre em contato comigo.

Finalmente, para iniciar o projeto execute:

"pnpm start" ou se estiver desenvolvendo e deseja que o servidor reinicie automaticamente ao modificar arquivos, use "pnpm run start:dev"



