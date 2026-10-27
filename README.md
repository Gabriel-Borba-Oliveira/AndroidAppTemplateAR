# AndroidAppTemplateAR — atividade de Realidade Aumentada

Projeto Android em Kotlin com SceneView/ARCore. Esta branch acrescenta dois modelos GLB, uma mecânica simples de pontuação e áudio.

## Alterações desta atividade

- `app/src/main/assets/coin.glb`: moeda 3D colecionável.
- `app/src/main/assets/heart.glb`: coração 3D colecionável.
- `app/src/main/assets/ambient.wav`: trilha ambiente em loop durante a tela de RA.
- `app/src/main/assets/collect.wav`: efeito sonoro ao coletar.
- Na tela de RA, o botão **Coletar (+1)** atualiza o contador de pontos e reproduz o efeito sonoro.
- A tela de seleção lista automaticamente todos os arquivos `.glb` em `assets`, então os dois novos modelos aparecem sem configuração adicional.

## Como testar

1. Abra o projeto no Android Studio e aguarde a sincronização do Gradle.
2. Execute em um celular Android compatível com ARCore e conceda a permissão de câmera.
3. Na aba de modelos, escolha **Coin** ou **Heart** e toque em **Exibir**.
4. Aponte para uma superfície, toque em **Posicionar objeto** e teste **Coletar (+1)**. Verifique a música ambiente e o efeito sonoro.

> A validação final em dispositivo físico precisa ser feita localmente. O ambiente em que este projeto foi preparado não conseguiu baixar a distribuição Gradle para compilar, portanto não foi possível confirmar a compilação nem gerar capturas reais de RA.
