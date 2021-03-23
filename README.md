# Template LAMP Docker 
## Getting Started
1. Instale o Docker Engine em sua máquina
	1. Windows: (<https://docs.docker.com/docker-for-windows/install/>)
	2. Linux: (<https://docs.docker.com/engine/install/#server>)
	3. MacOS: (<https://docs.docker.com/docker-for-mac/install/>)
2. Caso utilize Linux, será necessário a instalação manual do Docker Compose (<https://docs.docker.com/compose/install/>)
3. Gere um novo repositório baseado no template (<https://github.com/estherpeixoto/lampdocker/generate>)
4. Faça o _clone_ do seu projeto para sua máquina:
```bash
git clone https://github.com/seu_usuario/seu_repositorio.git
```
5. Preencha o arquivo _.env.example_ com as variáveis de ambiente para o MySQL
6. Remova do nome do arquivo _.env.example_ o trecho _.example_
7. Execute o seguinte comando na raiz do projeto:
```bash
docker-compose up -d
```
8. Acesse (<http://localhost:8080>)
## Contribuição
1. Faça o _fork_ do projeto (<https://github.com/estherpeixoto/lampdocker/fork>)
2. Crie uma _branch_ para sua modificação (`git checkout -b feature/foo`)
3. Faça o _commit_ (`git commit -am 'feat: adicionar foo'`)
4. _Push_ (`git push origin feature/foo`)
5. Crie um novo _Pull Request_