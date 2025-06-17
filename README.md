# naturguide-backend
Backend en Node.js con Express y PostgreSQL para una app de localización de pozas, playas fluviales, acampadas y lugares naturales. Desplegado en Railway.

# 🌿 NaturGuide Backend

API REST construida en Node.js con Express, PostgreSQL y Prisma ORM para una app de exploración de zonas naturales como:

- 🏞️ Pozas naturales
- 🏕️ Zonas de acampada
- 🌊 Playas fluviales
- 🏊 Piscinas naturales

Desplegada en [Railway](https://railway.app), lista para ser consumida desde frontend web o app móvil.

---

## 🚀 Tecnologías usadas

- [Node.js](https://nodejs.org/)
- [Express](https://expressjs.com/)
- [PostgreSQL](https://www.postgresql.org/)
- [Prisma ORM](https://www.prisma.io/)
- [Railway](https://railway.app/) (para despliegue y DB)
- [dotenv](https://www.npmjs.com/package/dotenv)
- [CORS](https://www.npmjs.com/package/cors)

---

## 📦 Endpoints disponibles

| Método | Ruta             | Descripción                     |
|--------|------------------|---------------------------------|
| GET    | `/api/places`    | Obtener todos los lugares       |
| POST   | `/api/places`    | Crear un nuevo lugar            |

### 🧾 Ejemplo JSON para POST `/api/places`

```json
{
  "nombre": "Poza Secreta del Río Verde",
  "descripcion": "Lugar tranquilo con agua cristalina.",
  "tipo": "poza",
  "latitud": 37.3833,
  "longitud": -5.9714
}

⚙️ Variables de entorno
Crea un archivo .env en la raíz con:

env

DATABASE_URL="postgresql://usuario:contraseña@host:puerto/base"
Railway lo genera automáticamente si conectas el plugin PostgreSQL.

🛠️ Scripts útiles
bash

npm install        # Instala dependencias
npm start          # Inicia servidor Express
npx prisma studio  # Interfaz web para ver la DB

🗃️ Estructura del proyecto
pgsql

backend/
├── prisma/
│   └── schema.prisma
├── src/
│   ├── index.js
│   └── routes/
│       └── places.js
├── .env
├── package.json
└── README.md

🧠 Futuras mejoras
🔐 Autenticación de usuarios

🧭 Filtro por distancia desde ubicación

🧠 IA para categorizar descripciones

🌍 Multilenguaje (ES/EN)

📸 Subida de imágenes

🌐 Buscador inteligente

📄 Licencia
Este proyecto está bajo la MIT License.

🤝 Contribuciones
¿Tienes ideas, correcciones o lugares interesantes? ¡Bienvenido a colaborar!
Puedes abrir un PR o contactarnos.

---

¿Quieres que te lo suba directamente al repo (puedes pasarme la URL) o te lo dejo como archivo descargable? También puedo hacer la versión en inglés si vas a configurar multilenguaje en el frontend.
