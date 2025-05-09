# Guia de Contribuição

Este documento descreve as diretrizes para contribuir com o projeto.

## Fluxo de Trabalho com Git

### Branches

- `main`: Branch principal, contém o código estável
- `develop`: Branch de desenvolvimento
- `feature/nome-da-feature`: Para novas funcionalidades
- `bugfix/nome-do-bug`: Para correções de bugs
- `docs/nome-da-documentacao`: Para atualizações de documentação

### Processo de Contribuição

1. Crie uma branch a partir de `develop`
2. Faça suas alterações
3. Submeta um Pull Request para `develop`
4. Aguarde a revisão de código
5. Após aprovação, seu código será mesclado

## Padrões de Codificação

[Descrever os padrões de codificação adotados pelo grupo]

## Processo de Review

- Todo código deve ser revisado por pelo menos um outro membro da equipe
- Utilize os comentários do Pull Request para discussões
- Siga a checklist de revisão (disponível em cada PR)

## Commits

Utilize mensagens de commit claras e descritivas seguindo o padrão:

```markdown
[tipo]: descrição curta

Descrição mais detalhada se necessário
```

Tipos:

- `feature`: Nova funcionalidade
- `fix`: Correção de bug
- `docs`: Alterações na documentação
- `style`: Formatação, ponto e vírgula, etc; sem alteração de código
- `refactor`: Refatoração de código
- `test`: Adição ou correção de testes
- `chore`: Atualizações de tarefas de build, configurações, etc

## Jira

Todas as tarefas devem estar associadas a um item no Jira.
Inclua o código da tarefa no início de cada mensagem de commit.
