# Monteiro & Graciano — Site Institucional

Site institucional estático (HTML/CSS/JS puro) da Monteiro & Graciano Contabilidade Empresarial, com todo o conteúdo baseado no material recuperado do site antigo.

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
assets/img/           # logo e fotos
```

## ⚠️ Imagens pendentes de substituição

Os arquivos de imagem enviados na conversa (logo oficial, foto do sócio, foto da sócia e foto dos dois juntos) não chegaram como arquivos neste ambiente — apenas o `.docx` com o conteúdo foi salvo como arquivo real. Por isso o site está usando placeholders elegantes (SVG) nos mesmos nomes de arquivo, prontos para serem substituídos:

| Arquivo a substituir | Onde é usado |
|---|---|
| `assets/img/logo-mg.svg` | Logo no header (fundo claro) |
| `assets/img/logo-mg-light.svg` | Logo no rodapé (fundo azul-marinho) |
| `assets/img/foto-socio.svg` | Foto de destaque no Hero |
| `assets/img/foto-socia.svg` | Foto principal da seção Sobre |
| `assets/img/foto-socios.svg` | Foto dos dois sócios (inset na seção Sobre) |

Basta enviar os arquivos reais (`.png`/`.jpg` ou a logo vetorial oficial) com esses mesmos nomes — ou trocar o nome no `src` correspondente em `index.html` — que o layout se ajusta automaticamente, pois as imagens usam `object-fit: cover` dentro de proporções fixas.
