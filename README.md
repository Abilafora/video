# 🌱 ReciclaConect

<div align="center">
  <img src="https://img.shields.io/badge/Java-21-orange?style=for-the-badge&logo=java" alt="Java 21">
  <img src="https://img.shields.io/badge/Spring%20Boot-3.5.7-brightgreen?style=for-the-badge&logo=spring" alt="Spring Boot">
  <img src="https://img.shields.io/badge/Maven-3.9+-blue?style=for-the-badge&logo=apache-maven" alt="Maven">
  <img src="https://img.shields.io/badge/H2-Database-blue?style=for-the-badge&logo=h2" alt="H2 Database">
  <img src="https://img.shields.io/badge/Status-Em%20Desenvolvimento-yellow?style=for-the-badge" alt="Status">
</div>

<br>

<p align="center">
  <strong>Plataforma que conecta catadores, cooperativas e empresas para fortalecer a cadeia de reciclagem no Brasil</strong>
</p>

---

## 📋 Sobre o Projeto

O **ReciclaConect** é um Projeto Integrador desenvolvido para o curso de **Tecnologia em Análise e Desenvolvimento de Sistemas**, com o objetivo de demonstrar a aplicação prática de conhecimentos em desenvolvimento full-stack, integrando front-end, back-end e banco de dados.

### 🎯 Problema Identificado

A cadeia de reciclagem no Brasil enfrenta desafios significativos:
- Dificuldade de conexão entre catadores e empresas recicladoras
- Falta de transparência nos preços dos materiais recicláveis
- Ausência de ferramentas digitais para facilitar negociações
- Baixa valorização do trabalho dos catadores

### 💡 Solução Proposta

Uma plataforma web que:
- **Conecta** catadores a empresas e cooperativas de reciclagem
- **Facilita** a negociação de materiais recicláveis
- **Mapeia** pontos de coleta e empresas próximas
- **Educa** sobre práticas sustentáveis de reciclagem
- **Valoriza** o trabalho dos profissionais da reciclagem

---

## ✨ Funcionalidades

### 👤 Para Catadores
- ✅ Cadastro completo com dados pessoais e localização
- 📍 Visualização de empresas e cooperativas próximas no mapa
- 💼 Acesso a oportunidades de venda de materiais
- 💬 Sistema de mensagens com empresas
- 📊 Dashboard com estatísticas e histórico
- 🎓 Área educativa sobre reciclagem

### 🏢 Para Empresas/Cooperativas
- ✅ Cadastro com informações da empresa
- 📢 Publicação de demandas por materiais recicláveis
- 👥 Busca e contato com catadores da região
- 📈 Gerenciamento de transações

### 🌐 Funcionalidades Gerais
- 🗺️ Mapa interativo com geolocalização
- 🔍 Sistema de busca avançada
- 🔔 Notificações em tempo real
- 📱 Interface responsiva (desktop, tablet e mobile)

---

## 🛠️ Tecnologias Utilizadas

### Back-end
- **Java 21** - Linguagem de programação
- **Spring Boot 3.5.7** - Framework principal
  - Spring Web - API REST
  - Spring Data JPA - Persistência de dados
  - Spring DevTools - Desenvolvimento
- **Maven** - Gerenciamento de dependências
- **Lombok** - Redução de código boilerplate
- **H2 Database** - Banco de dados em memória

### Front-end
- **HTML5** - Estrutura das páginas
- **CSS3** - Estilização e layout
  - Variáveis CSS (Custom Properties)
  - Flexbox e Grid Layout
  - Media Queries (Responsividade)
  - Animações e Transições
- **JavaScript (Vanilla)** - Interatividade
- **Thymeleaf** - Template engine
- **Font Awesome 6.4.0** - Ícones
- **Leaflet 1.9.4** - Mapas interativos

### Padrões e Arquitetura
- **MVC (Model-View-Controller)** - Padrão arquitetural
- **REST API** - Comunicação cliente-servidor
- **JPA/Hibernate** - ORM (Object-Relational Mapping)
- **Repository Pattern** - Acesso a dados

---

## 📁 Estrutura do Projeto

```
conect/
├── src/
│   ├── main/
│   │   ├── java/br/com/recicla/conect/
│   │   │   ├── ConectApplication.java          # Classe principal
│   │   │   ├── controller/
│   │   │   │   └── CadastroController.java     # Controlador de cadastros
│   │   │   ├── model/
│   │   │   │   └── Catador.java                # Entidade Catador
│   │   │   └── repository/
│   │   │       └── CatadorRepository.java      # Repositório JPA
│   │   │
│   │   └── resources/
│   │       ├── application.properties           # Configurações da aplicação
│   │       ├── static/
│   │       │   ├── css/
│   │       │   │   ├── style.css               # Estilos globais
│   │       │   │   ├── cadastro.css            # Estilos de cadastro
│   │       │   │   └── dashboard.css           # Estilos do dashboard
│   │       │   ├── js/
│   │       │   │   ├── main.js                 # Scripts globais
│   │       │   │   ├── cadastro-catador.js     # Lógica de cadastro
│   │       │   │   ├── cadastro-empresa.js     # Lógica de cadastro
│   │       │   │   ├── login.js                # Lógica de login
│   │       │   │   └── dashboard.js            # Lógica do dashboard
│   │       │   └── imagens/
│   │       │
│   │       └── templates/
│   │           ├── index.html                  # Página inicial
│   │           ├── login.html                  # Página de login
│   │           ├── cadastro-catador.html       # Cadastro de catador
│   │           ├── cadastro-empresa.html       # Cadastro de empresa
│   │           ├── dashboard-catador.html      # Dashboard do catador
│   │           └── mapa.html                   # Mapa interativo
│   │
│   └── test/
│       └── java/br/com/recicla/conect/
│           └── ConectApplicationTests.java     # Testes
│
├── pom.xml                                     # Dependências Maven
├── mvnw                                        # Maven Wrapper (Linux/Mac)
├── mvnw.cmd                                    # Maven Wrapper (Windows)
└── README.md                                   # Este arquivo
```

---

## 🚀 Como Executar o Projeto

### Pré-requisitos

- **Java 21** ou superior ([Download](https://www.oracle.com/java/technologies/downloads/))
- **Maven 3.9+** (ou utilizar o Maven Wrapper incluído)
- IDE recomendada: IntelliJ IDEA, Eclipse ou VS Code

### Passo a Passo

1. **Clone o repositório**
   ```bash
   git clone https://github.com/PriscilaOcchi/conect.git
   cd conect
   ```

2. **Execute o projeto com Maven**
   
   **Linux/Mac:**
   ```bash
   ./mvnw spring-boot:run
   ```
   
   **Windows:**
   ```cmd
   mvnw.cmd spring-boot:run
   ```
   
   **Ou com Maven instalado:**
   ```bash
   mvn spring-boot:run
   ```

3. **Acesse a aplicação**
   
   Abra seu navegador em: [http://localhost:8080](http://localhost:8080)

4. **Acesse o console H2 (opcional)**
   
   Para visualizar o banco de dados: [http://localhost:8080/h2-console](http://localhost:8080/h2-console)
   
   Configurações de conexão:
   - **JDBC URL:** `jdbc:h2:mem:testdb`
   - **Username:** `sa`
   - **Password:** _(deixe em branco)_

---

### Página Inicial
Apresentação da plataforma com informações sobre como funciona, benefícios e depoimentos.

### Dashboard do Catador
- Estatísticas de transações e receitas
- Oportunidades de venda disponíveis
- Mapa com empresas próximas
- Histórico de atividades

### Sistema de Cadastro
Formulários intuitivos para cadastro de catadores e empresas com validação de campos.

### Mapa Interativo
Visualização geolocalizada de empresas, cooperativas e pontos de coleta.

---

## 🎨 Identidade Visual

A plataforma utiliza uma paleta de cores que transmite sustentabilidade e confiança:

- **Laranja Principal** (`#FF6B35`) - Representa energia e ação
- **Verde Secundário** (`#2ECC71`) - Sustentabilidade
- **Azul Secundário** (`#3498DB`) - Confiança
- **Tons Neutros** (cinzas) - Clareza e profissionalismo

---

## 🔐 Segurança e Validações

### Validações Implementadas
- ✅ Validação de CPF no front-end e back-end
- ✅ Validação de e-mail com regex
- ✅ Validação de CEP (formato brasileiro)
- ✅ Validação de telefone
- ✅ Campos obrigatórios em formulários
- ✅ Sanitização de inputs

### Banco de Dados
- Banco H2 em memória para desenvolvimento
- Hibernate DDL em modo `update`
- SQL formatado para debugging

---

## 📚 Aprendizados e Conceitos Aplicados

### Programação Orientada a Objetos
- Encapsulamento (uso de Lombok)
- Herança e Polimorfismo
- Injeção de Dependências

### Desenvolvimento Web
- Arquitetura MVC
- API REST
- CRUD completo
- Template Engines (Thymeleaf)
- SPA (Single Page Application) parcial

### Banco de Dados
- JPA/Hibernate
- Relacionamento entre entidades
- Queries personalizadas
- Transações

### Front-end
- Design Responsivo
- UX/UI
- Acessibilidade
- Performance

---

## 🔄 Funcionalidades Futuras

- [ ] Autenticação e autorização (Spring Security)
- [ ] Sistema de chat em tempo real (WebSocket)
- [ ] Integração com APIs de geolocalização
- [ ] Sistema de avaliações e reviews
- [ ] Notificações por e-mail
- [ ] Exportação de relatórios (PDF/Excel)
- [ ] Painel administrativo
- [ ] API pública para integrações
- [ ] Migração para banco PostgreSQL/MySQL
- [ ] Deploy em nuvem (AWS/Azure/Heroku)

---

## 🤝 Contribuições

Este é um projeto acadêmico, mas sugestões e feedbacks são bem-vindos!

### Como Contribuir
1. Fork o projeto
2. Crie uma branch para sua feature (`git checkout -b feature/MinhaFeature`)
3. Commit suas mudanças (`git commit -m 'Adiciona MinhaFeature'`)
4. Push para a branch (`git push origin feature/MinhaFeature`)
5. Abra um Pull Request

---

## 📄 Licença

Este projeto foi desenvolvido para fins educacionais como parte do Projeto Integrador do curso de Tecnologia em Análise e Desenvolvimento de Sistemas.

---

## 👨‍💻 Autor

**Priscila Occhi**

- GitHub: [@PriscilaOcchi](https://github.com/PriscilaOcchi)
- LinkedIn: [Seu LinkedIn](https://linkedin.com/in/priscila-occhi)

  **Abiqueila de Souza Silva**
- GitHub: [@PriscilaOcchi]((https://github.com/Abilafora))
- LinkedIn: [Seu LinkedIn](www.linkedin.com/in/abiqueila-souza )
---

## 🎓 Instituição de Ensino

**[Nome da Instituição]**  
Curso: Tecnologia em Análise e Desenvolvimento de Sistemas  
Projeto Integrador - [Ano/Semestre]


---

<div align="center">
  <p>Desenvolvido com 💚 para conectar e fortalecer a cadeia de reciclagem no Brasil</p>
  <p>⭐ Se este projeto foi útil para você, considere dar uma estrela!</p>
</div>
