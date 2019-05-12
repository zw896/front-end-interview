## JS
1. null and undefined
    
    null:
    - null is an empty or non-existent value.
    - null must be assigned.

    undefined:
    - Undefined most typically means a variable has been declared, but not defined.

    null and undefined are two of the six falsy values /  primitive values.

    ```javascript
    let a = null;
    let b;
    console.log(typeof a);
    // object
    console.log(typeof b);
    // undefined
    ```

    With default parameters, undefined will use the default while null does not.
    ```javascript
    let logHi = (str = 'hi') => {
        console.log(str);
    }
    logHi(undefined);
    // hi
    logHi(null);
    // null
    ```

2. The JavaScript this Keyword

    The JavaScript this keyword refers to the object it belongs to.
    It has different values depending on where it is used:
    - Method: owner object.
    - Alone: global object.
    - Function: global object.
    - Function (in strict mode): this is undefined.
    - Event: element that received the event.
    - Methods like call(), and apply(): can refer this to any object.

3. Explain the difference between "==" and "==="?
"==" checks only for equality in value whereas "===" is a stricter equality test and returns false if either the value or the type of the two variables are different.

4. 