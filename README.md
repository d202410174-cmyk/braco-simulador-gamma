# Braço hidráulico com garra de engrenagens · simulador interativo

Simulador 3D do braço hidráulico do grupo, acionado por seringas, com garra de dois dedos movida por engrenagens. Projeto e Desenvolvimento de Produtos (DEP/UFTM).

## O que dá para fazer

- **Arrastar o êmbolo** das quatro seringas mestras (giro, ombro, cotovelo e garra). Cada subsistema se move sozinho, dentro do curso da animação feita no Blender.
- **Pegar e levar a engrenagem** de aço do suporte A até o B, operando as seringas, ou deixar o braço fazer sozinho com o botão "Pegar e levar a peça". A garra não fecha além da peça.
- **Isolar subsistemas** (giro, ombro, cotovelo, garra), ver a hidráulica em raio-X (MDF transparente) e trocar de câmera.
- **Ver em realidade aumentada** pela página `ar.html` (Chrome no Android, Safari no iPhone).

O aperto por dedo (≈) é estimado por trabalho virtual, a partir do curso do êmbolo da garra e da variação da abertura entre os pegadores. Ele considera uma força de 30 N na mão, seringas mestra e escrava iguais e nenhum atrito. A carga que a garra segura usa um atrito estimado de 0,3.

## Arquivos

| Arquivo | Conteúdo |
|---|---|
| `index.html` | O simulador (three.js 0.169 carregado do jsDelivr) |
| `ar.html` | Página de realidade aumentada (model-viewer) |
| `BracoRA.glb` | Modelo 3D com a animação, em metros |
| `BracoRA.usdz` | Modelo para o Quick Look do iPhone |

## Personalizar

No começo do script de `index.html`, edite o objeto `CONFIG`: título, grupo, integrantes, força da mão e atrito.

## Créditos

- Modelo 3D e animação: grupo, no Blender.
- Estrutura inspirada no simulador do braço A-81 da disciplina.
- Renderização 3D: [three.js](https://threejs.org) (licença MIT). RA: [model-viewer](https://modelviewer.dev) (licença Apache 2.0).
