# Build com Argumentos

Criar imagem:   
```docker image build -t build-com-arg .```

Criar imagem com Argumentos:   
```docker image build --build-arg S3_BUCKET=myapp -t build-com-arg .```

Rodar imagem e imprimir a variável de ambiente:   
```docker container run build-com-arg bash -c 'echo $S3_BUCKET'```

Exibir mantenedor:   
```docker image inspect --format="{{index .Config.Labels \"maintainer\"}}" build-com-arg```
