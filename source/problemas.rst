================
Problemas comuns
================

1. Como editar um commit anterior **antes** de fazer push?

.. code:: bash

        $ git commit --amend

2. Como editar um commit anterior **depois** de fazer push?

Basta fazer o mesmo comando anterior, que gerará uma modificação no último
commit, porém no remote não haverá nenhuma alteração. Para sincronizar o
remote com o local, basta fazer um push forçado:

.. code:: bash

        $ git push --force

Nota: Não é recomendado fazer isso em repositórios públicos, pois isso pode causar
confusão para os outros desenvolvedores. Se você fez um push errado, o ideal
é fazer um revert do commit e depois fazer um novo commit com as alterações
corretas.
