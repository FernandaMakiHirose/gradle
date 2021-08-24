# Projetos Java com Gradle
Instalar o Gradle na sua máquina (em um projeto que usa o Gradle):
>./gradlew

Versão do Gradlew:
>./gradlew --version

Tasks:
>./gradlew tasks

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
