# Projetos Java com Gradle
## aula1 - 01-testing-gradlew
Instalar o Gradle na sua máquina (em um projeto que usa o Gradle):
>./gradlew

Versão do Gradlew:
>./gradlew --version

Tasks:
>./gradlew tasks

## aula2 - 01-buildscript
Rodar o programa:
>gradle run

Rodar o programa sem os logs:
>gradle run -q

Build:
>gradle build

## aula2 - 02-application-plugin
Vai mostrar as tasks do plugin:
>./gradlew tasks

### aula2 - 03-java-project
Iniciando o projeto (responder as perguntas):
>gradle init

Testes:
>gradle test

## aula2 - 04-multi-modules
Rodar o programa:
>gradle run

1- Escolha o `1` ou `2`

## aula 3 01-first-tasks
Executar a primeira task:
>gradle myFirstTask

Executar a segunda task:
>gradle mySecondTask

Executar todas as tasks:
>gradle tasks

Realiza todo esse processo de uma vez só:
>gradle generateRelease

## aula 3 02-tasks-dependencies
Para executar uma task: `task` + `nome da task`

## aula 3 03-task-types
Deletar a pasta `build`:
>gradle deleteBuild

Gera a pasta `build`:
>gradle build

Cria a pasta `Release`
>gradle copyBuild

Cria uma pasta em zip:
>gradle zipReleaseToTestTeam

## Instalação do Gradle 
1) Faça o [download](https://gradle.org/install/)
2) Siga o passo a passo da configuração das variáveis de ambiente [aqui](https://gist.github.com/DenysNunes/c9e33b3422ef83ba362b)

## O que é o Gradle?
- Sistema de automação de compilação e de builds
- Ele pega todos os arquivos do projeto e cria um JAR ou um apk (ANDROID)
- Resumindo ele faz a build do seu projeto e você pode definir como será essa build
- Sistemas similares: Maven e Ant

## O que o Gradle faz?
- Fazer diversas tarefas antes, durante e após as builds
- Rodar os unit tests do projeto
- Colocar o JAR ou a APK em uma pasta diferenta da padrão
- Gestão de dependências de um projeto
- Fazer builds de múltiplos módulos (alguns chamam de multi projetos) e variações de compilação
- Gerar documentação (Javadoc)
- Assinar apks e aab no Android
- Tem um único comando

## Características
- Os arquivos de build do Gradle são scripts escritos na linguagem Groovy
- Ele é baseado em tasks
- Tem um forte sistemas de plugins
- Open source

## Gradlew
- Permite usar todas as funcionalidades do Gradle sem precisar instalá-lo
- "Envelopa" toda a configuração do Gradle
- Outros devs podem trabalhar no projeto com a mesma configuração de gradle
- Muito utilizado com times grandes

## BuildScript
- O arquivo `build.gradle` é chamado de BuildScript
- Ele define toda a configuração da build
- O `build.gradle` é escrito utilizando uma DSL (domain specific language)
- Que pode ser o Groovy ou em Kotlin
- Concentra as tarefas que serão possíveis serem executadas com o Gradle
- Quando executada uma task, o Gradle vai executar o que foi programado no arquivo `build.gradle`
- Todos os comandos no arquivo `build.gradle` vão sempre ser executados

## Plugins
- Facilita a criação de um executável de uma aplicação JVM
- Utiliza implicitamente os plugins "Java" e "distribution"
- Disponibiliza diversas tasks para projetos Java

## Multi Módulos
- Também chamado de "Multi Projetos"
- É possível adicionar submódulos dentro da sua aplicação Java
- O Gradle deve ser configurado para suportar os submódulos

## Por que usar?
- Organização do código em projetos muito grandes
- Possibilidade de dividir o time em subprojetos quase independentes
- Facilidade da adição de novos módulos ao projeto

## Criando tasks
- O Gradle te permite criar suas próprias tasks utilizando a DSL
- Muito útil quando nenhuma tasks de nenhum plugin satisfaz o que você quer fazer
- É possível criar tasks que utilizam outras tasks já existentes em plugins

## Task dependente
- Quando a execução de uma task depende da finalização de outra
- Para definir a ordem de execução das suas tasks
- 3 principais configurações para definir dependências: dependsOn (a task só será inicializada quando a task que ela depende ser executada primeiro), finalizedBy (após executar uma task vai chamar outra task), mustRunAfter (a task precisa ser executada depois de uma outra task)

## Task Types
- Auxilia no desenvolvimento de tasks complexas
- Tasks pré configuradas, como para copiar arquivos de uma pasta para outra ou gerar um zip
- Elas são diferenciadas pelo tipo, como "task do tipo copy/zip" 

## Próximos passos
- Dê uma olhada na documentação do Gradle
- Estudo os tipos possíveis de task types
- Utilize em conjunto com o Eclipse
- Pratique bastante

## Quiz
Qual a principal razão para utilizar o Gradlew (Gradle Wrapper)? 
Para que todos os desenvolvedores do time utilizem a mesma configuração do Gradle 

Para que serve o BuildScript?
Ele define a configuração do Gradle

Por que você usaria um plugin no Gradle?
Adicionar novos padrões da DSL ao Gradle

Qual das seguintes tasks apenas o plugin de Application adiciona ao Gradle?
Run

É uma definição de Gradle:
É um sistema de automação de compilação

Qual das alternativas abaixo NÃO é uma vantagem quando fazemos a gestão de dependências com o Gradle?
Utilizando a gestão de dependências você é capaz de fazer a configuração do seu Gradle corretamente

Por que você usaria Task Types?
Para desenvolver tasks com ações comuns já pré configuradas pelo Gradle, como gerar um arquivo zip

## Sobre a Autora
Oi, eu sou a Fernanda! Estou aqui para contribuir com meu conhecimento e espero poder ajudar no desenvolvimento profissional de cada um de vocês.

[![Linkedin Badge](https://img.shields.io/badge/-Fernanda_Maki_Hirose-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/fernanda-maki-hirose-801117208/)](https://www.linkedin.com/in/fernanda-maki-hirose-801117208/)  [![Gmail Badge](https://img.shields.io/badge/-femahi2020@gmail.com-c14438?style=flat-square&logo=Gmail&logoColor=white&link=mailto:femahi2020@gmail.com)](mailto:femahi2020@gmail.com)
