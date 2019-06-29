# dom-parser

Parser DOM de expresiones regulares adaptado a Velneo, basado en
[@ershov-konst/dom-parser](https://github.com/ershov-konst/dom-parser)

## Instalación

Importar el fichero dom-parser.js en los scripts de un proyecto.

## Uso

    #import (CurrentProject)/DomParser.js #TEST_DAT

    var html = '<html><body><h1 id="titulo">DomParser</h1><p>Párrafo 1</p><p>Párrafo 2</p></body></html>';

    var parser = new DomParser();
    var dom = parser.parseFromString(html);

    alert(dom.getElementById('titulo').innerHTML);
    var p = dom.getElementsByTagName('p');
    for(var i in p){
        alert(p[i].innerHTML);
    }

## API

##### Dom

Métodos implementados:

* getElementById
* getElementsByClassName
* getElementsByTagName
* getElementsByName

##### Node

Propiedades implementadas:

* nodeType
* nodeName
* childNodes
* firstChild
* lastChild
* parentNode
* attributes
* innerHTML
* outerHTML
* textContent

Métodos implementados:

* getAttribute
* getElementById
* getElementsByClassName
* getElementsByTagName
* getElementsByName

Uso - https://developer.mozilla.org/en-US/docs/Web/API/HTMLElement


## contributing

issues and pull requests are welcome!

## Credits

Basado en https://github.com/ershov-konst/dom-parser

This is forked from [@ershov-konst/dom-parser](https://github.com/ershov-konst/dom-parser).
