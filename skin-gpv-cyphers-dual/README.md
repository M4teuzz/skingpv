# Cyphers Dual

Variante do overlay Cyphers inspirada em um painel de controle: dois pedais com silhueta arredondada/trapezoidal e acabamento Oni preto/vermelho, além de dois analogicos minimalistas com o nome CYPHERS, alinhados horizontalmente.

## Controles exibidos

- Analogico esquerdo: `stick-1`.
- Analogico direito: `stick-2`.
- Pedal esquerdo: LT.
- Pedal direito: RT.

Os dois analogicos usam o mesmo asset Oni, mas cada elemento recebe independentemente os eixos correspondentes do Gamepad Viewer.

## Uso

Hospede esta pasta preservando a subpasta `assets` e informe a URL publica de `stylesheet.css` no parametro `css` do Gamepad Viewer.

Tamanho recomendado para a fonte de navegador no OBS: **500 x 210 px** ou maior.

Use `nocurve=1` na URL. O CSS tambem força `transform: none` nos sticks para impedir a inclinacao 3D, mantendo o deslocamento horizontal e vertical aplicado por margem.

## Personalizacao

As medidas e URLs dos assets ficam nas variaveis do bloco `:root` no inicio de `stylesheet.css`.

Os assets atuais sao `analogico-cyphers-minimal.png` e `pedal-oni-curvo.png`. O mesmo pedal e espelhado pelo CSS no lado esquerdo, corrigindo a orientacao. Os assets anteriores foram preservados na pasta para permitir retorno a outras aparencias.
