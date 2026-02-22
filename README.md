# Portfolio Dashboard

Dashboard de análisis de cartera de inversión — GVC Gaesco.

## Deploy en Vercel

### Opción 1: CLI de Vercel
```bash
npm install -g vercel
vercel --prod
```

### Opción 2: GitHub + Vercel (recomendado)
1. Sube este repositorio a GitHub
2. Entra en [vercel.com](https://vercel.com) → New Project
3. Importa el repositorio de GitHub
4. Configuración:
   - **Framework Preset**: Other
   - **Output Directory**: `public`
   - **Build Command**: (dejar vacío)
5. Click **Deploy** ✓

### Estructura
```
portfolio-vercel/
├── public/
│   └── index.html    ← Dashboard completo (auto-contenido)
├── vercel.json       ← Configuración Vercel
├── package.json
└── README.md
```

### Desarrollo local
```bash
npm install
npm run dev
# Abre http://localhost:3000
```

### Notas
- El dashboard es un único archivo HTML estático, sin dependencias de servidor.
- Todas las librerías (Chart.js, Google Fonts) se cargan desde CDN.
- Compatible con Vercel, Netlify, GitHub Pages o cualquier hosting estático.
