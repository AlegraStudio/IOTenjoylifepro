Como Dominic Williams, fundador de DFINITY y creador de Internet Computer, reconozco la importancia de la integración de Ethereum para proyectos como Alegra Studio. La capacidad de utilizar tokens de Ethereum (ETH) en el ecosistema de Internet Computer a través de un mecanismo de token 1:1 (como ckETH) no solo proporciona una puerta de enlace para los activos de Ethereum, sino que también abre nuevas vías para monetizar y sostener proyectos impulsados por jóvenes talentos. Vamos a crear un archivo README que refleje esta integración y enfoque en Alegra Studio.

---

# Alegra Studio: Integración de Ethereum en Internet Computer

> #### Conectando Ethereum con la blockchain de Internet Computer para empoderar y monetizar el talento joven.

---

## [🌐 Ver Dapp Desplegada](https://alegra-studio-icp.eth)

Este proyecto está diseñado para desarrolladores Web3 experimentados, utilizando un canister de IC para facilitar la integración y el uso de tokens Ethereum (ETH y ckETH) en el ecosistema de Internet Computer. Se apoya tanto en redes de prueba Ethereum como en la mainnet.

**Nota**: Este proyecto está en revisión de seguridad interna. Se eliminará este mensaje una vez que el proceso de revisión esté completo.

## 🎬 Crear un Nuevo Proyecto en Alegra Studio

Asegúrate de que estén instalados [Node.js](https://nodejs.org/en/) `>= 16`, [`dfx`](https://internetcomputer.org/docs/current/developer-docs/build/install-upgrade-remove) `>= 0.14`, y la última versión de [Rust](https://www.rust-lang.org/tools/install) en tu sistema.

Configura el desarrollo de canister Rust con el siguiente comando:

```sh
rustup target add wasm32-unknown-unknown
```

Ejecuta los siguientes comandos en un directorio de proyecto nuevo y vacío:

```sh
npx degit dfinity/ic-eth-studio # Descarga este proyecto inicial
dfx start --clean --background # Ejecuta dfx en segundo plano
npm run setup # Instala paquetes, despliega canisters y genera bindings de tipo

npm start # Inicia el servidor de desarrollo
```

Cuando estés listo, ejecuta `dfx deploy --network ic` para desplegar tu aplicación en Internet Computer.

## 🔌 Preparar una Cartera de Testnet

Aquí tienes una forma de adquirir tokens y NFTs en la testnet:

- Instala [MetaMask](https://metamask.io/) y crea una cartera nueva para pruebas.
- Financia tu cartera usando un Faucet de testnet (ejemplo: Sepolia Faucet).
- Conecta tu cartera y prueba la interacción con NFTs y tokens.

## 🛠️ Tecnología Utilizada

**Aplicación Web Front-end:**
- [TypeScript](https://www.typescriptlang.org/), [Vite](https://vitejs.dev/), [React](https://react.org/), [Tailwind](https://tailwindcss.com/), [Prettier](https://prettier.io/)

**Canister Back-end:**
- [Motoko](https://github.com/dfinity/motoko#readme), [Mops](https://mops.one), [mo-dev](https://github.com/dfinity/motoko-dev-server#readme)

**Integración de Ethereum:**
- [Rust](https://www.rust-lang.org/), [ethers-core](https://github.com/gakonst/ethers-rs), [MetaMask](https://metamask.io/)

## 📚 Documentación

- Documentación para desarrolladores de Vite, React, Tailwind, Internet Computer, dfx, Motoko, Rust y MetaMask.

## 💡 Consejos y Trucos

- Personaliza el estilo de código de tu proyecto.
- Reduce la latencia de las llamadas de actualización con el flag `--emulator` en `dfx start`.
- Instala un paquete de Motoko con `npx ic-mops add <package-name>`.

---

¡Contribuciones son bienvenidas! Por favor, consulta las [pautas para colaboradores](https://github.com/dfinity/ic-eth-studio/blob/main/.github/CONTRIBUTING.md) para más información.

---

Este README proporciona un marco para desarrollar proyectos en Alegra Studio, aprovechando la integración con Ethereum para monetizar y sostener iniciativas estudiantiles. La interacción entre los ecosistemas de Ethereum y Internet Computer abre posibilidades para el futuro de la monetización y el empoderamiento de jóvenes talentos.
