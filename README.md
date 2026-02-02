🧮 Calculadora Operativa
Sistema de optimización con backend en FastAPI y frontend en Next.js, diseñado para resolver problemas de investigación operativa y potenciar las respuestas mediante modelos de lenguaje (Groq / Google Gemini).

📋 Requisitos Previos
Python 3.13+

Node.js 18+

Git

🛠️ Instalación y Configuración
1. Clonar el repositorio
git clone https://github.com/Jettro12/InvestigacionO.git cd InvestigacionO

2. Configuración del Backend (FastAPI)
Desde la raíz del proyecto, ejecuta los siguientes comandos:

Crear y activar el entorno virtual: python -m venv .venv ..venv\Scripts\Activate.ps1

Instalar dependencias: pip install -r requirements.txt

Configurar variables de entorno: Crea un archivo llamado .env en la raíz del proyecto y añade tus credenciales: GROQ_API_KEY=tu_api_key_de_groq_aqui GOOGLE_API_KEY=tu_api_key_de_gemini_aqui

Ejecutar el servidor: cd app python -m uvicorn main:app --host 127.0.0.1 --port 8000 --reload

El backend estará disponible en: http://127.0.0.1:8000

3. Configuración del Frontend (Next.js)
Abre una nueva terminal y navega a la carpeta del frontend:

Instalar dependencias: cd frontend/frontend npm install

Ejecutar en modo desarrollo: npm run dev

El frontend estará disponible en: http://localhost:3000

📂 Notas Importantes
Variables de Entorno: El archivo .env contiene información sensible y no debe subirse a GitHub. Asegúrate de que esté incluido en tu .gitignore.

Carpeta Static: Git no rastrea carpetas vacías. Se recomienda crear un archivo .gitkeep dentro de app/static/ para mantener la estructura de carpetas necesaria para FastAPI.

Puertos: Si modificas el puerto del backend (8000), recuerda actualizar la URL de la API en las llamadas del frontend.