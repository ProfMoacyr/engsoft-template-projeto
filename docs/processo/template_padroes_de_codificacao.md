# Padrões de Codificação

Este documento define os padrões de codificação a serem seguidos por todos os membros da equipe durante o desenvolvimento do projeto.

## 1. Nomenclatura

### 1.1 Classes e Interfaces

- Nomes de classes e interfaces devem ser substantivos
- Usar PascalCase (ex: `CalculadoraDeImpostos`, `PessoaFisica`)
- Nomes de interfaces podem começar com "I" (ex: `IRepositorio`, `IServico`)

### 1.2 Métodos

- Nomes de métodos devem ser verbos ou frases verbais
- Usar camelCase (ex: `calcularTotal()`, `buscarPorId()`)
- Métodos de teste devem seguir o padrão: `deveComportamento_quandoEstado()`

### 1.3 Variáveis e Parâmetros

- Usar camelCase (ex: `valorTotal`, `nomeCompleto`)
- Nomes descritivos que indiquem o propósito
- Evitar abreviações, exceto as muito comuns (ex: `id`, `http`)

### 1.4 Constantes

- Usar SNAKE_CASE_MAIÚSCULO (ex: `TAXA_JUROS`, `VALOR_MAXIMO`)

### 1.5 Pacotes

- Usar apenas letras minúsculas (ex: `com.empresa.projeto.modulo`)

## 2. Formatação

### 2.1 Indentação

- Usar 4 espaços para indentação (não tabs)
- Alinhar chaves de abertura e fechamento verticalmente

### 2.2 Comprimento de Linha

- Limitar a 80-120 caracteres por linha
- Quebrar linhas longas de forma lógica

### 2.3 Espaços em Branco

- Um espaço após palavras-chave (if, for, while, etc.)
- Um espaço antes e depois de operadores (=, +, -, etc.)
- Sem espaços após parênteses de abertura e antes de parênteses de fechamento

### 2.4 Organização de Arquivos

- Uma classe por arquivo
- Ordem dos elementos: campos, construtores, métodos
- Agrupamento lógico de métodos relacionados

## 3. Documentação

### 3.1 Comentários

- Usar comentários para explicar "por quê", não "o quê" ou "como"
- Comentários de linha única: // Comentário
- Comentários de múltiplas linhas: /*Comentário*/

### 3.2 Javadoc/Docstrings

- Todos os métodos públicos devem ter documentação
- Incluir descrição, parâmetros, retorno e exceções
- Manter documentação atualizada com o código

## 4. Práticas de Codificação

### 4.1 Princípios SOLID

- Single Responsibility Principle: uma classe deve ter apenas uma razão para mudar
- Open/Closed Principle: aberto para extensão, fechado para modificação
- Liskov Substitution Principle: subtipos devem ser substituíveis por seus tipos base
- Interface Segregation Principle: interfaces específicas são melhores que uma interface geral
- Dependency Inversion Principle: depender de abstrações, não de implementações

### 4.2 Tratamento de Erros

- Usar exceções para condições excepcionais, não para fluxo de controle
- Sempre capturar exceções específicas, não genéricas
- Documentar exceções lançadas por métodos públicos

### 4.3 Código Limpo

- Métodos pequenos e com responsabilidade única
- Evitar código duplicado (DRY: Don't Repeat Yourself)
- Preferir composição à herança
- Minimizar efeitos colaterais
- Evitar números mágicos e strings hardcoded

## 5. Testes

### 5.1 Nomenclatura de Testes

- Padrão: `deveComportamentoEsperado_quandoCondicao()`
- Ex: `deveRetornarValorCorreto_quandoEntradaValida()`

### 5.2 Estrutura de Testes

- Seguir o padrão AAA (Arrange, Act, Assert)
- Testes unitários devem ser independentes entre si
- Usar mocks e stubs quando apropriado

### 5.3 Cobertura de Testes

- Visar cobertura de pelo menos 80% do código
- Priorizar testes para lógica de negócio crítica

## 6. Controle de Versão

### 6.1 Mensagens de Commit

- Formato: `[tipo]: descrição curta`
- Tipos: feat, fix, docs, style, refactor, test, chore
- Descrição no imperativo, clara e concisa

### 6.2 Branches

- Formato: `tipo/descricao-curta`
- Tipos: feature, bugfix, hotfix, docs, refactor
- Ex: `feature/cadastro-usuarios`, `bugfix/correcao-calculo`

>[!TIP]
>Consistência é mais importante que preferências pessoais. Siga estes padrões mesmo que você prefira outros estilos.
