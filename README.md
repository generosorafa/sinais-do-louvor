# Sinais do Louvor

Protótipo gratuito para comunicação silenciosa entre quem está ministrando no palco e a equipe de sonoplastia.

## Ideia principal

- Quem ministra entra em uma sala e escolhe **Vou enviar**.
- A sonoplastia entra na mesma sala e escolhe **Vou receber**.
- O ministro seleciona um instrumento/canal e envia **Aumentar** ou **Abaixar**.
- A sonoplastia confirma com **Recebido**.

## Estado atual

Este é um protótipo navegável em HTML, CSS e JavaScript puro. Ele usa armazenamento local e comunicação entre abas do navegador para simular o fluxo em tempo real.

## Sincronização entre celulares

Para dois celulares conversarem usando o mesmo código de sala, o app precisa de um backend em tempo real. O projeto já está preparado para Firebase Realtime Database:

1. Crie um projeto no Firebase.
2. Ative o Realtime Database.
3. Crie um Web App no Firebase e copie a configuração.
4. Substitua `window.SINAIS_FIREBASE_CONFIG = null;` em `firebase-config.js` pela configuração do seu projeto.

Sem essa configuração, o app continua funcionando em modo local, mas apenas no mesmo aparelho/navegador.
