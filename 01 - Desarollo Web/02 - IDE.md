## Editor de código
- **Prettier** -> Formatea el código de forma bonita.
	- Intalarlo por **npm**
	- Usarlo para *desarollo*
	- Usarlo para *proyectos* *(cada proyecto con su version y configuración idependiente)*

- **GESTOR DE PAQUETES**
	- Le pasaras tu código, no todo el proyecto compilado *(receta de cocina)*
	- Documentaras las dependencias *(librerias)* que hacen falta para que el código funcione correctamente *(utensilios de cocina que debe usar)*

### Intalación
1. Desde la consola de comandos de Visual Code, ir a la ruta de tu protecto donde este el index.

2. Insertar:
```bash
npm init
#Enter hasta decir yes
```

3. Instalar Prettier
```bash
npm install -D prettier
```

4. Crear un fichero **.prettierrc.json** (con dos llaves):
```bash
echo {}> .prettierrc.json
```

5. Instalar ***Prettier - Code formatter*** en Visual Code

6. Añade esto en el package.json:
```json
"devDependencies": {

"prettier": "^2.8.4"

}
```

7. Sigue [[versión semántico]].
¿Qué es el versionado semántico?

8. También se crea un package-lock.json con mis dependecias concretas

9. Instalar la extension Prettier en el Visual Code

### Instalar otros plugins
- **Live Server** en VS code -> Te ejecuta la web en un servidor sin tener que ir directo a un navegador.

- **Quokka** en VS code -> Para crear archivos .js que te ayuda a visibilizar si el código esta funcionando correctamente.

- **Linters** (*eslint*)-> Corrector semántico de código
```bash
npm install --save-dev eslint-config-prettier
```

	- yes el configurador
	- el que tiene todo (estilo)
	- El resto lo que estemos usando
	- contestar preguntas
	- json