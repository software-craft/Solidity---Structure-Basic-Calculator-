# Solidity Calculator Contract

## Description

This `Calculator` contract is designed as an educational example to practice good Solidity practices. It combines basic technical skills like:

- State management
- Modifiers
- Events
- Function visibility
- Internal logic separation

The main focus is readability, structure, and solid fundamentals.

# Calculator Contract Documentation

## Variables

- `resultado`: public value of type `uint256` initialized to 10.

## Modifiers

- `checkNumber(uint256 num1_)`: checks that `num1_` is 10, otherwise the transaction reverts.

## Events

- `Addition(uint256 number1, uint256 number2, uint256 resultado)`: emitted when two numbers are added.  
- `Substraction(uint256 number1, uint256 number2, uint256 resultado)`: emitted when two numbers are subtracted.

## External Functions

- `addition(uint256 num1_, uint256 num2_)`: adds two numbers and emits an `Addition` event.  
- `substraction(uint256 num1_, uint256 num2_)`: subtracts two numbers using internal logic and emits a `Substraction` event.  
- `substraction2(int256 num1_, int256 num2_)`: subtracts two integer numbers using internal logic, pure function.  
- `multiplier(uint256 num1_)`: multiplies the `resultado` variable by `num1_`.  
- `multiplier2(uint256 num1_)`: multiplies `resultado` by `num1_` only if `num1_` is 10 (checked by `checkNumber`).  

## Internal Functions

- `subtraction_logic(uint256 num1_, uint256 num2_)`: internal logic to subtract `uint256` numbers.  
- `subtraction_logic2(int256 num1_, int256 num2_)`: internal logic to subtract `int256` numbers.  

## Notes

This contract is used to understand the structure of a Solidity contract, practice separation of logic, events, and modifiers, and apply good practices in Smart Contract development.





# Calculadora Solidity Contract

## Descripción

Este contrato `Calculadora` está diseñado como ejemplo educativo para practicar buenas prácticas en Solidity. Combina habilidades técnicas básicas como:

- Manejo de estado
- Modifiers
- Eventos
- Visibilidad de funciones
- Separación de lógica interna

El enfoque principal es la legibilidad, la estructura y fundamentos sólidos.

# Documentación del Contrato Calculadora

## Variables

- `resultado`: valor público de tipo `uint256` inicializado en 10.

## Modifiers

- `checkNumber(uint256 num1_)`: valida que `num1_` sea igual a 10, de lo contrario revierte la transacción.

## Eventos

- `Addition(uint256 number1, uint256 number2, uint256 resultado)`: emitido al sumar dos números.  
- `Substraction(uint256 number1, uint256 number2, uint256 resultado)`: emitido al restar dos números.

## Funciones Externas

- `addition(uint256 num1_, uint256 num2_)`: suma dos números y emite un evento `Addition`.  
- `substraction(uint256 num1_, uint256 num2_)`: resta dos números usando lógica interna y emite un evento `Substraction`.  
- `substraction2(int256 num1_, int256 num2_)`: resta dos números enteros, usando lógica interna, función `pure`.  
- `multiplier(uint256 num1_)`: multiplica la variable `resultado` por `num1_`.  
- `multiplier2(uint256 num1_)`: multiplica `resultado` por `num1_` solo si `num1_` es 10 (verificado por `checkNumber`).  

## Funciones Internas

- `subtraction_logic(uint256 num1_, uint256 num2_)`: lógica interna para restar números `uint256`.  
- `subtraction_logic2(int256 num1_, int256 num2_)`: lógica interna para restar números `int256`.  

## Notas

Este contrato sirve para comprender la estructura de un contrato Solidity, practicar separación de lógica, eventos y modifiers, y aplicar buenas prácticas en desarrollo de Smart Contracts.
