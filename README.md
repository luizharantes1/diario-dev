# diario-dev
Meu diário de evolução como dev (commits, branches e anotações)
---

## 🗓️ Diário de Progresso

### Dia 0 — Preparação do Ambiente ✅
- VS Code e Git instalados  
- SSH conectado ao GitHub (teste: `Hi luizharantes1! ...`)  
- Extensões essenciais configuradas  

**Aprendido:** o que é SSH, diferença entre chave pública/privada e teste de autenticação.
### Dia 1 — Git na prática (branch → commit → PR → merge) ✅
- Criei e gerenciei branches com `git checkout -b`
- Fiz commits seguindo o padrão **Conventional Commits**
- Aprendi o fluxo completo de versionamento:
  `editar → commit → push → pull request → merge`
- Entendi como manter a `main` sempre atualizada com `git pull`

**Aprendido:** o Git é mais do que salvar versões — é colaboração, clareza e histórico bem documentado.
### Dia 2 a 4 — Git avançado, HTTP, REST e fundamentos Java ✅
- Praticado o fluxo completo de versionamento (branch → commit → PR → merge)
- Entendido o funcionamento do HTTP, REST e JSON
- Instaladas e testadas ferramentas de apoio: Postman e DBeaver
- Revisados tipos primitivos e estruturas de repetição (`for`, `while`)
- Criada a classe `ContaBancaria` aplicando os conceitos de POO

**Aprendido:** como o versionamento organiza o trabalho em equipe, como as APIs trocam dados via JSON, e como a lógica e POO estruturam o pensamento de um desenvolvedor.

## 🗓️ Dia 5 — Primeiros passos com Spring Boot 🚀

Hoje iniciei o projeto **gestao-tarefas**, meu primeiro projeto Java com **Spring Boot**.  
Aprendi a gerar o projeto pelo *Spring Initializr*, entender a estrutura do `pom.xml`, configurar o Maven e executar o servidor localmente.

Implementei meu primeiro **controller REST** com o endpoint `/hello`, retornando uma resposta JSON com:
- mensagem de status da API  
- autor do projeto  
- versão  
- timestamp  

Adicionei também o endpoint `/health` para monitorar o status da aplicação.

**Principais aprendizados:**
- Estrutura padrão de um projeto Spring Boot  
- Função do arquivo `pom.xml`  
- Uso de `@RestController` e `@GetMapping`  
- Personalização via `application.properties`  
- Execução com `./mvnw spring-boot:run`

**Status:** 🟢 Projeto rodando localmente em `http://localhost:8081`
