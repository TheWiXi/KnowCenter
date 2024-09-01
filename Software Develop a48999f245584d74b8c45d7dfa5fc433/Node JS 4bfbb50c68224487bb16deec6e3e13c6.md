# Node JS

- Modulos:
    - CommonJs (Clasica-Antigua)
        
        ```jsx
        //Exportar 
        function NombreFuncion(){
        	return()
        }
        module.exports = NombreFuncion
        //importar 
        const aliasFuncion = require('./rutaArchivo')
        //Exportar como objetos
        function NombreFuncion(){
        	return()
        }
        module.exports={
        	NombreFuncion
        }
        //importar
        const {NombreFuncion} = require('./rutaArchivo')
        
        //importar modulos nativos
        require('node:MODULO')
        ```
        
    - ES Modules
        
        ```jsx
        //extensiones obligatorias
        //Exportar elarchivo es m.js
        export function NombreFuncion(){
        	return()
        }
        //importar
        import {Funciones} from './rutaArchivo.js'
        ```