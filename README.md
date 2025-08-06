# Sistema de Controle de Gastos Pessoais

## Descrição
Aplicação para registro e acompanhamento de despesas pessoais, permitindo adicionar gastos, categorizá-los e visualizar um resumo mensal.  
O **backend** é desenvolvido com **Spring Boot** e **H2 Database**, enquanto o **frontend** é feito com **HTML, CSS, JavaScript e Bootstrap**.

## Objetivos
- Registrar despesas com valor, categoria, data e descrição.
- Listar e editar despesas já cadastradas.
- Exibir resumo mensal por categoria com gráficos.
- (Opcional) Exportar relatório mensal em PDF.

## Tecnologias Utilizadas
### Backend
- **Linguagem:** Java
- **Framework:** Spring Boot
- **Banco de Dados:** H2 Database
- **ORM:** Spring Data JPA

### Frontend
- **HTML5** para estrutura
- **CSS3** para estilo
- **JavaScript** para interatividade
- **Bootstrap** para layout responsivo e componentes prontos

### Gerais
- **Controle de Versão:** Git e GitHub

## Estrutura do Projeto
```
backend/
├── src/main/java/...   # Código do backend
├── src/main/resources/ # Configurações (application.properties)
frontend/
├── index.html          # Página principal
├── css/                # Arquivos de estilo
├── js/                 # Scripts JavaScript
├── assets/             # Recursos estáticos
README.md               # Documentação do projeto
```

## Como Executar
### Backend
1. Clone este repositório:
   ```bash
   git clone https://github.com/seuusuario/projeto-controle-gastos.git
   ```
2. Configure o `application.properties` para utilizar o H2 Database:
   ```properties
   spring.datasource.url=jdbc:h2:mem:controle_gastos
   spring.datasource.driverClassName=org.h2.Driver
   spring.datasource.username=your_username
   spring.datasource.password=your_password
   spring.jpa.database-platform=org.hibernate.dialect.H2Dialect
   spring.h2.console.enabled=true
   ```
3. Execute o projeto Spring Boot.

### Frontend
1. Abra o arquivo `frontend/index.html` no navegador.

## Funcionalidades Esperadas
- Cadastro e listagem de despesas
- Resumo mensal por categoria
- Visualização de gráficos com JavaScript (ex: Chart.js)
- Exportação de relatório (opcional)

## Licença
Este projeto está licenciado sob a [MIT License](LICENSE).
