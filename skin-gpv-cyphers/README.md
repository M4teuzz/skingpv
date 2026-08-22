# Cyphers Oni — skin para Gamepad Viewer

Overlay de direcao para transmissao e gravacao. O analogico esquerdo controla o volante; LT e RT representam os dois pedais.

## Link pronto do Gamepad Viewer

Esta versao esta publicada de forma isolada na pasta `skin-gpv-cyphers` do repositorio publico `M4teuzz/skingpv`. Use:

```text
https://gamepadviewer.com/?p=1&s=1&smetter=1&nocurve=0&css=https%3A%2F%2Fcdn.jsdelivr.net%2Fgh%2FM4teuzz%2Fskingpv%40main%2Fskin-gpv-cyphers%2Fstylesheet.css
```

Esse endereco usa uma pasta diferente do CSS antigo na raiz, portanto nao altera nem conflita com a skin anterior.

## Arquivos

- `stylesheet.css`: skin carregada pelo Gamepad Viewer.
- `assets/`: imagens otimizadas do volante e dos pedais.
- `docs/`: capturas antigas usadas como referencia visual.
- Os PNGs antigos na raiz foram preservados para permitir comparacao ou retorno ao tema anterior.

## Instalacao

1. Hospede a pasta `skin-gpv` em um endereco acessivel pelo navegador.
2. Abra o Gamepad Viewer e selecione um layout customizado.
3. Informe a URL publica de `stylesheet.css` como CSS personalizado.
4. No OBS, adicione o viewer como Fonte de navegador com fundo transparente.
5. Use uma fonte de pelo menos **450 x 300 px** para acomodar o overlay sem corte.

O primeiro controle conectado nao precisa ser obrigatoriamente `gamepad-0`: a skin exibe qualquer `.controller.custom` conectado. Se houver mais de um, os overlays ocuparao a mesma posicao.

## Personalizacao

As medidas principais ficam no bloco `:root` no inicio de `stylesheet.css`:

- `--overlay-scale`: escala geral.
- `--wheel-left` e `--wheel-top`: posicao inicial do volante.
- `--pedal-side-gap` e `--pedal-top`: posicao dos pedais.
- `--wheel-image`, `--left-pedal-image` e `--right-pedal-image`: assets ativos.

Depois de substituir uma imagem, altere o valor `?v=1` da URL correspondente para evitar cache antigo no navegador ou OBS.

## Comportamento dos gatilhos

Os pedais iniciam com `opacity: 0`. O Gamepad Viewer deve atualizar a opacidade inline conforme o valor analogico de LT/RT. As regras `data-value` existentes tratam os formatos de zero conhecidos, mas nao tentam converter arbitrariamente texto de atributo em opacidade, pois CSS puro nao faz essa conversao de forma portavel.

## Resolucao dos assets

- Volante ativo (`volante-cyphers.png`): 512 x 512 px.
- Pedais: 256 x 320 px cada.

Essas resolucoes oferecem nitidez acima do tamanho exibido sem manter os arquivos-fonte excessivamente grandes.
