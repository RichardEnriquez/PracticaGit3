![img](https://www.syloper.com/wp-content/uploads/git_destacada-1024x426.png)

**Caso 1:**

¿como usar ramas para crear nuevas funcionalidades?

Como ya tenemos un proyecto base “es decir una versión funcional” en el repositorio tendremos que crearnos una rama develop para crear nuevas funcionalidades

Primero tendremos que crear una rama “develop”:

git branch develop

![image-20200306171223310](https://github.com/RichardEnriquez/PracticaGit3/blob/master/img/image-20200306171223310.png)

después de crearla nos tendremos que cambiar de rama:

git checkout develop

![image-20200306171323427](https://github.com/RichardEnriquez/PracticaGit3/blob/master/img/image-20200306171323427.png)

Ahora como estamos en la rama develop podremos crear nuevas funcionalidades y subirlas a la rama develop:

![image-20200306171423530](https://github.com/RichardEnriquez/PracticaGit3/blob/master/img/image-20200306171423530.png)

![image-20200306171427601](https://github.com/RichardEnriquez/PracticaGit3/blob/master/img/image-20200306171427601.png)

![image-20200306171438843](https://github.com/RichardEnriquez/PracticaGit3/blob/master/img/image-20200306171438843.png)

![image-20200306171457308](https://github.com/RichardEnriquez/PracticaGit3/blob/master/img/image-20200306171457308.png)

Luego de subir las nuevas funcionalidades a la rama develop podremos unir a la rama master (si ya están aprobadas claro)

Primero nos movemos a la rama que queremos unificar, en mi caso master![image-20200306171518401](https://github.com/RichardEnriquez/PracticaGit3/blob/master/img/image-20200306171518401.png)

Luego hacemos un merge (“merge se utiliza para unificar 2 ramas”)![image-20200306171528638](https://github.com/RichardEnriquez/PracticaGit3/blob/master/img/image-20200306171528638.png)

Ahora si hacemos un git log podremos ver los nuevos commits que vinieron de la rama develop![image-20200306171655536](https://github.com/RichardEnriquez/PracticaGit3/blob/master/img/image-20200306171655536.png)

Como vemos hay 2 commits nuevos “estos commits son los que estuvieron en la rama develop”, tendremos que hacer un push para guardar los cambios en rama master

**Caso 2:**

¿como puedo resolver un conflicto?

en este caso creare un conflicto y luego lo resolvere

Primero tendremos que invitar al compañero al repositorio e Indicaremos que edite una línea ![image-20200306171835429](https://github.com/RichardEnriquez/PracticaGit3/blob/master/img/image-20200306171835429.png)![image-20200306171842077](https://github.com/RichardEnriquez/PracticaGit3/blob/master/img/image-20200306171842077.png)

Ahora que él tiene editado la función tendrá que comittear sobre ella para luego hacer un push al repositorio.

Ahora como yo no hice un pull del proyecto podre crear un conflicto editando esa misma línea y hacer un commit para intentar subir al repositorio                            ![image-20200306171907264](https://github.com/RichardEnriquez/PracticaGit3/blob/master/img/image-20200306171907264.png)![image-20200306171937646](https://github.com/RichardEnriquez/PracticaGit3/blob/master/img/image-20200306171937646.png)

Hacemos un commit sobre este cambio ![image-20200306171945874](https://github.com/RichardEnriquez/PracticaGit3/blob/master/img/image-20200306171945874.png)

Al intentar hacer un push veremos que nos salta un conflicto![image-20200306171959965](https://github.com/RichardEnriquez/PracticaGit3/blob/master/img/image-20200306171959965.png)

Lo que tendremos que hacer es hacer pull del repositorio y veremos que nos informa que hay conflictos para resolver:![image-20200306172008182](https://github.com/RichardEnriquez/PracticaGit3/blob/master/img/image-20200306172008182.png)

Para poder arreglar un conflicto tendremos que dirigirnos al lugar donde editamos el archivo![image-20200306172015154](https://github.com/RichardEnriquez/PracticaGit3/blob/master/img/image-20200306172015154.png)

Como vemos están los dos cambios que hicimos.

![image-20200306172034590](https://github.com/RichardEnriquez/PracticaGit3/blob/master/img/image-20200306172034590.png)

Ahora hacemos el commit de este cambio y pusheamos

Y listo :D así se puede arreglar un conflicto

![image-20200306172100977](https://github.com/RichardEnriquez/PracticaGit3/blob/master/img/image-20200306172100977.png)

