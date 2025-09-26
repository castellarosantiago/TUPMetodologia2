# Sistema Integral de Gestión de Negocios

##  Idea del Proyecto
El proyecto busca desarrollar una plataforma web que permita agilizar el control de productos, categorías, stock y ventas dentro de una empresa, sin importar su tamaño o rubro.  
La propuesta se centra en un diseño simple e intuitivo, adaptable a diferentes contextos y que requiera una mínima capacitación del personal.

---

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

Todas las funcionalidades serán opcionales y configurables según las necesidades del negocio.  
Ejemplo: un kiosco puede usar únicamente el rol *Administrador* o excluir el manejo de comprobantes si ya utiliza un sistema externo.

---

## 👨 Integrantes
- Santiago Castellaro  
- Paula General  
- Mateo Muscolino  

---

##  Tecnologías a Utilizar
- **Frontend:** React + Tailwind CSS  
- **Backend API:** Node.js + Express + Mongoose  
- **Base de Datos:** MongoDB  
- **Despliegue:** Render  
- **Repositorio:** GitHub  

---

##  Patrones de Diseño Seleccionados

### **Arquitectura Base**
- **MVC (Model-View-Controller):**  
  Mantiene el sistema organizado, separando la lógica de negocio, la interfaz de usuario y el control del flujo.

### **Creacionales**
- **Singleton:**  
  Aplicado a la conexión con la base de datos (MongoDB) para asegurar una única instancia global, evitando duplicaciones y mejorando la eficiencia.

### **Estructurales**
- **Facade:**  
  Simplifica el manejo de módulos complejos como generación de reportes, exportación a PDF y dashboard, ofreciendo una interfaz clara y única.

### **De Comportamiento**
- **Strategy (opcional):**  
  Útil para manejar diferentes algoritmos intercambiables, como métodos de autenticación, estrategias de búsqueda o generación de reportes.  

- **Observer (opcional):**  
  Permite implementar notificaciones en tiempo real o actualizaciones automáticas del dashboard cuando se registra una venta o cambia el stock.

---

##  Justificación
La combinación de estos patrones permite:
- **Orden y mantenibilidad:** gracias a MVC.  
- **Eficiencia y control:** garantizados por Singleton en la conexión a la DB.  
- **Claridad y simplicidad:** mediante Facade en subsistemas complejos.  
- **Flexibilidad y escalabilidad futura:** con Strategy y Observer para adaptarse a nuevos escenarios.  

De esta forma, el sistema logra una base sólida para su desarrollo inicial y se prepara para evolucionar sin perder organización.
