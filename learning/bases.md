### Instalación de Lua

Más o menos en cualquier sistema moderno encontrarás Lua instalado por defecto. Puedes verificarlo ejecutando:

```sh
lua -v
```

Si no lo tienes, puedes instalarlo con un gestor de paquetes como Homebrew (en macOS) o apt (en Ubuntu).

### Estructura Básica de un Programa Lua

Un programa Lua es simplemente texto regular. Aquí tienes una estructura básica:

```lua
-- Este es un comentario en lua

print("Hola, Mundo!")
```

### Variables y Tipos de Datos

Lua no necesita declaraciones explícitas de variables. Cuando asignas un valor a una variable, Lua infiere el tipo automáticamente.

#### Números

```lua
number1 = 42
number2 = -3.5
```

Los números son de punto flotante. Lua no distingue entre integers y floats.

#### Cadenas

Las cadenas se definen con comillas.

```lua
string1 = 'Esto es una cadena'
string2 = "Esta también lo es"
```

#### Booleanos

Lua tiene los valores `true` y `false`.

```lua
bool1 = true
bool2 = false
```

#### Nada (nil)

Simila a null o None en Python.

```lua
nil_value = nil
```

### Operadores Basicos

Aquí tienes algunos operadores básicos:

- Aritméticos: `+`, `-`, `*`, `/`

  ```lua
  resultado_suma = 5 + 3
  resultado_resta = 5 - 3
  resultado_multiplicacion = 4 * 2
  resultado_division = 10 / 2
  ```

- Comparación: `==` (igualdad), `~=`, `<`, `>`, `<=`, `>=`
  ```lua
  booleano = 5 == 3
  otro_booleano = "hola" == "adios"
  ```
- Lógicos: `and`, `or`, `not`
  ```lua
  verdad = true and false
  falso = not verdad
  ```

### Estructuras de Datos

Lua tiene tres tipos básicos de estructuras de datos:

1. Tablas (Arrays y Diccionarios)
2. Strucs (tuplas)
3. Nil (vacío)

#### Tablas (Matrices)

Las tablas en Lua podrían ser pensadas como listas o diccionarios. Aquí tienes un ejemplo:

```lua
miTabla = {"a", "b", "c"}

print(miTabla[1])  -- Imprime 'a'
```

Además, puedes crear tablas como diccionarios de la siguiente manera:

```lua
miDiccionario = {nombre="Alice", edad=30}

print(miDiccionario.nombre)  -- Imprime 'Alice'
```

#### Funciones

Aquí tienes un ejemplo básico de cómo definir y usar funciones:

```lua
-- Definir una función
function saludos(nombre)
    return "Hola, " .. nombre .. "!"
end

-- Usar la función
resultado = saludos("Juan")
print(resultado)  -- Imprime 'Hola, Juan!'
```

### Control Flow

Lua tiene los constructos típicos de control flow que esperas en cualquier lenguaje moderno.

#### If Statement

```lua
if edad >= 18 then
    print("Eres mayor de edad.")
else
    print("Eres menor de edad.")
end
```

#### For Loops

`for` puede trabajar con índices y también puede ser utilizado para iterar sobre tablas.

```lua
for i=1, 5 do
    print(i)  -- Imprime números del 1 al 5
end

-- Iteración sobre una tabla
miTabla = {"a", "b", "c"}

for indice, valor in ipairs(miTabla) do
   print(indice, valor)
end
```

#### While Loops

```lua
i = 0
while i < 3 do
    print(i)  -- Imprime números del 0 al 2
    i = i + 1
end
```

### Return

Las funciones en Lua pueden devolver múltiples valores.

```lua
function suma_y_resta(a, b)
    return a + b, a - b
end

s, r = suma_y_resta(5, 3)
print(s)  -- Imprime '8'
print(r)  -- Imprime '2'
```

### Resumen

Aquí tienes un resumen conceptual de lo que acabamos de cubrir:

1. Variables y Tipos de Datos
2. Operadores Básicos
3. Estructuras de Datos (Tablas, Strucs, Nil)
4. Funciones
5. Control Flow (If-Statement, For-Loops, While-Loops)
6. Return

Estas son las bases del lenguaje Lua y te darán una buena comprensión para seguir trabajando en problemas más complicados. ¡Sigue adelante con ejercicios adicionales y proyectos para practicar y fortalecer tus conocimientos!
