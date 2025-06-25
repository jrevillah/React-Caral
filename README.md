# IDAT - Desarrollo de Interfaces 2
## Sistema de Reservas de Mesas — [Caral Sanguchería]

> **Instrucciones:** 

## 1. Prerequisitos
Para asegurar un correcto funcionamiento de la aplicación, es necesario tener instaladas las siguientes herramientas en tu sistema:

| Herramienta | Versión mínima |
|-------------|---------------|
| Node        | 18 LTS        |
| npm         | 10            |

## 2. Instalación
Sigue estos pasos para obtener una copia local del proyecto y configurar las dependencias:
1. Clona el repositorio: Abre tu terminal y ejecuta el siguiente comando para clonar el proyecto a tu máquina:
```bash
git clone https://github.com/jrevillah/React-Caral.git
```

2. Accede al directorio del proyecto: Navega hasta la carpeta del proyecto clonado:
```bash
cd React-Caral
```

3. Instala las dependencias: Una vez dentro del directorio, instala todas las dependencias necesarias con npm:
```bash
npm install
```

## 3. Ejecución en modo desarrollo
Para arrancar la aplicación en tu entorno local y comenzar a desarrollar, utiliza el siguiente comando:

```bash
npm run dev
```

Una vez que el servidor de desarrollo esté activo, podrás acceder a la aplicación en tu navegador a través de la URL por defecto: http://localhost:5173.

## 4. Estructura de carpetas (abreviada)
A continuación, se presenta una estructura simplificada de los directorios y archivos más relevantes del proyecto:

```
src/
├── assets/components/   # Componentes específicos de la página principal (OnePage).
│   ├── footer.jsx       # Componente del pie de página.
│   ├── Gallery.jsx      # Componente para la sección de galería de imágenes.
│   ├── Header.jsx       # Componente del encabezado de la página.
│   ├── Hero.jsx         # Componente de la sección principal o "Hero".
│   ├── MenuSection.jsx  # Componente para mostrar las secciones del menú.
│   ├── PromoCards.jsx   # Componente para tarjetas de promociones.
│   └── Reservas.jsx     # Componente para la sección de reservas dentro de la OnePage.
├── components/          # Componentes reutilizables generales de la aplicación (ej. autenticación).
│   ├── LoginPage.jsx    # Componente para la interfaz de inicio de sesión.
│   ├── RegisterPage.jsx # Componente para la interfaz de registro de nuevos usuarios.
│   └── UserRecoveryPage.jsx # Componente para la interfaz de recuperación de credenciales.
├── hooks/               # Lógica compartida y personalizada de React.
│   └── useReservas.js   # Hook personalizado para la gestión de reservas.
└── App.jsx              # Componente principal que define las rutas de la aplicación.   
```

## 5. Enrutamiento
La aplicación utiliza react-router-dom para gestionar la navegación entre las diferentes vistas. La configuración principal de las rutas se encuentra en App.jsx y se inicializa en main.jsx.

A continuación, se muestra la estructura de rutas definida en App.jsx:

```bash
<Routes>
  <Route path="/" element={<OnePage />} /> {/* Ruta principal para la página de inicio */}
  <Route path="/Login" element={<Login />} /> {/* Ruta para la página de inicio de sesión */}
  <Route path="/Register" element={<Register />} /> {/* Ruta para la página de registro */}
  <Route path="/UserRecovery" element={<UserRecovery />} /> {/* Ruta para la página de recuperación de usuario */}
</Routes>
```

## 6. Créditos
Este proyecto fue desarrollado por el siguiente equipo:

|          Integrante             |   Código   |    Rol   |
|---------------------------------|------------|----------|
| Jimenez Rojas, Jonathan José    | iv42035014 | Dev / PM |
| Revilla Huapaya, Javier Alberto | a1402516   | Dev / UI |
| Talledo Ceverino, Andy Steve    | sm44972333 | Dev / QA |