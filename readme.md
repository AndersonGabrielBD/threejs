# 🌐 Cena 3D Interativa com Three.js

Projeto web de cena 3D interativa utilizando **Three.js**, com carregamento de modelo 3D via `GLTFLoader` e controle de câmera por `OrbitControls`.

---

## 📦 Modelo 3D Utilizado

| Campo        | Informação |
|--------------|------------|
| **Nome**     | Damaged Helmet |
| **Autor**    | Khronos Group / glTF-Sample-Assets |
| **Formato**  | GLB (glTF Binary) |
| **Licença**  | [CC Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/) |
| **Link de origem** | [https://sketchfab.com/3d-models/battle-damaged-sci-fi-helmet-pbr-b81008d513954189a063ff901f7abfe4](https://sketchfab.com/3d-models/battle-damaged-sci-fi-helmet-pbr-b81008d513954189a063ff901f7abfe4) |

> O modelo também está disponível no repositório oficial do Khronos Group:
> [`glTF-Sample-Assets/Models/DamagedHelmet`](https://github.com/KhronosGroup/glTF-Sample-Assets/tree/main/Models/DamagedHelmet)

---

## 🚀 Como Executar

Basta abrir o arquivo `index.html` diretamente no navegador — não é necessário instalar nada.

> **Requisito:** conexão com a internet (Three.js e o modelo são carregados via CDN/URL externa).

```bash
# Opção 1 — abrir diretamente
Clique duas vezes em index.html

# Opção 2 — servidor local com Python (recomendado para modelos locais)
python -m http.server 8080
# Acesse: http://localhost:8080

# Opção 3 — servidor local com Node.js
npx serve .
# Acesse: http://localhost:3000
```

---

## 🎮 Controles de Câmera (OrbitControls)

| Ação | Mouse | Touch |
|------|-------|-------|
| **Rotacionar** | Clique esquerdo + arrastar | 1 dedo |
| **Zoom** | Scroll do mouse | Pinça com 2 dedos |
| **Pan (deslocar)** | Clique direito + arrastar | 2 dedos |

---

## 💡 Recursos Implementados

- ✅ **GLTFLoader** — carregamento de modelo `.glb` sem erros no console
- ✅ **OrbitControls** — rotação, zoom e pan com mouse e touch
- ✅ **Iluminação** — luz ambiente (`AmbientLight`) + luz direcional (`DirectionalLight`) + fill light
- ✅ **Loop de animação** — `requestAnimationFrame` com suporte a `AnimationMixer`
- ✅ **Resize handler** — câmera e renderer se adaptam ao redimensionamento da janela
- ✅ **Overlay de carregamento** — feedback visual com progresso percentual
- ✅ **Seletor de modelos** — troca entre 4 modelos glTF de exemplo em tempo real
- ✅ **Sombras** — `PCFSoftShadowMap` no renderer e nos meshes

---

## 🗂 Estrutura do Projeto

```
projeto-threejs/
├── index.html   # Aplicação completa (HTML + CSS + JS em um arquivo)
└── README.md    # Este arquivo
```

---

## 🛠 Tecnologias

- [Three.js r168](https://threejs.org/) — via CDN (importmap ES Module)
- `GLTFLoader` — carregamento de modelos glTF/GLB
- `OrbitControls` — controle de câmera interativo
- `RGBELoader` — suporte a iluminação HDR (disponível no código)

---

## 📄 Licença

Este projeto é de uso acadêmico. Os modelos 3D utilizados estão licenciados sob [Creative Commons Attribution 4.0](https://creativecommons.org/licenses/by/4.0/).