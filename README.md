# 📚 Desafio DIO — Aprendendo na Prática o Paradigma de Orientação a Objetos

<p align="center">
  <img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white"/>
  <img src="https://img.shields.io/badge/IntelliJ_IDEA-000000?style=for-the-badge&logo=intellij-idea&logoColor=white"/>
  <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white"/>
  <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"/>
  <img src="https://img.shields.io/badge/DIO-6A0DAD?style=for-the-badge&logo=data:image/png;base64,&logoColor=white"/>
</p>

---

## 💡 Sobre o Projeto

Este projeto foi desenvolvido como parte do desafio prático da plataforma **Digital Innovation One (DIO)**, com o objetivo de aplicar os **4 pilares da Programação Orientada a Objetos (POO)** em Java através de um sistema de Bootcamp.

O sistema simula o funcionamento de um Bootcamp, onde Devs se inscrevem, progridem nos conteúdos e acumulam pontos de XP.

---

## 🏗️ Estrutura do Projeto

```
src/
└── br/com/dio/desafio/dominio/
    ├── Conteudo.java     → Classe abstrata base
    ├── Curso.java        → Herda de Conteudo
    ├── Mentoria.java     → Herda de Conteudo
    ├── Bootcamp.java     → Gerencia conteúdos e devs
    ├── Dev.java          → Representa o desenvolvedor
    └── Main.java         → Classe principal (testes)
```

---

## 🧠 Os 4 Pilares da POO aplicados

### 🔹 Abstração
A classe `Conteudo` representa de forma abstrata qualquer conteúdo de um Bootcamp, seja um Curso ou uma Mentoria, sem se preocupar com os detalhes específicos de cada um.

### 🔹 Encapsulamento
Todos os atributos das classes são privados (`private`) e acessados apenas através de métodos `getters` e `setters`, protegendo os dados internos de cada objeto.

### 🔹 Herança
As classes `Curso` e `Mentoria` herdam da classe abstrata `Conteudo`, reutilizando seus atributos (`titulo`, `descricao`) e implementando o método `calcularXp()` de forma específica para cada uma.

### 🔹 Polimorfismo
O método `calcularXp()` é implementado de forma diferente em `Curso` e `Mentoria`:
- **Curso**: `XP_PADRAO * cargaHoraria`
- **Mentoria**: `XP_PADRAO + 20`

---

## ⚙️ Como Executar

### Pré-requisitos
- Java JDK 11 ou superior
- IntelliJ IDEA (ou outra IDE Java)
- Git

### Passos
```bash
# Clone o repositório
git clone https://github.com/Pedro-arauj0/POO-java.git

# Abra o projeto no IntelliJ IDEA
# Execute a classe Main.java
```

---

## 📊 Exemplo de Saída

```
Conteúdos Inscritos Camila: [Curso Java, Curso JS, Mentoria Java]
Conteúdos Concluídos Camila: [Curso Java, Curso JS]
XP: 120.0
-------
Conteúdos Inscritos João: [Curso Java, Curso JS, Mentoria Java]
Conteúdos Concluídos João: [Curso Java, Curso JS, Mentoria Java]
XP: 150.0
```

---

## 🛠️ Tecnologias Utilizadas

- **Java 21**
- **IntelliJ IDEA**
- **Git & GitHub**

---

## 👨‍💻 Autor

**Pedro Araújo**

[![GitHub](https://img.shields.io/badge/GitHub-Pedro--arauj0-181717?style=flat&logo=github)](https://github.com/Pedro-arauj0)

---

## 📝 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.
