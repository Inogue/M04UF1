# Codigo y docmuentacion M04-UF1
Ciberseguridad: Llenguatge de marques

## **_XML_**

  En **_XML_** es necesario comenzar agregando ```XML \<?xml version="1.0" encoding="UTF-8" ?>```, esto es una cabecera. 
  
  Gracias a esta etiqueta el lenguaje puede funcionar correctamente. 
  
  En todo archivo **XML** es necesario que haya una etiquieta raiz.
  
  Existen varios tipos de etiquetas:
  
  * Pares
  * Impares 
  * Booleanas
   
  **PARES:** Estas etiquetas son las que tienen una etiqueta para abrir y otra para cerrar. _EJEMPLO:_```XML <name>Eustaquio\</name>```
  
  **IMPARES:** Estas etiquetas solo necesitan una etiqueta que cierre. _EJEMPLO:_ ```XML <age years="197" />```
  
  **BOOLEANAS:** Con esta etiqueta puedes determinar el estado de una variable por defecto, si es true o false. _EJEMPLO:_ ```XML <tienelaeso />``` 
  
  Para que todos los archivos xml sigan una estructura concreta es necesario que haya un archivo que determine dicha estructura. 
  El lenguaje de estas estructuras pueden ser **DTD** o **XSD**.
 

## **_DTD_**
Los _apuntes_ de **DTD**

```dtd
<!ELEMNT character (name, surname, age, race, 
 class,gender, height,
 weight, language, tienelaeso?, weapons?)>
<!ELEMENT name (#PCDATA)>
<!ELEMENT surname (#PCDATA)>
<!ELEMENT age EMPTY>
<!ELEMENT race (#PCDATA)>
<!ELEMENT class (#PCDATA)>
<!ELEMENT gender (#PCDATA)>
<!ELEMENT height EMPTY>
<!ELEMENT weight EMPTY>
<!ELEMENT language (#PCDATA)>
<!ELEMENT tienelaeso EMPTY>
<!ELEMNT weapons (weapon*)>
<!ELEMENT weapon EMPTY>

<!ATTLIST age years CDATA #REQUIRED>
<!ATTLIST gender abbrev CDATA #REQUIRED>
<!ATTLIST height cm CDATA #REQUIRED>
<!ATTLIST weight kg CDATA #REQUIRED>
<!ATTLIST language abbrev CDATA #REQUIRED>
<!ATTLIST language prefix CDATA>
<!ATTLIST id_weapon CDATA #REQUIRED>

```
Gracias a esto tenemos un estandar para los archivos de characters en XML. 


## **_MarkDown_**

### Listas
* uno
* dos
	* sub dos
		* sub sub normal
* tres


### Citaciones

> Un gran poder conlleva
> una gran responsabilidad
>
> -Carmen de Mairena

> Esto es citar
>> Esto es citar por dos
>
> Ya no se cita


---
### Enlaces

Un enlace a la mejor web del mundo

[CondorChem](https://condorchem.com)

Y [ESTO](https://enti.cat) es otro enlace.


### Imagen incrustada

![African Lore](https://i.ytimg.com/vi/z-EU53ib2M4/maxresdefault.jpg)

### EJEMPLO DE CODIGO RESALTADO

```kotlin
fun main(args: Array<String>){
print("A")
}
```

---

### Lista de tareas

- [ ] Primera cosa
- [X] COSA

### Caracteres extendidos

:poop: :alien: :cry: :imp: :banana:

### Estilos de caracteres

_A_
~~A~~

### Tablas


| id_character | name | age | level |
| ---: | ---: | ---: | ---: |
| 1 | Eustaquio | 197 | 99 |
| 2 | Mariana | 20 | 100 | 
| 3 | Mortadelo | 100 | 1 |
| 4 | Messi | 44 | 32 |