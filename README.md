# 🦸‍♂️ Marvel Bot (Node.js + Azure)

Un bot inteligente creado con **Node.js**, **Microsoft Bot Framework** y **Azure**, que permite consultar información de superhéroes del universo **Marvel** usando la **API oficial de Marvel**.

---

## 🚀 Características

- Consulta información de personajes de Marvel (Iron Man, Spider-Man, etc.)  
- Desarrollado con **Bot Framework SDK para Node.js**  
- Conectado a la **API oficial de Marvel**  
- Desplegado en **Microsoft Azure**  
- Interfaz de chat embebida en web mediante **Bot Framework Web Chat**

---

## 🧩 Estructura del Proyecto

marvel-bot/
│
├── .env
├── .gitignore
├── package.json
├── index.js
│
├── bot/
│ ├── marvelBot.js
│ └── dialogs/
│ └── mainDialog.js
│
└── services/
└── marvelService.js


---

## ⚙️ Instalación y Configuración

### 1️⃣ Clonar el repositorio

git clone https://github.com/tuusuario/marvel-bot.git
cd marvel-bot
2️⃣ Instalar dependencias


npm install
3️⃣ Crear archivo .env
Crea un archivo .env en la raíz del proyecto con el siguiente contenido:

env
MicrosoftAppId=TU_APP_ID_DE_AZURE
MicrosoftAppPassword=TU_APP_PASSWORD
MarvelPublicKey=TU_CLAVE_PUBLICA_MARVEL
MarvelPrivateKey=TU_CLAVE_PRIVADA_MARVEL
PORT=3978
⚠️ Asegúrate de agregar .env al archivo .gitignore para no subir tus credenciales.

🧠 Uso local
1️⃣ Iniciar el bot

node index.js
2️⃣ Probar con Bot Framework Emulator
Descarga el emulador desde 👉 https://aka.ms/botframework-emulator

Conéctalo a:

http://localhost:3978/api/messages
🌐 Despliegue en Azure
Crea un recurso Azure Bot Channels Registration.

Crea un App Service (Node.js 18 o superior).

Sube tu proyecto con VS Code o GitHub Actions.

Configura el endpoint del bot:

https://tuapp.azurewebsites.net/api/messages
Copia el Direct Line Secret para usarlo en el iframe.

💬 Integración Web (iframe)
Agrega este código a tu sitio web para integrar el chat:


<iframe 
  src='https://webchat.botframework.com/embed/botAzureJuan-bot?s=***************************'
  style='min-width: 400px; width: 100%; min-height: 500px;'>
</iframe>
🔑 API de Marvel
Para usar la API, crea tu cuenta gratuita en 👉 https://developer.marvel.com

Obtendrás tus Public Key y Private Key, necesarias en el archivo .env.

🧰 Tecnologías usadas
Node.js

Bot Framework SDK

Microsoft Azure

Axios

Marvel Developer API

Restify

🧑‍💻 Autor
👨‍💻 Juan [Guerrero]
