# COMO ADICIONAR VÍDEOS E FOTOS DE FUNDO

## 📹 VÍDEOS DE FUNDO

Para adicionar vídeos de fundo nas seções:

1. **Coloque seus vídeos na pasta `videos/`**
2. **Use os nomes sugeridos:**
   - `about-bg.mp4` - Para seção Sobre
   - `services-bg.mp4` - Para seção Serviços  
   - `visit-bg.mp4` - Para seção Agendar Visita
   - `contact-bg.mp4` - Para seção Contato

3. **No HTML, descomente a linha do vídeo:**
   ```html
   <!-- Para adicionar vídeo de fundo: <video class="video-background" autoplay muted loop><source src="videos/about-bg.mp4" type="video/mp4"></video> -->
   ```
   Vire:
   ```html
   <video class="video-background" autoplay muted loop><source src="videos/about-bg.mp4" type="video/mp4"></video>
   ```

## 📸 FOTOS DE FUNDO

Para adicionar fotos de fundo nas seções:

1. **Coloque suas imagens na pasta `images/`**
2. **Use os nomes sugeridos:**
   - `about-bg.jpg` - Para seção Sobre
   - `services-bg.jpg` - Para seção Serviços
   - `visit-bg.jpg` - Para seção Agendar Visita
   - `contact-bg.jpg` - Para seção Contato

3. **No HTML, descomente a linha da imagem:**
   ```html
   <!-- Para adicionar imagem de fundo: <img class="image-background" src="images/about-bg.jpg" alt="Background"> -->
   ```
   Vire:
   ```html
   <img class="image-background" src="images/about-bg.jpg" alt="Background">
   ```

## 🎯 DICAS

- **Formatos recomendados:** MP4 para vídeos, JPG/PNG para imagens
- **Tamanho ideal:** 1920x1080 pixels para melhor qualidade
- **Duração vídeos:** 10-30 segundos em loop
- **Opacidade:** O fundo terá 90% de transparência automática
- **Performance:** Vídeos e imagens otimizadas para web carregam mais rápido

## 📁 ESTRUTURA DE PASTAS

```
personal-website/
├── images/
│   ├── logo-au-e.png
│   ├── about-bg.jpg
│   ├── services-bg.jpg
│   ├── visit-bg.jpg
│   └── contact-bg.jpg
├── videos/
│   ├── about-bg.mp4
│   ├── services-bg.mp4
│   ├── visit-bg.mp4
│   └── contact-bg.mp4
└── index.html
```
