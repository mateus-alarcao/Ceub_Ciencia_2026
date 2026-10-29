# Aplicação simples: Minhas Tarefas

Aplicação web simples para adicionar, concluir e remover tarefas. Não precisa de Git, banco de dados ou instalação de linguagem.

## Como executar

1. Extraia o arquivo ZIP.
2. Abra o PowerShell na pasta `app-tarefas-docker`, onde está o Dockerfile.
3. Execute:

```powershell
docker build -t app-tarefas .
docker run -d --name app-tarefas -p 8080:80 app-tarefas
```

4. Abra http://localhost:8080 no navegador.

## Comandos úteis

Ver o container:
```powershell
docker ps
```

Parar:
```powershell
docker stop app-tarefas
```

Iniciar novamente:
```powershell
docker start app-tarefas
```

Remover o container:
```powershell
docker rm -f app-tarefas
```

As tarefas ficam apenas na página aberta; ao atualizar o navegador, a lista é reiniciada.
