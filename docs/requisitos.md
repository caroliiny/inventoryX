# Requisitos do Sistema

> Versão: 0.1.0

---

# Requisitos Funcionais

## RF01 — Cadastro de Empresa

O sistema deverá permitir que uma empresa realize seu cadastro informando:

- Nome da empresa
- CNPJ
- E-mail
- Senha
- Telefone

---

## RF02 — Login

O sistema deverá permitir autenticação utilizando:

- e-mail;
- senha.

---

## RF03 — Logout

O sistema deverá permitir que o usuário encerre sua sessão.

---

## RF04 — Recuperação de Senha

O sistema deverá permitir recuperar a senha por e-mail.

---

## RF05 — Perfil da Empresa

A empresa poderá editar seus dados cadastrais.

---

## RF06 — Cadastro de Categorias

O sistema deverá permitir cadastrar categorias de produtos.

---

## RF07 — Edição de Categorias

Permitir alterar categorias existentes.

---

## RF08 — Exclusão de Categorias

Permitir remover categorias que não estejam sendo utilizadas.

---

## RF09 — Cadastro de Fornecedores

Cadastrar fornecedores contendo:

- nome;
- telefone;
- e-mail;
- endereço.

---

## RF10 — Editar Fornecedor

Permitir alteração dos dados.

---

## RF11 — Excluir Fornecedor

Permitir remoção de fornecedores.

---

## RF12 — Cadastro de Produtos

Cadastrar produtos contendo:

- nome;
- descrição;
- código;
- SKU;
- categoria;
- fornecedor;
- preço;
- quantidade;
- estoque mínimo;
- estoque máximo.

---

## RF13 — Editar Produto

Permitir alterar qualquer informação do produto.

---

## RF14 — Excluir Produto

Permitir excluir produtos.

---

## RF15 — Pesquisa de Produtos

Pesquisar por:

- nome;
- código;
- SKU;
- categoria.

---

## RF16 — Filtros

Filtrar produtos por:

- categoria;
- fornecedor;
- quantidade;
- data.

---

## RF17 — Entrada de Estoque

Registrar entrada de produtos.

---

## RF18 — Saída de Estoque

Registrar saída de produtos.

---

## RF19 — Histórico

Registrar automaticamente todas as movimentações realizadas.

---

## RF20 — Dashboard

Exibir indicadores contendo:

- total de produtos;
- produtos em estoque baixo;
- produtos cadastrados;
- movimentações recentes.

---

## RF21 — Relatórios

Permitir emissão de relatórios.

---

## RF22 — Pesquisa Global

Permitir localizar rapidamente qualquer produto.

---

## RF23 — Auditoria

Registrar:

- usuário;
- data;
- horário;
- ação realizada.

---

# Requisitos Não Funcionais

## RNF01

O sistema deverá possuir interface responsiva.

---

## RNF02

O sistema deverá ser desenvolvido utilizando Next.js.

---

## RNF03

O sistema deverá utilizar React.

---

## RNF04

O sistema deverá utilizar TypeScript.

---

## RNF05

O banco de dados deverá ser PostgreSQL.

---

## RNF06

O ORM utilizado será Prisma.

---

## RNF07

O sistema deverá possuir autenticação segura.

---

## RNF08

As senhas deverão ser armazenadas criptografadas.

---

## RNF09

As informações deverão ser isoladas por empresa.

---

## RNF10

O sistema deverá possuir tempo médio de resposta inferior a 2 segundos para operações comuns.

---

## RNF11

O sistema deverá possuir código organizado seguindo arquitetura em camadas.

---

## RNF12

O sistema deverá seguir boas práticas de acessibilidade.

---

## RNF13

O sistema deverá possuir layout responsivo para desktop e dispositivos móveis.

---

## RNF14

O sistema deverá ser versionado utilizando Git.

---

## RNF15

O projeto deverá possuir documentação técnica.

---

# Regras de Negócio

## RN01

Cada empresa visualizará apenas seus próprios dados.

---

## RN02

Não será permitido cadastrar dois produtos com o mesmo código dentro da mesma empresa.

---

## RN03

O estoque nunca poderá possuir quantidade negativa.

---

## RN04

Toda entrada ou saída deverá gerar uma movimentação.

---

## RN05

Toda alteração em produtos deverá atualizar automaticamente a data de modificação.

---

## RN06

Produtos vinculados a movimentações não poderão ser excluídos permanentemente (preferencialmente, serão inativados).

---

## RN07

Categorias em uso por produtos não poderão ser excluídas.

---

## RN08

Fornecedores vinculados a produtos não poderão ser excluídos sem tratamento prévio.

---

## RN09

A empresa deverá possuir um e-mail único no sistema.

---

## RN10

O CNPJ deverá ser único no sistema.