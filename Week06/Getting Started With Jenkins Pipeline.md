## [Getting Started With Jenkins Pipeline](https://jenkins.io/doc/book/pipeline/getting-started/)

### Introduction to Jenkins Pipeline

- Jenkins Pipeline is a suite of plugins that supports implementing and integrating continuous delivery pipelines into Jenkins.
- It provides tools for modeling delivery pipelines "as code" using the Pipeline DSL.
- Two DSLs available: Declarative and Scripted Pipeline.

### Prerequisites

- Jenkins 2.x or later is required (older versions may work but are not recommended).
- Pipeline plugin should be installed (included in the "suggested plugins").

### Defining a Pipeline

- Three ways to define a Pipeline:
  1. Through Blue Ocean: Set up a Pipeline project in Blue Ocean and use the graphical editor to create and commit the Jenkinsfile.
  2. Through the classic UI: Enter a basic Pipeline directly in Jenkins using the classic UI.
  3. In SCM: Write a Jenkinsfile manually and commit it to your project's source control repository.

### Writing a Pipeline Script in Jenkins

#### Through Blue Ocean

- Blue Ocean UI helps set up a Pipeline project and automatically creates the Jenkinsfile using the graphical editor.
- Changes made in the Pipeline editor are saved and committed to source control.

#### Through the classic UI

- Create a basic Pipeline using the Jenkins classic UI:
  1. Access the "New Item" option in the Jenkins home page.
  2. Enter the project name and select "Pipeline".
  3. Configure the Pipeline section and enter the Pipeline code in the Script text area.
  4. Save the configuration and run the Pipeline.

#### In SCM

- Configure the Pipeline project to use a Jenkinsfile from source control:
  1. Access the Pipeline configuration page.
  2. Choose the Pipeline script from SCM option.
  3. Select the source control system and complete the required fields.
  4. Specify the location of the Jenkinsfile in the Script Path field.
  5. Trigger a new build when the repository is updated.

### Built-in Documentation

- Jenkins Pipeline includes built-in documentation for reference and guidance during Pipeline development.
- Documentation is available globally at ${YOUR_JENKINS_URL}/pipeline-syntax and linked as Pipeline Syntax in the side-bar.
- Snippet Generator utility helps generate code snippets for individual steps and provides online help for Pipeline steps.
- Global Variable Reference provides documentation for variables provided by Pipeline or plugins available for Pipelines.
- Declarative Directive Generator helps generate configuration for Declarative directives used in a Declarative Pipeline.

### Further Reading

- Jenkins Pipeline offers more advanced features and possibilities.
- The next section, "The Jenkinsfile," discusses additional Pipeline steps and real-world implementation patterns.