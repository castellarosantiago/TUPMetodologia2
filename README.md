# Sistema Integral de Gestión de Negocios

##  Idea del Proyecto
El proyecto busca desarrollar una plataforma web que permita **agilizar el control de productos, categorías, stock y ventas** dentro de una empresa, sin importar su tamaño o rubro.  
La propuesta se centra en un **diseño simple e intuitivo**, adaptable a diferentes contextos, y que requiera una **mínima capacitación del personal**.

##  Alcance del Proyecto
El sistema contemplará las siguientes funcionalidades principales:

- **Tipos de usuarios**  
  - Administrador  
  - Empleado  

- **Autenticación y roles**  
  - Registro, login, logout  
  - Permisos según rol  

- **Gestión de productos, categorías y ventas**  
  - Operaciones CRUD  
  - Búsquedas con filtros  

- **Reportes**  
  - Generación y envío de comprobantes  
  - Exportación a PDF  
  - Visualización de gráficos  

- **Dashboard**  
  - Vista general con estadísticas relevantes  

> Todas las funcionalidades serán opcionales y configurables según las necesidades del negocio.  
> Ejemplo: un kiosco puede usar únicamente el rol "Administrador" o excluir el manejo de comprobantes si ya utiliza un sistema externo.

##  Tecnologías a Utilizar
- **Frontend**: React + Tailwind CSS  
- **Backend API**: Node.js + Express + Mongoose  
- **Base de Datos**: MongoDB  
- **Despliegue**: Render  
- **Repositorio**: GitHub  

##  Posibles Patrones de Diseño
Para el desarrollo, se evaluará la aplicación de los siguientes patrones:

- **MVC (Model-View-Controller)**  
  Separar la lógica de negocio, la interfaz de usuario y el control de flujo.  
  Útil para mantener un sistema escalable y organizado.

- **Repository Pattern**  
  Abstraer la lógica de acceso a datos en la interacción con MongoDB, permitiendo mayor flexibilidad y mantenibilidad.

- **Factory Method** (opcional)  
  Para la creación de objetos relacionados con usuarios, productos o reportes, facilitando la extensibilidad.

- **Singleton**  
  Aplicable en casos como la conexión a la base de datos para garantizar que exista una única instancia.

##  Integrantes del Proyecto
- Santiago Castellaro  
- Paula General  
- Mateo Muscolino  
