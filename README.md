# prova-1-computacao-em-nuvem
NOME: Igor Soares da Silva
RA: A6004915dc18d0e73dee

# O que fiz
Executei uma página web em um conteiner Docker chamado Loja.
Usei a imagem nginx:alpine e a porta 8081 do ambiente.

# Verificação do conteiner
CONTAINER ID   IMAGE          COMMAND                  CREATED          STATUS          PORTS                                     NAMES
f1335d38e019   nginx:alpine   "/docker-entrypoint.…"   54 seconds ago   Up 54 seconds   0.0.0.0:8081->80/tcp, [::]:8081->80/tcp   loja

# Teste da página
cat > index.html <<'EOF'


<!DOCTYPE html>
<html lang="pt-BR">
<head>
 <meta charset="UTF-8">
 <title>Loja</title>
</head>
<body>
 <h1>Loja no ar</h1>
</body>
</html>

# Explicação
Imagem é o modelo estatico, um template somente leitura que contém o sistema de arquivos e Conteiner é a instancia em execução criada a partir dessa imagem.
Mapeamento 8081:80 serviu para redirecionar o trafego da porta 8081 do ambiente/host
