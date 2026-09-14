# Fullstack
Caso semestral de fullstack SaludPlus

# SaludPlus - Sistema de Gestión de Farmacia Comunitaria

Proyecto web desarrollado para la farmacia comunitaria **SaludPlus** (ubicada en Maipú, Región Metropolitana), diseñado para resolver los problemas de desabastecimiento, control manual y gestión de stock mediante una plataforma multipágina limpia, moderna y funcional.

---

# Resumen del Caso de Negocio

| Categoría | Descripción / Detalle |
| :--- | :--- |
| **Ubicación & Experiencia** | Comuna de Maipú, Región Metropolitana. Más de 8 años en el sector farmacéutico. |
| **Volumen Operativo** | Promedio de **200 clientes diarios** y más de **1.500 transacciones mensuales**. |
| **Problemática Actual** | Crecimiento del 30% en la demanda en los últimos tres años, lo que tensionó el sistema manual basado en planillas Excel y POS básico (provocando desabastecimiento, pérdida por vencimiento y errores de precios). |
| **Equipo Humano** | 3 farmacéuticos, 4 vendedores, 1 encargado de inventario, 1 encargado de compras y 1 administrador. |

---

# Actores Involucrados y Roles en el Sistema

| Actor | Rol en el Proceso | Relación con el Sistema |
| :--- | :--- | :--- |
| **Cliente** | Compra productos farmacéuticos y de cuidado personal. | Realiza compras en la tienda online y visualiza catálogo en tiempo real. |
| **Vendedor** | Atiende al público y registra ventas. | Utiliza el sistema POS integrado para gestionar transacciones. |
| **Farmacéutico** | Dispensa medicamentos y asesora. | Revisa stock físico y apoya en la validación de dispensaciones. |
| **Encargado de Inventario** | Gestiona el stock y conteos de bodega. | Reemplaza las planillas manuales por el panel de control de inventario digital. |
| **Encargado de Compras** | Gestiona reposiciones y proveedores. | Controla el flujo de abastecimiento y pedidos. |
| **Administrador** | Finanzas y estrategia gerencial. | Accede al panel gerencial con métricas y reportes consolidados. |

---

# Estructura y Vistas de la Solución Frontend

El desarrollo frontend está estructurado en vistas interconectadas mediante JavaScript, simulando una arquitectura multipágina sin necesidad de base de datos relacional:

| Módulo / Vista | Archivo Asociado | Descripción Funcional |
| :--- | :--- | :--- |
| **Tienda Online (Cliente)** | `index.html` (Vista Cliente) | Catálogo interactivo de medicamentos con buscador, carrito flotante y diseño institucional. |
| **Checkout de Compras** | `index.html` (Vista Checkout) | Formulario de datos personales del cliente con validación estricta de campos vacíos, edad, selector dinámico de Región/Comuna y campo condicional de Departamento/Edificio. |
| **Acceso Administrador** | `index.html` (Vista Admin Login) | Inicio de sesión simulado para el panel gerencial. |
| **Panel Gerencial (Admin)** | `index.html` (Vista Admin Dashboard) | Estadísticas de ventas mensuales, transacciones y control financiero. |
| **Acceso Inventario** | `index.html` (Vista Inventario Login) | Inicio de sesión simulado exclusivo para el control de bodega. |
| **Control de Stock** | `index.html` (Vista Inventario Dashboard) | Listado maestro de productos con alertas automáticas de **Stock Crítico**. |

---

# Tecnologías y Arquitectura de Archivos

El código se encuentra modularizado en tres archivos independientes para facilitar su mantenimiento y despliegue:

| Componente | Archivo | Descripción Técnica |
| :--- | :--- | :--- |
| **Estructura** | `index.html` | Contiene el esqueleto semántico y las secciones conmutables de todas las vistas del sistema. |
| **Estilos** | `style.css` | Hoja de estilos basada en variables CSS, diseño responsivo (Flexbox/Grid) y colores claros con el verde institucional de SaludPlus. |
| **Lógica** | `script.js` | Controla el enrutamiento de vistas, arreglos de productos, carrito de compras, validación de formularios y manejo dinámico del DOM. |

---

# Instrucciones de Uso

1. Clona o descarga los tres archivos principales en tu equipo:
   * `index.html`
   * `style.css`
   * `script.js`
2. Coloca tu archivo de logotipo en la carpeta bajo el nombre `logo.png`.
3. Abre **`index.html`** en cualquier navegador web moderno.
4. Para explorar las vistas protegidas, haz clic en **Admin** o **Inventario** en la barra superior (los accesos vienen prellenados para facilitar la revisión inmediata).

---

# Bitácora de Desarrollo y Control de Versiones

# Benjamin Reyes parte 10/09/26

Para la primera parte se creo una base en Balsamiq para poder recrear una pagina como lo solicita el pedido de SaludPlus, con esto en la parte de estructura nos inspiramos en la pagina del Doctor Simi con esto se ocupo los indicadores de productos y tamaño de letras lo mas parecidos posible, un detalle que tuve fue el no poder ver bien el como hacer que se pueda tener 3 cuentas a la vez (user, admin, bodega).

# Benjamin Reyes 11/09/26

Con la investigación de otras paginas de farmacias se me ocurrió la idea de hacer un "inicio de sesión" que solo sea un boton que al presionarlo te mande una vista de cada rol, dependiendo la opcion seleccionada te manda la vista de administrador, bodega o usuario, con eso en mente recree una interfaz ya utilizada anteriormente para poder recrear un "inicio de sesion" sin BD.


# Michael Santibañez 12/09/2026

con dicho por mi compañero benjamin yo fui encargardo de hacer el CSS para que la paguina web se vea mejor a la vista del usuario y que no sea tas tosaca y insipida y con ello lo que llegue a hacer fue poner el color de fondo, el como se veria los botone y casi todo lo que se tratara de una vista mas agradable para que el usuario pueda guiarse de una forma mas eficas dentro del sitio web


# Felipe Fredes 12/09/2026

# UPDATE 0.1.0

Con lo investigado y el diseño hecho por nuestro compañero Michael, podemos dar ya la primera versión de nuestra pagina SALUDPLUS 0.1.0 este incluye vista de administrador, gestion de inventario, carrito de compras logo y todo lo que se pide en la rubrica estamos a nada ya de sacarlo al publico. Falta pulir los ultimos detalles y estamos listos para el release de la 1.0.

# Benjamin Reyes, Felipe Fredes, Michael Santibañez

# UPDATE FINAL 1.0

Ya con lo hecho con la version anterior y viendo que es totalmente funcional decidimos entre todos ya dar por finalizada la creacion y gestion de nuesta pagina de Saludplus
Cumpliendo asi la evaluacion heuristica lo cual era totalmente opcional pero decidimos usarlo aun asi para darle mas profesionalidad con esto damos por finalizado esto //
