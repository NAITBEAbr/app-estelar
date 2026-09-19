# App Estelar

Aplicativo mobile sobre astronomia, com três telas: naves espaciais, mapa estelar e a
foto astronômica do dia.

## Funcionalidades

- **Naves espaciais**: lista naves e agências espaciais, com foto, nome e descrição,
  buscadas da API pública The Space Devs
- **Mapa estelar**: mostra o céu ao vivo da sua posição, com constelações, nomes das
  estrelas e linhas de grade, usando o Virtual Sky dentro de uma WebView
- **Foto do dia**: exibe a imagem astronômica do dia da NASA (APOD), com título e
  explicação

## Tecnologias

- React Native com Expo
- React Navigation (navegação em pilha e por abas)
- axios, para consumir as APIs
- react-native-webview, para o mapa estelar

## APIs usadas

| API | Para quê |
|---|---|
| NASA APOD | foto astronômica do dia |
| The Space Devs | catálogo de naves espaciais |
| Virtual Sky (LCO) | mapa do céu interativo |

## Como executar

```bash
npm install
npx expo start
```

Depois é só ler o QR Code com o Expo Go no celular.

Para usar sua própria chave da NASA, pegue uma gratuita em
[api.nasa.gov](https://api.nasa.gov) e substitua a chave em `screens/DailyPic.js`.
