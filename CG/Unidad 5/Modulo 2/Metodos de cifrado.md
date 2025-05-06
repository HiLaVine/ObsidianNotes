## Fundamentos de la criptografía

### ¿Qué es la criptografía?

Esta convierte a la información de forma que los no destinatarios no puedan entenderla. Cualquier tipo de dato se mantiene en secreto mediante un proceso de dos pasos: 
1. Cifrado para ocultar la información
2. Descifrado para revelar la información

### Contexto de la criptografia

Este metodo para cuidar la información lleva mucho existiendo, incluso antes que la computación. Uno de los primeros métodos conocidos, es el cifrado de César. Este metodo lleva el nombre del general romano Julio César. Este es un algoritmo simple que mueve las letras romanas un cierto número de espacios. Y este puede ser cualquier numero, por ejemplo:

Un cifrado de César con desplazamiento 3 deja la palabra "hello" como "khoor" (abecedario sin ñ).

Y para poder decifrarlo necesitas la cantidad de desplazamientos, y esto se le conoce como la llave. 

En criptografia una clave criptografica es un mecanismo que descifra el texto cifrado. En el ejemplo, la clave indica de 3 desplazamiento.  

## Ingraestructura de clave pública PKI

Es un marco de cifrado que protege el intercambio de datos en linea, es un sistema amplio que facilita y protege el acceso a la información. 

### ¿Comó funciona?

El PKI es un proceso de dos pasos. Empieza con el intercambio de información cifrada. Esto implica cifrado asimetrico, simetrico o ambos. 

- Cifrado Asimetrico: usa una clave publica y una privada para cifrar y descifrar datos.
- Cifrado Simetrico: este permite gestionar claves de forma rapida y simple. Este solo usa una sola clave secreta para intercambiar infomacion.

El PKI aborda la vulnerabilidad de compartir claves creando confianza con un sistema de certificados digitales entre computadoras y redes. Un certificado digital es un archivo que verifica la identidad de un titular de clave pública. La mayoría de la información en línea se intercambia usando certificado digital. Los usuarios, empresas y redes poseen uno y los intercambian al comunicar información en línea como una forma de señalar confianza. 
