# dsmeta

Ferramentas
DÚVIDAS: veja o canal #duvidas-frequentes no Discord do evento

Nodejs 16 e Yarn (vídeo: https://youtu.be/x5tgFTS-CYA )
STS (vídeo: https://youtu.be/TGQ0K9QsX88 )
VS Code
IntelliCode
ESLint
JSX HTML <tags/>
Passo: criar projeto ReactJS
DevSuperior no Instagram

yarn create vite frontend --template react-ts
DÚVIDAS: veja o canal #duvidas-frequentes no Discord do evento

Passo: criar projeto Spring Boot
Criar projeto Spring Boot no Spring Initializr com as seguintes dependências:

Web
JPA
H2
Security
Ajuste no arquivo pom.xml:

<plugin>
	<groupId>org.apache.maven.plugins</groupId>
	<artifactId>maven-resources-plugin</artifactId>
	<version>3.1.0</version><!--$NO-MVN-MAN-VER$ -->
</plugin>
Botão direito no projeto -> Maven -> Update project (force update)
Passo: salvar primeira versão no Github
DÚVIDAS: veja o canal #duvidas-frequentes no Discord do evento

git init

git add .

git commit -m "Project created"

git branch -M main

git remote add origin git@github.com:seuusuario/seurepositorio.git

git push -u origin main
Passo: "limpar" o projeto ReactJS
Vamos pegar o CSS que fizemos nas aulas de preparação:

https://github.com/acenelio/dsmeta-css

COMMIT: Project clean
Passo: Primeiro componente
Projeto HTML/CSS: https://github.com/acenelio/dsmeta-css

COMMIT: First component
Passo: Outros componentes
COMMIT: Other components
Passo: Datepicker
Documentação: https://github.com/Hacker0x01/react-datepicker

yarn add react-datepicker@4.8.0 @types/react-datepicker@4.4.2
import DatePicker from "react-datepicker";
import "react-datepicker/dist/react-datepicker.css";
<DatePicker
    selected={new Date()}
    onChange={(date: Date) => {}}
    className="dsmeta-form-control"
    dateFormat="dd/MM/yyyy"
/>
COMMIT: Datepicker
Passo: React Hook useState para manter estado das datas
Macete para criar uma data de X dias atrás:

const date = new Date(new Date().setDate(new Date().getDate() - 365));
COMMIT: useState