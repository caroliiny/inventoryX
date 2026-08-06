# Sistema de Controle de Estoque - InventoryX

---

# 1. Introdução

O InventoryX é um sistema web desenvolvido para auxiliar empresas no gerenciamento de estoque de maneira prática, organizada e segura.

A aplicação permitirá que empresas realizem o controle completo de seus produtos, fornecedores, categorias e movimentações de estoque, centralizando todas as informações em um único ambiente.

O sistema será desenvolvido utilizando tecnologias modernas do ecossistema JavaScript, priorizando escalabilidade, desempenho, organização do código e boa experiência do usuário.

---

# 2. Problema

Muitas pequenas e médias empresas ainda realizam o controle de estoque utilizando planilhas eletrônicas ou processos manuais.

Esses métodos apresentam diversos problemas, como:

- dificuldade para localizar produtos;
- ausência de histórico de movimentações;
- erros de contagem;
- duplicidade de informações;
- falta de indicadores;
- pouca rastreabilidade das operações.

Esses fatores dificultam a gestão do estoque e aumentam o risco de prejuízos financeiros.

---

# 3. Objetivo Geral

Desenvolver um sistema web para gerenciamento de estoque que permita às empresas controlar seus produtos de forma organizada, segura e eficiente.

---

# 4. Objetivos Específicos

O sistema deverá permitir:

- cadastro de empresas;
- autenticação de usuários;
- gerenciamento de produtos;
- gerenciamento de categorias;
- gerenciamento de fornecedores;
- controle de entrada e saída de produtos;
- consulta do histórico de movimentações;
- geração de indicadores através de dashboard;
- pesquisa rápida de produtos;
- organização das informações por empresa.

---

# 5. Público-alvo

O sistema é destinado a:

- pequenas empresas;
- médias empresas;
- lojas;
- comércios;
- distribuidoras;
- empresas que necessitam controlar estoque.

---

# 6. Escopo

## O sistema contemplará

- autenticação;
- cadastro de empresa;
- CRUD de produtos;
- CRUD de categorias;
- CRUD de fornecedores;
- movimentações de estoque;
- dashboard;
- filtros;
- pesquisa;
- histórico de alterações.

---

## Fora do escopo (Versão 1.0)

Nesta primeira versão não serão implementados:

- emissão de nota fiscal;
- integração bancária;
- integração com marketplaces;
- controle financeiro;
- aplicativo mobile;
- leitura de código de barras.

Essas funcionalidades poderão ser adicionadas em versões futuras.

---

# 7. Tecnologias

## Front-end

- Next.js
- React
- TypeScript
- Tailwind CSS

## Back-end

- API Routes (Next.js)

## Banco de Dados

- PostgreSQL

## ORM

- Prisma

## Controle de Versão

- Git
- GitHub

---

# 8. Arquitetura Geral

Usuário

↓

Interface Web (Next.js)

↓

API

↓

Prisma

↓

PostgreSQL

---

# 9. Premissas

- Cada empresa possuirá sua própria conta.
- Os dados serão isolados por empresa.
- Apenas usuários autenticados poderão acessar o sistema.
- Todas as movimentações serão registradas.

---

# 10. Restrições

- Necessidade de conexão com internet.
- Navegadores modernos.

---

# 11. Futuras Implementações

- QR Code
- Código de barras
- Upload de imagens
- Exportação PDF
- Exportação Excel
- Controle por níveis de acesso
- Dashboard avançado