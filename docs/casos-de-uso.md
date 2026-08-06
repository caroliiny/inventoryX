# Casos de Uso

> Projeto: InventoryX
>
> Versão: 0.1.0
>

---

# 1. Introdução

Este documento descreve os principais casos de uso do sistema InventoryX, especificando as interações entre os atores e o sistema.

Os casos de uso representam as funcionalidades disponíveis para cada tipo de usuário.

---

# 2. Atores

## Empresa

Representa a empresa que realiza o cadastro na plataforma.

---

## Usuário

Representa um funcionário autenticado que utiliza o sistema para gerenciar o estoque.

Na primeira versão do sistema, será considerado apenas um usuário administrador por empresa.

---

# 3. Diagrama Geral (Textual)

Empresa

- Cadastrar empresa

- Realizar login

    - Recuperar senha

↓

Usuário

- Gerenciar produtos

- Gerenciar categorias

- Gerenciar fornecedores

- Registrar entrada de produtos

- Registrar saída de produtos

- Visualizar dashboard

- Gerar relatórios

    - Atualizar perfil

---

# 4. Casos de Uso

## UC01 – Cadastrar Empresa

### Objetivo

Permitir que uma empresa crie uma conta na plataforma.

### Atores

Empresa

### Pré-condições

Nenhuma.

### Fluxo Principal

1. A empresa acessa a tela de cadastro.
2. Informa os dados obrigatórios.
3. O sistema valida as informações.
4. O sistema cria a empresa.
5. O sistema cria automaticamente o primeiro usuário administrador.
6. O sistema redireciona para o login.

### Pós-condições

A empresa passa a possuir uma conta válida.

---

## UC02 – Realizar Login

### Objetivo

Permitir acesso ao sistema.

### Atores

Usuário

### Pré-condições

Possuir cadastro ativo.

### Fluxo Principal

1. Informar e-mail.
2. Informar senha.
3. O sistema valida as credenciais.
4. O dashboard é exibido.

### Fluxos Alternativos

- E-mail inexistente.
- Senha incorreta.

### Pós-condições

Usuário autenticado.

---

## UC03 – Recuperar Senha

### Objetivo

Permitir redefinir a senha.

### Fluxo Principal

1. Informar e-mail.
2. O sistema envia um link de recuperação.
3. O usuário define uma nova senha.

---

## UC04 – Cadastrar Categoria

### Objetivo

Cadastrar uma categoria de produtos.

### Pré-condições

Usuário autenticado.

### Fluxo Principal

1. Acessar Categorias.
2. Clicar em "Nova Categoria".
3. Informar o nome.
4. Salvar.

### Pós-condições

Categoria cadastrada.

---

## UC05 – Editar Categoria

Objetivo:

Alterar informações de uma categoria existente.

---

## UC06 – Excluir Categoria

Objetivo:

Remover uma categoria sem produtos vinculados.

---

## UC07 – Cadastrar Fornecedor

### Objetivo

Cadastrar fornecedores da empresa.

### Fluxo Principal

1. Informar nome.
2. Informar telefone.
3. Informar e-mail.
4. Informar endereço.
5. Salvar.

---

## UC08 – Editar Fornecedor

Alterar informações de um fornecedor.

---

## UC09 – Excluir Fornecedor

Excluir fornecedor que não esteja vinculado a produtos.

---

## UC10 – Cadastrar Produto

### Objetivo

Cadastrar um novo produto.

### Fluxo Principal

1. Acessar Produtos.
2. Clicar em "Novo Produto".
3. Informar:
   - Nome
   - Código
   - SKU
   - Categoria
   - Fornecedor
   - Quantidade
   - Estoque mínimo
   - Estoque máximo
   - Preço
4. Salvar.

### Pós-condições

Produto disponível no estoque.

---

## UC11 – Editar Produto

Alterar qualquer informação do produto.

---

## UC12 – Excluir Produto

Excluir produto sem movimentações ou marcá-lo como inativo.

---

## UC13 – Pesquisar Produto

### Objetivo

Localizar rapidamente produtos.

### Critérios

Pesquisar por:

- Nome
- Código
- SKU
- Categoria

---

## UC14 – Registrar Entrada de Estoque

### Objetivo

Adicionar unidades ao estoque.

### Fluxo Principal

1. Selecionar produto.
2. Informar quantidade.
3. Informar motivo.
4. Confirmar.

### Pós-condições

Quantidade atualizada.

Movimentação registrada.

---

## UC15 – Registrar Saída de Estoque

### Objetivo

Remover unidades do estoque.

### Fluxo Principal

1. Selecionar produto.
2. Informar quantidade.
3. Informar motivo.
4. Confirmar.

### Pós-condições

Quantidade reduzida.

Movimentação registrada.

---

## UC16 – Visualizar Dashboard

### Objetivo

Exibir indicadores do estoque.

### Informações exibidas

- Total de produtos
- Produtos com estoque baixo
- Produtos cadastrados
- Últimas movimentações

---

## UC17 – Visualizar Histórico

### Objetivo

Consultar todas as movimentações realizadas.

### Filtros

- Produto
- Usuário
- Data
- Tipo de movimentação

---

## UC18 – Gerar Relatórios

### Objetivo

Emitir relatórios do estoque.

### Tipos

- Produtos
- Movimentações
- Estoque baixo

---

## UC19 – Atualizar Perfil

### Objetivo

Alterar informações da empresa.

### Fluxo Principal

1. Acessar Perfil.
2. Alterar informações.
3. Salvar.

---

## UC20 – Realizar Logout

### Objetivo

Encerrar a sessão do usuário.

### Fluxo Principal

1. Clicar em "Sair".
2. O sistema encerra a sessão.
3. O usuário retorna para a tela de login.

---

# 5. Observações

- Todos os casos de uso, exceto cadastro, login e recuperação de senha, exigem autenticação.
- Cada empresa visualizará apenas seus próprios dados.
- Todas as movimentações de estoque serão registradas automaticamente para auditoria.