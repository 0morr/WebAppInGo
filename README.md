# Desarrollo un mock de una web app en Go

Una aplicación simple de lista de tareas construida con Go, HTMX y Petite-vue. Permite crear, completar y eliminar tareas con una interfaz moderna y responsiva.

## Características

* Interfaz de usuario moderna con Tailwind CSS
* Actualizaciones en tiempo real con HTMX
* Backend rápido y eficiente en Go
* Estado reactivo del frontend con Petite-vue
* Diseño responsivo

## Tecnologías Utilizadas

* **Backend**

  * Go 1.21
  * Fiber v2 (Framework web)
  * UUID para identificadores únicos

* **Frontend**

  * HTMX para interacciones con el servidor
  * Petite-vue para reactividad
  * Tailwind CSS para estilos

## Prerrequisitos

* Go 1.21 o superior
* Git

## Instalación

1. Clona el repositorio

```bash
git clone https://github.com/0morr/WebAppInGo.git
cd my-todo-app
```

2. Instala las dependencias

```bash
go mod tidy
```

3. Ejecuta la aplicación

```bash
go run main.go
```

4. Abre tu navegador y visita `http://localhost:3000`

## Estructura del Proyecto

```
todo-list-app/
├── main.go              # Código principal del servidor
├── go.mod              # Dependencias de Go
├── go.sum              # Checksums de las dependencias
├── index.html          # Frontend de la aplicación
├── README.md           # Esta documentación
└── .gitignore         # Archivos ignorados por git
```

## API Endpoints

### GET /api/tasks

Obtiene todas las tareas.

### POST /api/tasks

Crea una nueva tarea.

```json
{
    "name": "Nueva tarea"
}
```

### PUT /api/tasks/toggle/:id

Marca una tarea como completada o no completada.

### DELETE /api/tasks/:id

Elimina una tarea.

## Contribuir

1. Fork el proyecto
2. Crea tu rama de características (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add: alguna característica asombrosa'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

## Por Hacer

* [ ] Persistencia de datos
* [ ] Autenticación de usuarios
* [ ] Categorías para las tareas
* [ ] Fechas límite
* [ ] Filtros y búsqueda

## Licencia

Este proyecto está bajo la Licencia MIT - ver el archivo [LICENSE](LICENSE) para más detalles.
