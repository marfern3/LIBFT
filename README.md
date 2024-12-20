# LIBFT

Libft es un proyecto de 42 que consiste en crear una biblioteca de funciones en C desde cero. Este proyecto te permite profundizar en conceptos básicos de la programación, como el manejo de cadenas, memoria, listas enlazadas y manipulación de archivos.

## Tabla de Contenidos

- [Introducción](#introducci%C3%B3n)
- [Requisitos](#requisitos)
- [Funciones Implementadas](#funciones-implementadas)
- [Uso](#uso)
- [Testing](#testing)
- [Recursos](#recursos)
- [Contribuciones](#contribuciones)
- [Licencia](#licencia)

---

## Introducción

Libft es una biblioteca personal que implementa funciones estándar de la biblioteca de C y algunas funciones adicionales útiles para la programación. Es el primer paso para familiarizarte con los estándares de código de 42 y aprender sobre compilación y uso de bibliotecas personalizadas.

El proyecto incluye:
- Reimplementación de funciones de `libc`.
- Funciones para manejo de cadenas y memoria.
- Manejo de listas enlazadas.

## Requisitos

Para compilar y usar Libft, necesitarás:

- Un sistema compatible con UNIX (Linux o macOS).
- `gcc` (GNU Compiler Collection).
- `make`.

## Funciones Implementadas

### Parte Obligatoria

| Categoría           | Funciones                                     |
|---------------------|----------------------------------------------|
| Manipulación de cadenas | `ft_strlen`, `ft_strchr`, `ft_strdup`, etc. |
| Memoria             | `ft_memset`, `ft_memcpy`, `ft_calloc`, etc.  |
| Conversiones        | `ft_atoi`, `ft_itoa`                         |
| Entrada/Salida      | `ft_putchar_fd`, `ft_putstr_fd`, etc.        |

### Parte Bonus

| Categoría           | Funciones                                     |
|---------------------|----------------------------------------------|
| Listas Enlazadas    | `ft_lstnew`, `ft_lstadd_front`, `ft_lstdelone`, etc. |

## Uso

### Compilación

Para compilar la biblioteca, simplemente ejecuta el siguiente comando en la terminal:

```bash
make
```

Esto generará el archivo `libft.a`, que podrás usar en tus proyectos. Para limpiar los archivos objetos:

```bash
make clean
```

Para limpiar todos los archivos generados:

```bash
make fclean
```

### Integración

Para usar la biblioteca en tu proyecto, incluye `libft.h` en tus archivos `.c` y compila tu proyecto enlazando el archivo `libft.a`:

```bash
gcc -Wall -Wextra -Werror -L. -lft -o programa archivo.c
```

## Testing

### Pruebas Internas

Se proporciona un archivo `main.c` que contiene pruebas básicas para verificar las funciones implementadas.

```bash
gcc -Wall -Wextra -Werror -o test main.c libft.a
./test
```

### Pruebas Externas

Recomendamos usar testers externos como:
- [libft-unit-test](https://github.com/alelievr/libft-unit-test)
- [libftTester](https://github.com/Tripouille/libftTester)

## Recursos

- [Norminette](https://github.com/42School/norminette): Para verificar que tu código cumple con las normas de 42.
- [Documentación de la libc](https://www.man7.org/linux/man-pages/): Para entender las funciones estándar de C.

## Contribuciones

Si deseas contribuir o tienes sugerencias, siéntete libre de abrir un issue o enviar un pull request.

## Licencia

Este proyecto es parte del currículo de 42 y no tiene una licencia específica. Está destinado únicamente para fines educativos.

