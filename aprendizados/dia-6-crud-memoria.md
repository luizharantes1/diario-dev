# 🗓️ Dia 6 — CRUD de Tarefas em Memória (Java + Spring Boot)

Hoje implementei o primeiro CRUD completo do projeto **Gestão de Tarefas**.  
Aprendi a estruturar o código em camadas (`domain`, `service` e `web`), criar rotas REST e trabalhar com respostas HTTP padronizadas.

---

## 🔧 Atividades concluídas
- Criação da entidade **`Task`** (`id`, `title`, `done`, `createdAt`)
- Implementação da camada **`TaskService`** para gerenciar as tarefas em memória
- Criação do **`TaskController`** com as rotas:
  - `POST /tasks` → cria nova tarefa  
  - `GET /tasks` → lista todas  
  - `GET /tasks/{id}` → busca por ID  
  - `PATCH /tasks/{id}/done` → marca como concluída  
  - `DELETE /tasks/{id}` → exclui tarefa  
- Criação do DTO **`TaskRequest`** para entrada de dados
- Testes realizados com sucesso no **Postman**
- Organização da **Collection** com todas as rotas
- Integração completa com o **GitHub** (branch → commit → PR → merge)

---

## ⚠️ Erros e soluções

**1.** *Erro:* `fatal: not a git repository`  
> **Causa:** projeto gerado a partir de arquivo ZIP, sem a pasta `.git`.  
> **Solução:** inicializei o Git local com `git init` e conectei ao repositório remoto.

**2.** *Erro:* “Compare & pull request” não aparecia.  
> **Causa:** branch criada depois do commit, sem diferenças em relação à main.  
> **Solução:** criei uma nova branch (`feat/tasks-crud-memory-v2`) e fiz commit válido. O PR foi aberto normalmente.

**3.** *Erro:* esquecimento de deletar a branch após merge.  
> **Solução:** removi manualmente com  
> `git push origin --delete feat/tasks-crud-memory-v2` e `git branch -d feat/tasks-crud-memory-v2`.

---

## 💡 Aprendizados principais
- Separação de responsabilidades entre **Domain / Service / Controller**
- Padrões REST e status HTTP (200, 201, 204, 400, 404)
- Uso de **DTOs (`record`)** para entrada de dados
- Git Workflow completo: branch → commit → push → PR → merge → delete
- Como diagnosticar e resolver erros de repositório remoto
- Organização de testes com Postman (Collections)

---

## 🟢 Status final
CRUD funcional e testado.  
Repositório atualizado com sucesso (`gestao-tarefas`).  
Histórico documentado no `diario-dev`.

---

### 📅 Próximo passo
**Dia 7 — Validações e tratamento global de erros**
- Adicionar Bean Validation (`@NotBlank`, `@Size`)
- Criar um `GlobalExceptionHandler` para respostas de erro em JSON
- Continuar boas práticas REST antes de conectar com PostgreSQL.
