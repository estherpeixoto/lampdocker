# Template LAMP Docker

## Requisitos
1. Instale o Docker Engine em sua máquina
	1. Windows: <https://docs.docker.com/docker-for-windows/install/>
	2. Linux: <https://docs.docker.com/engine/install/#server>
	3. MacOS: <https://docs.docker.com/docker-for-mac/install/>
2. Caso utilize Linux, será necessário a instalação manual do Docker Compose <https://docs.docker.com/compose/install/>

## Getting Started
1. Faça o _clone_ do projeto para sua máquina:
```bash
git clone https://github.com/estherpeixoto/lampdocker.git
```
2. Preencha o arquivo _.env.example_ com as variáveis de ambiente para o MySQL
3. Remova do nome do arquivo _.env.example_ o trecho _.example_
4. Execute o seguinte comando na raiz do projeto:
```bash
docker-compose up -d
```
5. Acesse <http://example.com>

## Configurar novo virtual host
1. Crie seu projeto na pasta _/html_
2. Configure o virtual host no arquivo _/docker/apache-2.4.conf_
3. Adicione o IP do container + ServerName ao seu arquivo de hosts 
	1. Windows: _C:\Windows\System32\drivers\etc_
	2. Linux: _/etc/hosts_
	3. MacOS: _/private/etc/hosts_
5. Acesse seu site a partir do ServerName configurado

## Contribuição
1. Faça o _fork_ do projeto (<https://github.com/estherpeixoto/lampdocker/fork>)
2. Crie uma _branch_ para sua modificação (`git checkout -b feature/foo`)
3. Faça o _commit_ (`git commit -am 'feat: adicionar foo'`)
4. _Push_ (`git push origin feature/foo`)
5. Crie um novo _Pull Request_
