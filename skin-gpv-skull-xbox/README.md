# SKULL Xbox — preto e branco

Skin para o Gamepad Viewer, com geometria de 750 × 630 px. Corpo preto, ornamentos Oni em escala de cinza e lettering SKULL branco ao fundo, abaixo dos comandos. Os estados de ativação usam iluminação branca.

## Prévia local

Abra `preview.html` no navegador. O botão permite simular os comandos iluminados; a prévia não lê um controle conectado.

## Uso

Hospede `stylesheet.css` e `assets` juntos, preservando os caminhos relativos. Configure a URL pública do CSS como skin personalizada no Gamepad Viewer.

Use uma fonte de navegador de **750 × 630 px** ou maior. Inclua `smeter=1` para os gatilhos analógicos e `nocurve=1` para impedir inclinação 3D dos analógicos.

O botão central usa um emblema Xbox com caveira em preto e branco. Os analógicos mantêm a arte ornamental original em escala de cinza pelo CSS. O novo `assets/wordmark-skull-brush.png` é integrado ao corpo com `mix-blend-mode: screen`. Os arquivos antigos foram preservados, mas o lettering CYPHERS não é usado pela skin atual.
