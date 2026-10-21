# app-frontend-client

Aplicación frontend construida con **React** y **Vite**. Proyecto personal para retomar y reforzar el desarrollo web moderno.

## 🚀 Tecnologías

- [React](https://react.dev/) — librería de UI
- [Vite](https://vite.dev/) — bundler y servidor de desarrollo
- JavaScript (ES2022+)
- ESLint — calidad de código

## 📋 Requisitos previos

- Node.js 20 o superior
- npm 10 o superior
- Git

Verifica tus versiones:

```bash
node -v
npm -v
git -v
```

## ⚙️ Instalación

```bash
# 1. Clonar el repositorio
git clone https://github.com/IrvinNova/app-frontend-client.git

# 2. Entrar a la carpeta
cd app-frontend-client

# 3. Instalar dependencias
npm install

# 4. Crear tu archivo de variables de entorno
cp .env.example .env

# 5. Levantar el servidor de desarrollo
npm run dev
```

La app estará disponible en `http://localhost:5173`.

## 📜 Scripts disponibles

| Comando           | Descripción                                    |
| ----------------- | ---------------------------------------------- |
| `npm run dev`     | Inicia el servidor de desarrollo               |
| `npm run build`   | Genera la versión de producción en `dist/`     |
| `npm run preview` | Previsualiza localmente el build de producción |
| `npm run lint`    | Revisa el código con ESLint                    |

## 📁 Estructura del proyecto

```
app-frontend-client/
├── public/            # Archivos estáticos públicos
├── src/
│   ├── assets/        # Imágenes, fuentes, íconos
│   ├── components/    # Componentes reutilizables (Button, Card...)
│   ├── pages/         # Vistas completas (Home, Login...)
│   ├── hooks/         # Custom hooks
│   ├── services/      # Llamadas a APIs (fetch / axios)
│   ├── utils/         # Funciones auxiliares
│   ├── App.jsx        # Componente raíz
│   └── main.jsx       # Punto de entrada
├── .env.example       # Plantilla de variables de entorno
├── .gitignore
├── index.html
├── package.json
└── vite.config.js
```

## 🔐 Variables de entorno

Las variables deben empezar con `VITE_` para que Vite las exponga al cliente.

```env
VITE_API_URL=http://localhost:3000/api
```

> ⚠️ Nunca subas tu archivo `.env` al repositorio. Usa `.env.example` como plantilla.

## 🌿 Flujo de trabajo con Git

**Ramas**

- `main` — código estable
- `feature/nombre` — nuevas funcionalidades
- `fix/nombre` — corrección de errores

**Convención de commits** ([Conventional Commits](https://www.conventionalcommits.org/es/))

| Prefijo     | Uso                                        |
| ----------- | ------------------------------------------ |
| `feat:`     | Nueva funcionalidad                        |
| `fix:`      | Corrección de un error                     |
| `chore:`    | Configuración, dependencias, mantenimiento |
| `refactor:` | Cambio de código sin alterar funcionalidad |
| `style:`    | Formato, espacios (sin cambios lógicos)    |
| `docs:`     | Documentación                              |

Ejemplo:

```bash
git checkout -b feature/login-page
git commit -m "feat: agregar formulario de inicio de sesión"
git push origin feature/login-page
```

Después abre un Pull Request hacia `main`.

## 🗺️ Roadmap

- [x] Configuración inicial con React + Vite
- [ ] Navegación con React Router
- [ ] Estilos con Tailwind CSS
- [ ] Consumo de API
- [ ] Autenticación
- [ ] Deploy (Vercel / Netlify)

## 👥 Autores

- **Irvin Nova** — [@IrvinNova](https://github.com/IrvinNova)
- **Jhonatan Domínguez** — [@jhonatan810](https://github.com/jhonatan810)
- **Cristian González** — [@cristiangonzalezh](https://github.com/cristiangonzalezh)
