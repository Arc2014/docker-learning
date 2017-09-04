# Build Dev

Criar Imagem:   
```docker image build -t build-dev .```

Rodar Imagem:
```docker container run -it -v $(pwd):/app -p 80:8000 --name pyton-server build-dev```
