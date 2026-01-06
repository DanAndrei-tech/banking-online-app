🏦 Banking Online App

Aplicación web de banca online desarrollada con React + TypeScript, que permite gestionar cuentas bancarias, consultar movimientos y realizar transferencias.
El backend está simulado mediante json-server, ideal para demostración y portfolio.

🚀 Demo online

Frontend (Vercel):
👉 https://banking-online-app.vercel.app

Backend / API (Railway):
👉 https://banking-online-app-production-6ca7.up.railway.app/api

🔐 Credenciales de acceso

Para acceder a la aplicación utiliza las siguientes credenciales:

Usuario: admin@email.com
Contraseña: test

🧩 Funcionalidades

✅ Login de usuario

✅ Listado de cuentas bancarias

✅ Consulta de movimientos por cuenta

✅ Transferencias bancarias

✅ Alta de nuevas cuentas

✅ Validaciones de formularios

✅ Navegación SPA (React Router)

✅ Separación clara Frontend / Backend

✅ Arquitectura basada en ViewModels y Mappers

🛠️ Tecnologías utilizadas
Frontend

React 18

TypeScript

Vite

React Router

Axios

CSS Modules

Backend (mock)

Node.js

json-server

Faker.js (generación de IBAN)

Middlewares personalizados

Deploy

Frontend: Vercel

Backend: Railway

🗂️ Estructura del proyecto
banking-online-app/
├── front-end/ # Aplicación React (Vite)
│ ├── src/
│ ├── public/
│ ├── vercel.json
│ └── package.json
│
├── back-end/ # API simulada (json-server)
│ ├── server/
│ │ ├── data.json
│ │ ├── login.middleware.js
│ │ ├── account.middleware.js
│ │ └── package.json
│ └── config/
│ └── routes.json

▶️ Ejecutar el proyecto en local
1️⃣ Clonar el repositorio
git clone https://github.com/tu-usuario/banking-online-app.git
cd banking-online-app

2️⃣ Backend (API mock)
cd back-end/server
npm install
npm start

La API se levantará en:

http://localhost:3000/api

3️⃣ Frontend
cd front-end
npm install
npm run dev

La aplicación estará disponible en:

http://localhost:5173

🔄 Variables de entorno
Frontend (front-end/.env)
VITE_BASE_API_URL=http://localhost:3000/api

En producción, esta variable apunta al backend desplegado en Railway.

🧠 Notas técnicas

Se utiliza el patrón Mapper para desacoplar los modelos del backend de los ViewModels del frontend.

El backend genera automáticamente:

IBAN

Balance inicial

Fecha de última transacción

El proyecto está pensado como SPA, con configuración específica para Vercel (vercel.json).
