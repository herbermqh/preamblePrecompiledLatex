# preamblePrecompiledLatex
## Seguir los siguientes pasos para precompilar precompilar 
1. Nuestro documento LaTeX será de la siguiente forma:
``% static part
...
\endofdump
%dynamic part
...
\begin{document}``
2. Al finalizar la parte estática debemos añadir el comando ``\endofdump``.
3. Abrimos el terminal.
4. Nos vamos al directorio del archivo LaTeX (supongamos que nuestro archivo se llama fisicaII.tex)
5. Ejecutamos el siguiente comando en el terminal.
``xelatex-dev.exe -ini -jobname="fisicaII" "&xelatex" mylatexformat.ltx fisicaII.tex``
6. Comenzará a compilar el documento LaTeX.
7. Si en el compilado aparece 'fisicaII.mtc0' no encontrado, pues solo se debe presionar enter.
8. Una vez finalizado la compilación, se obtendrá un archivo llamdo "fisicaII.fmt".
9. En la primera línea del documento LaTeX (en esta caso fisicaII.tex) se debe añadir ``%&fisicaII``. 
10. El código de la parte estática podemos comentar, eliminar o simplemente dejarlo tal como está.
11. La proxima compilación del documento LaTeX es tres veces más rápido.

*Fuente de tutorial:* https://web.archive.org/web/20160712215709/http://www.howtotex.com:80/tips-tricks/faster-latex-part-iv-use-a-precompiled-preamble/
