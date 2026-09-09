# ping-tool e Servidor Web Nginx

Projeto de Docker e Git, feito com sucesso por Cindyane!

## Fase 1: Network Diagnostics Tool
Imagem Docker baseada em Ubuntu com utilitário ping.

### Build
docker build -t ping-tool:1.0 .

### Uso
docker run -it --rm ping-tool:1.0 

## Fase 2: Servidor Web Nginx com Bind Mount

### Execução
docker run -d --name meu-web-server -p 8080:80 -v $(pwd)/html:/usr/share/nginx/html nginx:latest

### Acesso
Acesse http://localhost:8080 no seu navegador.
