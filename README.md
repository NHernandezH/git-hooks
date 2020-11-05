# git-hooks
Creacion de hooks para automatizar tareas de integracion y despliege

1.- pre-receive
este script se ejecuta una vez realizado un push al servidor remoto, en este caso el scrip validara que se hayan realizado cambios en las subcarpetas definidas (que en este caso son proyectos maven) y ejecutara las pruebas unitarias, en caso de que llegase a fallar alguna prueba, se finalizara la tarea y se rechazara el push hasta que todas las pruebas sean exitosas
