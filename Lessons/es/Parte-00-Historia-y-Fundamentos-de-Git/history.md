# Historia y Fundamentos de Git

# Introducción

Git es un sistema de control de versiones distribuido creado por Linus Torvalds en 2005. Git representa la historia de una manera fundamentalmente diferente a los sistemas de control de versiones centralizados (CVCS) como Team Foundation Version Control, Perforce o Subversion. Los sistemas centralizados almacenan una historia separada para cada archivo en un repositorio. Git almacena la historia como un gráfico de instantáneas de todo el repositorio. Estas instantáneas, llamadas commits en Git, pueden tener múltiples padres, creando una historia que parece un gráfico en lugar de una línea recta. Esta diferencia en la historia es extremadamente importante y es la razón principal por la cual los usuarios familiarizados con CVCS encuentran confuso a Git.

Es importante aprender Git hoy en día porque es ampliamente utilizado por desarrolladores y empresas en todo el mundo. Es una herramienta esencial para gestionar cambios de código y colaborar con otros desarrolladores en proyectos. Git permite a los desarrolladores trabajar en código de manera independiente y luego fusionar sus cambios cuando estén listos.

## ¿Quién creó Git?

Git fue creado originalmente por Linus Torvalds en 2005 para el desarrollo del kernel de Linux. Desde entonces, otros desarrolladores del kernel han contribuido a su desarrollo inicial. Junio Hamano ha sido el mantenedor principal desde 2005.

## La Razón por la cual se creó Git

El equipo original ya no podía utilizar BitKeeper, un sistema de control de versiones anterior, después de perder su licencia gratuita para usarlo. En ese momento, ningún otro Sistema de Gestión de Control de Origen (SCM) cumplía con sus requisitos específicos para un sistema distribuido. Algunos de los objetivos del nuevo sistema eran la velocidad, un diseño simple, un sólido soporte para el desarrollo no lineal (miles de ramas paralelas), completamente distribuido y capaz de manejar proyectos grandes como el kernel de Linux de manera eficiente (velocidad y tamaño de datos).

## Alternativas a Git

Existen varias alternativas a Git, como Subversion (SVN), Mercurial (Hg) y Perforce.

Subversion es un sistema de control de versiones centralizado similar a CVS. A menudo se utiliza en entornos empresariales porque es fácil de usar y se integra bien con otras herramientas.

Mercurial es un sistema de control de versiones distribuido similar a Git. A menudo se utiliza en proyectos más pequeños porque es más fácil de aprender que Git.

Perforce es un sistema de control de versiones centralizado que se utiliza con frecuencia en entornos empresariales. Tiene un buen soporte para archivos grandes y archivos binarios.

Cada uno de estos sistemas tiene sus propias fortalezas y debilidades, y la elección de cuál usar depende de las necesidades específicas del proyecto. Git se utiliza ampliamente por desarrolladores y empresas en todo el mundo porque es una herramienta esencial para gestionar cambios de código y colaborar con otros desarrolladores en proyectos. Git permite a los desarrolladores trabajar de manera independiente en el código y luego fusionar sus cambios cuando estén listos.

## Dónde almacenar tus repositorios de forma gratuita

Existen varios lugares gratuitos en Internet donde puedes almacenar tus repositorios Git. Aquí tienes algunos de los más populares:

- GitHub
- GitLab
- Bitbucket
- SourceForge

Cada uno de estos servicios tiene sus propias fortalezas y debilidades, y la elección de cuál usar depende de las necesidades específicas del proyecto. GitHub es el servicio más popular y es ampliamente utilizado por desarrolladores y empresas de todo el mundo. Ofrece repositorios públicos ilimitados y un número limitado de repositorios privados de forma gratuita.

GitLab es otro servicio popular que ofrece repositorios privados ilimitados de forma gratuita. Bitbucket se utiliza a menudo en equipos pequeños porque ofrece repositorios privados ilimitados de forma gratuita para hasta cinco usuarios. SourceForge es un servicio que ha existido durante mucho tiempo y se utiliza con frecuencia para proyectos de código abierto.