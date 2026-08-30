# Cyphers Dual

Variante do overlay Cyphers com dois pedais e os dois analogicos do controle.

## Controles exibidos

- Analogico esquerdo: `stick-1`.
- Analogico direito: `stick-2`.
- Pedal esquerdo: LT.
- Pedal direito: RT.

Os dois analogicos usam o mesmo asset Oni, mas cada elemento recebe independentemente os eixos correspondentes do Gamepad Viewer.

## Uso

Hospede esta pasta preservando a subpasta `assets` e informe a URL publica de `stylesheet.css` no parametro `css` do Gamepad Viewer.

Tamanho recomendado para a fonte de navegador no OBS: **500 x 280 px** ou maior.

Use `nocurve=1` na URL. O CSS tambem força `transform: none` nos sticks para impedir a inclinacao 3D, mantendo o deslocamento horizontal e vertical aplicado por margem.

## Personalizacao

As medidas e URLs dos assets ficam nas variaveis do bloco `:root` no inicio de `stylesheet.css`.

O tema foi produzido em preto e vermelho a partir da referencia visual Cyphers/Oni. O asset do analogico foi gerado em alta resolucao e otimizado para 256 x 256 px com transparencia real.
