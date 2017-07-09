## Lingẅars notebooks

Conjunto de cuadernos de Jupyter utilizados en talleres que hemos ido realizando.


#### Nota.-

 * Si utilizas un control de versiones para tus cuadernos de Jupyter sabrás lo inoportuno
que es que te muestre diferencias cada vez que ejecutas una celda. Te recomendamos que
utilices [nbstripout](https://github.com/kynan/nbstripout) para evitarlo; esta aplicación
limpiará el cuaderno antes de hacer un *commit* o un *diff*. Aunque las instrucciones de
instalación son extremadamente simples, te las resumo a continuación:

   * `pip install nbstripout`
   * `nbstripout --install`: debería añadir algunos parámetros de configuración:

        ```
        # git config --list
        [...]
        filter.nbstripout.clean="<path/to/virtualenv/python>" "<path/to/virtualenv/nbstripout.py>"
        filter.nbstripout.smudge=cat
        filter.nbstripout.required=true
        ``` 
   * y también deberías tener un archivo `.gitattributes`:

        ```
        *.ipynb filter=nbstripout
        ```


