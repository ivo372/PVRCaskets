## Website de Loja de Caixões - Documentação Técnica

# Objetivo

Este projeto consiste numa loja online para exposição de caixões, permitindo aos visitantes visualizar os produtos e entrar em contacto com o proprietário. Não existe funcionalidade de compra direta. A intenção é fornecer um frontend funcional e preparado para integração com backend.

# Situação Atual do Frontend

O frontend está praticamente finalizado com as seguintes páginas:

- index.html: Página inicial com produtos em destaque (conteúdo hardcoded).

- products.html: Página para listar todos os produtos (estrutura pronta para conteúdo dinâmico).

- about.html: Página "Sobre Nós" com informações institucionais.

- contact.html: Página de contacto com formulário.

- 404.html: Página de erro personalizada (recentemente adicionada).

- política-de-privacidade.html: Página com política de privacidade genérica.

- Área de Administração (Layout apenas)

- admin-login.html: Login para administradores.

- admin-products.html: Gestão dos produtos (listar, editar, apagar, adicionar).

- admin-add-product.html: Formulário para adicionar novos produtos.

- admin-edit-product.html: Formulário para editar produtos existentes.

Todas essas páginas estão totalmente estáticas e prontas para integração.

## O Que Está Implementado

Estrutura HTML, CSS e JS completa.

Design responsivo com layout limpo e adaptável.

Comentários no código indicando os pontos onde deve existir conteúdo dinâmico.

Layouts administrativos com botões e formulários prontos (sem funcionalidade).

## O Que Falta Implementar (Para o Backend Developer)

1. Integração com Base de Dados

Os produtos, informações e listas estão todos hardcoded.

Precisa-se de uma base de dados (MongoDB, MySQL, etc.) para:

Armazenar produtos, descrições, imagens, categorias.

Associar produtos à homepage ou à listagem geral.

2. Funcionalidade Dinâmica

index.html: Destacar produtos dinâmicos da base de dados.

products.html: Listar todos os produtos dinamicamente.

product.html: Página de detalhes de cada produto.

Formulários administrativos: Devem carregar e enviar dados reais.

3. Área de Administração

Autenticação (login do administrador, proteção das páginas).

CRUD de produtos (criar, ler, atualizar, apagar).

Validações de formulários e mensagens de feedback (sucesso/erro).

Gestão de categorias, filtros ou destaques (homepage vs. produtos gerais).

4. Formulário de Contacto

Enviar mensagem por email (via SMTP, serviço externo, etc.).

Validação de campos obrigatórios e mensagem de confirmação.

5. Segurança e Acesso

Proteger rotas administrativas (redirecionar se não autenticado).

Escapar inputs, evitar XSS, CSRF, etc.

## Notas para o Desenvolvedor Backend

O código HTML contém comentários identificando os pontos dinâmicos.

Os formulários de adicionar e editar estão prontos para receber GET/POST e integração com API.

Os botões (editar, apagar, adicionar) estão prontos visualmente — precisam apenas de lógica JS/API.

A estrutura está preparada para usar JSON, templates ou renderização dinâmica.

O layout é simples de reaproveitar com qualquer framework (Node/Express, Laravel, Django, etc.).

Se notar algo que possa ser melhorado ou otimizado, o backend developer tem liberdade total para alterar ou expandir a lógica conforme necessário.

## Sugestões de Melhorias Futuras

Adicionar paginação ou busca de produtos.

Criar sistema de categorias/etiquetas.

Implementar painel com estatísticas de visitas ou produtos mais visualizados.

Adicionar um sistema de favoritos (sem necessidade de login).

CMS simples para editar textos estáticos (ex: About, Política de Privacidade).

## Como Avançar

Revisar a estrutura HTML/CSS existente.

Criar e modelar a base de dados.

Desenvolver API ou sistema de renderização para carregar os produtos dinamicamente.

Implementar autenticação do administrador.

Ligar os formulários e botões à base de dados e lógica backend.

Adicionar validações, mensagens de feedback e segurança básica.

## Atenção

Este website foi editado apartir de um template com o frontend bastante completo. Após a edição, muito código pode ter ficado inativo.

A página index.html foi criada com o intuito de ser uma página de exemplo, sendo que foi tudo feito em hardcode. Ou seja pode ser que haja algumas falhas na preparação para o backend.

As páginas de admin foram criadas com um design simples para facilitar o uso e a gestão. Contudo podem haver falhas na preparação para o backend, como na maneira como os dados serão carregados e tratados.

A página de produtos.html foi criada com o intuito de ser uma página de exemplo, sendo que foi tudo feito em hardcode. Ou seja pode ser que haja algumas falhas na preparação para o backend. O objetivo é que cada produto seja adicionado pelas páginas de admin, e que o backend carregue os dados de forma dinâmica. O exemplo foi mostrar como se devem comportar os produtos ao serem adicionados á página.

## Sugestão

Uma página de produto individual deveria ser adicionada
