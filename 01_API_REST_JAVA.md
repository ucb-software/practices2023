# Creacion de API REST en Java y consumo Web.

Instrucciones:

1. Crear un nuevo repositorio en Github: practica-contenedor.
2. Ingresar a start.spring.io y crear un proyecto. No olvidar agregar la dependencia WEB.
3. Subir el proyecto del punto 2 al repositorio creado en el punto 1.
4. Agregar un endpoint REST al proyecto Java que implemente lo siguiente (Sin BBDD todo en memoria).
	GET /api/v1/task
	[
	  {
		taskId: 1
		name: Hacer mi tarea
		dueDate: 25/12/2023
		status: PENDING
	 } ...
	]
	
	POST /api/v1/task 
	  {
		name: Hacer mi tarea
		dueDate: 25/12/2023
		status: PENDING
	 } 

	DELETE /api/v1/task/1 

5. Crear la imagen docker de la aplicación JAVA.
6. Exponer la aplicación con un NGINX por delante del JAVA haciendo Reverse Proxy.
7. Agregar al NGINX una app Web sencilla que consuma el API.