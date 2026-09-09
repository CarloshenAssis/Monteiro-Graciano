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
index.html                          # homepage, com as seções resumidas
servicos/index.html                 # hub com os 6 serviços completos
servicos/<slug>/index.html          # página individual de cada serviço
assets/css/style.css                # estilos (paleta navy/azul/branco, tipografia serif + sans)
assets/js/main.js                   # menu mobile, ano do rodapé
assets/img/                         # logo oficial e fotos reais dos sócios
reference/                          # imagem de referência visual (protótipo), não usada no site
```

Os 6 serviços têm página própria em `/servicos/<slug>/`:
`assessoria-fiscal`, `abertura-de-empresas`, `assessoria-contabil`,
`departamento-pessoal`, `e-social`, `planejamento-tributario`. Na home,
os cards de serviço mostram só um resumo e o botão "Saiba mais" leva à
página completa correspondente.

## Imagens

| Arquivo | Uso |
|---|---|
| `assets/img/logo-mg.png` | Logo oficial — header e rodapé (sobre uma "plate" branca no rodapé) |
| `assets/img/foto-socio.png` | Foto do sócio-proprietário — seção Hero |
| `assets/img/foto-socia.png` | Foto da sócia-proprietária — seção Sobre |
| `assets/img/foto-socios.png` | Foto dos dois sócios — inset da seção Sobre |
