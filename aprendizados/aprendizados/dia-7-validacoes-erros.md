✅ S1 · Dia 7 — Validações e Tratamento Global de Erros
Atividades concluídas

✅ Adicionado spring-boot-starter-validation ao pom.xml

✅ Atualizado o DTO TaskRequest com @NotBlank e @Size

✅ Aplicado @Valid no TaskController

✅ Criado o GlobalExceptionHandler para retornar erros padronizados em JSON

✅ Testes realizados no Postman (casos válidos e inválidos)

✅ Commit, PR e merge no GitHub

✅ “Descanso ativo”: assistido vídeo sobre Bean Validation no Spring Boot (Galego Dev) e anotações feitas

Erros enfrentados e soluções

❌ Porta 8081 já em uso → ✔ identificado com lsof e liberado com kill

❌ Variação na mensagem de erro (@NotBlank x @Size) → ✔ entendido que é comportamento normal, sem necessidade de ajuste

Aprendizados principais

💡 Bean Validation e suas anotações (@NotBlank, @Size)
💡 Tratamento global de exceções com @ControllerAdvice
💡 Respostas HTTP 400 padronizadas em JSON
💡 Diagnóstico de erros reais no ambiente de desenvolvimento
💡 Equilíbrio entre estudo prático e revisão leve (descanso ativo)

Status: 🟢 Concluído