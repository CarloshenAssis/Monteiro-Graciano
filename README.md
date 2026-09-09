# Monteiro & Graciano — Site Institucional

Site institucional estático (HTML/CSS/JS puro) da Monteiro & Graciano Contabilidade Empresarial, com todo o conteúdo baseado no material recuperado do site antigo e as fotos/logo oficiais da empresa.

## Como visualizar localmente

Não há build nem dependências. Basta servir a pasta como arquivos estáticos, por exemplo:

```bash
python3 -m http.server 8080
```

E abrir `http://localhost:8080/index.html`.

## Estrutura

```
index.html            # homepage única, com todas as seções
assets/css/style.css  # estilos (paleta navy/azul/branco, tipografia serif + sans)
assets/js/main.js     # menu mobile, acordeões "Saiba mais", ano do rodapé
assets/img/           # logo oficial e fotos reais dos sócios
reference/            # imagem de referência visual (protótipo), não usada no site
```

## Imagens

| Arquivo | Uso |
|---|---|
| `assets/img/logo-mg.png` | Logo oficial — header e rodapé (sobre uma "plate" branca no rodapé) |
| `assets/img/foto-socio.png` | Foto do sócio-proprietário — seção Hero |
| `assets/img/foto-socia.png` | Foto da sócia-proprietária — seção Sobre |
| `assets/img/foto-socios.png` | Foto dos dois sócios — inset da seção Sobre |
