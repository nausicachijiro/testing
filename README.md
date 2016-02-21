# Ejemplo de como tener varias cuentas en github

* Pseudo alumno para probar en GitHub
* Usando nausicachihiro
* He creado la clave `chuchu` con `ssh-keygen` y la he publicado en github 
* Véase esta entrada en `~/.ssh/config`

            Host github-nausica.com
            HostName github.com
            user git
            IdentityFile /Users/casiano/.ssh/chuchu
* El remote del repo debe ser cambiado de acuerdo:
            $ git remote -v
            origin git@github-nausica.com:nausicachijiro/testing.git
* Para que los commits funcionen con la personalidad alternativa 
  debo anunciarle a git mi nuevo `user` y `email`
            git config user.name nausicachijiro
            git config user.email nausica.chijiro@gmail.com
