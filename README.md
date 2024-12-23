# SkillHub

**SkillHub** es un sistema de gestión de aprendizaje (LMS) diseñado específicamente para academias e instituciones educativas. La plataforma facilita la creación de cursos, el seguimiento del progreso de los estudiantes y la evaluación de su desempeño. Construido con **Spring Boot**, **Thymeleaf** y **MySQL**, SkillHub es ideal para gestionar el aprendizaje de manera efectiva en entornos académicos.

## Características

- **Gestión de Cursos**: Crear, editar y organizar cursos de manera intuitiva.
- **Lecciones y Material de Apoyo**: Añadir lecciones con contenido multimedia como videos, documentos PDF y presentaciones.
- **Roles y Permisos**: Acceso diferenciado para administradores, instructores y estudiantes.
- **Evaluaciones y Exámenes**: Cuestionarios automáticos y evaluaciones personalizables.
- **Seguimiento de Progreso**: Visualización del avance de los estudiantes en cada curso.
- **Reportes y Análisis**: Generación de estadísticas detalladas sobre el rendimiento y la finalización de cursos.
- **Certificación**: Certificados de finalización para los estudiantes que completen sus cursos.

## Tecnologías Utilizadas

- **Backend**: Java, Spring Boot
- **Frontend**: Thymeleaf, HTML, CSS
- **Base de Datos**: MySQL
- **Gestión de Dependencias**: Maven
- **Otros**: Git para el control de versiones

## Instalación

Sigue estos pasos para instalar y ejecutar SkillHub en tu entorno local.

### Prerrequisitos

- **Java 11** o superior
- **Maven**
- **MySQL** (instalado y en ejecución)

### Configuración

1. **Clonar el Repositorio**:
   ```bash
   git clone https://github.com/lucasbarrientosmu/SkillHub.git
   cd SkillHub
   ```

2. **Configuración de la Base de Datos**:
   - Crea una base de datos en MySQL:
     ```sql
     CREATE DATABASE skillhub_db;
     ```
   - Configura las credenciales de la base de datos en el archivo `src/main/resources/application.properties`:
     ```properties
     spring.datasource.url=jdbc:mysql://localhost:3306/skillhub_db
     spring.datasource.username=your_mysql_username
     spring.datasource.password=your_mysql_password
     ```

3. **Compilar el Proyecto**:
   ```bash
   mvn clean install
   ```

4. **Ejecutar la Aplicación**:
   ```bash
   mvn spring-boot:run
   ```

5. **Acceder a la Aplicación**:
   - Abre un navegador web y navega a `http://localhost:8080`.

## Uso

### Roles de Usuario

- **Administrador**:
  - Gestiona usuarios, cursos y el sistema en general.
  - Puede ver reportes detallados de rendimiento y actividad de los estudiantes.

- **Profesor/Instructores**:
  - Crea y gestiona sus propios cursos, lecciones y evaluaciones.
  - Puede ver el progreso de los estudiantes inscritos en sus cursos.

- **Estudiantes**:
  - Se inscriben en cursos, completan lecciones y realizan evaluaciones.
  - Reciben un certificado al finalizar un curso.

### Funcionalidades

Una vez que accedes a la aplicación, puedes navegar por las funcionalidades dependiendo de tu rol:

- **Administrador**: Puede acceder al panel de administración para supervisar usuarios y cursos.
- **Profesor**: Gestiona sus cursos, lecciones y evaluaciones, y realiza el seguimiento de los estudiantes.
- **Estudiante**: Visualiza los cursos disponibles, completa lecciones y participa en evaluaciones.

## Contribución

Las contribuciones son bienvenidas. Si deseas colaborar en el proyecto, sigue estos pasos:

1. Haz un fork del repositorio.
2. Crea una rama para tu nueva función (`git checkout -b feature/nueva-funcion`).
3. Realiza tus cambios y haz commits (`git commit -m 'Añadir nueva función'`).
4. Sube tu rama (`git push origin feature/nueva-funcion`).
5. Abre un Pull Request.

## Licencia

Este proyecto está bajo la **Proprietary License by Lucas Barrientos Muñoz**. Consulta el archivo [LICENSE](./LICENSE) para más detalles.