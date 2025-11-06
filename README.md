# Proyecto: Constructores y Objetos en JavaScript

Este proyecto contiene ejercicios para aprender sobre constructores, objetos y el uso de `this` en JavaScript.

## Tareas Realizadas

### Task 1: Mail Object Básico
- utilizamos un constructor `Mail` con propiedades fijas
- **Aprendimos**: Cómo definir un constructor básico y crear instancias con `new`

### Task 2: Mail con Parámetros de Ejecución  
- Modificamos el constructor para recibir parámetros desde `process.argv`
- **Aprendimos**: Cómo acceder a argumentos de línea de comandos y asignarlos a propiedades

### Task 3: Mail con Método
- Agregamos el método `printMail()` al constructor
- **Aprendimos**: Cómo definir métodos dentro de constructores que pueden acceder a las propiedades del objeto

### Task 4: Constructor Journey
- Creamos mi propio constructor `Journey` que toma parámetros start y end
- **Aprendimos**: Cómo diseñar un constructor desde cero y usarlo con datos dinámicos

### Task 5: FriendsList con Array
- Implementamos un constructor que almacena nombres en un array
- **Aprendimos**: Cómo trabajar con arrays dentro de objetos y recoger input del usuario

## Conceptos Clave Aplicados

### Uso de `this`
- **`this`** se refiere a la instancia actual del objeto
- Se usa dentro de constructores para asignar propiedades: `this.propiedad = valor`
- Permite que cada objeto mantenga sus propios valores

### Constructores
- **Función constructora**: `function NombreConstructor(parametros) { ... }`
- Sirven como plantilla para crear múltiples objetos similares
- Definen la estructura y comportamiento de los objetos

### Operador `new`
- **`new Constructor()`** crea una nueva instancia del objeto
- Asigna memoria para el nuevo objeto
- Establece el contexto de `this` para esa instancia
- Retorna automáticamente el nuevo objeto

## Ejemplo de Flujo
```javascript
// 1. Definir constructor
function Persona(nombre) {
    this.nombre = nombre;
}

// 2. Crear instancia
const persona1 = new Persona("María");

// 3. Usar el objeto
console.log(persona1.nombre); // "María"
