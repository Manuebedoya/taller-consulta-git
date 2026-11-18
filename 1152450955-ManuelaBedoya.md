1. **¿Qué es Git y qué problema resuelve en el desarrollo de software?**
1. ¿Qué es Git y qué problema resuelve en el desarrollo de software?
¿Qué es?: Git es un Sistema de Control de Versiones Distribuido de código abierto, diseñado originalmente por Linus Torvalds. Permite registrar y rastrear cada cambio realizado en el código fuente de un proyecto a lo largo del tiempo.

Problema que resuelve: Resuelve el caos del desarrollo de software tradicional (como tener carpetas llamadas proyecto_final_v1, proyecto_final_definitivo_ahora_si.zip). Git evita la pérdida de código permitiendo volver atrás en el tiempo a cualquier estado anterior funcional, soluciona los conflictos cuando varias personas editan el mismo archivo al mismo tiempo, y mantiene un historial exacto de quién hizo qué y por qué.

2. **Diferencias clave entre Git y GitHub.** (Expliquen por qué no son lo mismo).
2. Diferencias clave entre Git y GitHub (¿Por qué no son lo mismo?)
Aunque se usan juntos, son cosas totalmente distintas:

Git es la herramienta local (el software instalado en tu computador) que gestiona el control de versiones sin necesidad de internet.

GitHub es una plataforma en la nube (un servicio de alojamiento web) que utiliza Git para almacenar repositorios de forma remota, facilitando la colaboración en equipo, la revisión de código (Pull Requests) y la gestión de proyectos.

En resumen: Git es el motor que registra los cambios en tu PC, y GitHub es el garaje en la nube donde guardas y compartes el carro con tus compañeros.

3. **¿Qué es una nube de repositorios?** Expliquen este concepto y mencionen al menos tres alternativas diferentes en el mercado (por ejemplo, además de GitHub, ¿qué otras plataformas existen?).
3. ¿Qué es una nube de repositorios y tres alternativas en el mercado?
Concepto: Es un servicio de alojamiento web que almacena repositorios de Git de forma centralizada en la nube. Funciona como respaldo seguro y como un espacio de trabajo colaborativo donde los desarrolladores pueden subir sus proyectos, gestionar incidencias (issues) y coordinar el flujo de trabajo en equipo.

Alternativas a GitHub:

GitLab: Una plataforma muy potente de DevOps que incluye integración continua (CI/CD) avanzada y herramientas completas de gestión de ciclo de vida del software.

Bitbucket: Plataforma de alojamiento de Atlassian, muy popular por su integración fluida con herramientas como Jira y Trello.

Azure DevOps (anteriormente Visual Studio Team Services): Plataforma de Microsoft orientada a empresas que integra repositorios Git con tableros Kanban, pipelines de despliegue y gestión ágil.

4. **Glosario básico:** Definan con sus propias palabras, de forma clara y **agregando un ejemplo práctico para cada uno**, los siguientes conceptos fundamentales de Git:
   * *Commit*
   * *Branch* (Rama)
   * *Merge* (Fusión)
   * *Pull* y *Push*
   * *Pull Request (PR)*
   * *Clone* (Clonar)
   * *Upstream* (y su diferencia con *Origin*)
   4. Glosario básico (Definición y ejemplo práctico)
Commit:

Definición: Es una "fotografía" o instantánea oficial del estado de los archivos en tu proyecto en un momento dado. Guarda los cambios realizados con un mensaje descriptivo y un identificador único (SHA).

Ejemplo práctico: Después de escribir el código para el formulario de login, ejecutas git commit -m "feat: add user login validation form" para congelar ese avance en el historial.

Branch (Rama):

Definición: Es una línea de desarrollo independiente que te permite apartarte de la línea principal (como main) para experimentar, agregar funciones o corregir errores sin afectar el código estable.

Ejemplo práctico: Creas una rama llamada feature/carrito-compras para programar la pasarela de pagos de una tienda virtual mientras la rama principal sigue intacta.

Merge (Fusión):

Definición: Es el proceso de unir el historial y los cambios de una rama con otra (por ejemplo, integrar una rama secundaria de vuelta a la principal).

Ejemplo práctico: Una vez terminada y probada la rama del carrito de compras, haces un merge para fusionarla dentro de la rama develop o main.

Pull y Push:

Definición: Push es enviar tus commits locales hacia el repositorio remoto (en la nube). Pull es descargar los cambios más recientes del repositorio remoto hacia tu equipo local.

Ejemplo práctico: Haces git push origin main para subir tus últimas tareas a GitHub, y tus compañeros hacen git pull para actualizar sus computadores con tu código.

Pull Request (PR):

Definición: Es una solicitud formal en plataformas como GitHub para avisar a tu equipo que has terminado una rama y propones fusionar (merge) esos cambios en otra rama (como main o develop). Permite revisar el código antes de integrarlo.

Ejemplo práctico: Abres un Pull Request en GitHub titulado "Añadir módulo de autenticación" para que tu profe o equipo revise el código antes de aceptarlo en el proyecto oficial.

Clone (Clonar):

Definición: Es la acción de descargar por primera vez una copia exacta de un repositorio remoto completo (con todo su historial y ramas) desde la nube hacia tu computador local.

Ejemplo práctico: Al iniciar un proyecto en equipo, ejecutas git clone [https://github.com/usuario/proyecto.git](https://github.com/usuario/proyecto.git) para tener el código base listo en tu VS Code.

Upstream y su diferencia con Origin:

Definición: origin es el nombre por defecto que le da Git al repositorio remoto de donde clonaste originalmente (tu propia copia o el repositorio principal). upstream se refiere habitualmente al repositorio original o matriz (por ejemplo, el del profesor o la empresa original) desde el cual hiciste un fork, y se usa para sincronizar actualizaciones.

Ejemplo práctico: Si clonas tu propio repositorio en GitHub, origin apunta a tu cuenta. Si trabajas en un proyecto open-source haciendo un fork, configuras upstream apuntando al repositorio del dueño original para jalar sus últimas actualizaciones con git pull upstream main.