# Website de Loja de Caixões - Documentação

## Situação Atual

Este projeto consiste numa loja online para exposição de caixões, onde os clientes podem consultar preços e características dos produtos, mas não podem efetuar compras diretamente no site. Para adquirir um produto, o cliente deve entrar em contacto com o proprietário através da página de contactos.

O frontend do site está praticamente concluído, com as seguintes páginas principais:

- **index.html**: Página inicial com produtos em destaque (atualmente hardcoded).
- **products.html**: Página para listar todos os produtos (estrutura preparada, sem produtos dinâmicos).
- **about.html**: Página "Sobre Nós".
- **contact.html**: Página de contactos com formulário de contacto para futuro de contacto.
- **admin-login.html**: Página de login para acesso à área de administração (apenas layout, sem funcionalidade).
- **admin-products.html**: Gestão de produtos (listar, editar, apagar, adicionar - apenas layout).
- **admin-add-product.html**: Formulário para adicionar novo produto (apenas layout).
- **admin-edit-product.html**: Formulário para editar produto existente (apenas layout).

## O que está feito

- Estrutura HTML/CSS/JS de todas as páginas, incluindo layout e design básico. Verifição da estrutura é aconselhada antes iniciar o backend
- Comentários claros no código a indicar onde o conteúdo deverá ser dinâmico no futuro.
- Layouts estáticos para toda a área de administração, incluindo formulários de adicionar e editar produtos.
- Botões e funcionalidades de gestão (adicionar, editar, apagar) estão presentes mas desativados (apenas para referência visual). Ter em atenção que alguns botões podem não estar conectados ás páginas correspondentes.

## O que está em falta (e porquê)

- **Ligação a base de dados**:  
  Não existe qualquer ligação a base de dados. Todos os produtos e informações estão hardcoded no HTML.  
  Isto foi deixado de fora porque o objetivo era apenas preparar o frontend para que um programador backend possa, posteriormente, implementar a lógica de ligação à base de dados.

- **Formulário de contacto**: 
    O formulário de contacto está presente, mas não está configurado para enviar e-mails.

- **Funcionalidade dinâmica**:  
  As páginas de administração (login, adicionar, editar, apagar) não têm qualquer funcionalidade.  
  Falta implementar:
  - Autenticação de administrador
  - Listagem dinâmica dos produtos
  - Edição, adição e remoção de produtos na base de dados
  - Gestão de onde cada produto aparece (homepage, products, ambos)

- **Validação de formulários e mensagens de erro/sucesso**:  
  Não existem validações nem mensagens dinâmicas, como por exemplo "O produto foi editado com sucesso".  
  Isto será tratado quando o backend estiver implementado.

- **Proteção de páginas de administração**:  
  Qualquer pessoa pode aceder às páginas de administração diretamente pelo link.  
  Só com backend será possível proteger estas páginas com autenticação.

## Notas para o programador backend

- Todos os locais onde o conteúdo deve ser dinâmico estão devidamente comentados no HTML.
- As listas de características dos produtos estão preparadas para serem geradas a partir de arrays/listas vindas da base de dados.
- Os botões de ação (adicionar, editar, apagar) estão presentes mas desativados, prontos para serem ligados à lógica backend.
- Os formulários de adicionar e editar produto estão prontos para receber dados dinâmicos e enviar alterações para a base de dados.
- Caso exista algo que o programador ache que irá melhor o website em qualquer maneira, tem a liberdade de fazer as alterações necessárias.

## Como avançar

0. Verifique se a estrutura HTML/CSS/JS está correta e está de acordo com as necessidades do projeto.
1. Implementar a base de dados para armazenar os produtos e respetivas características.
2. Ligar o frontend ao backend para tornar as páginas dinâmicas.
3. Implementar autenticação de administrador e proteção das páginas de gestão.
4. Ativar e programar os botões de ação nos formulários e tabelas de administração.

---

Qualquer dúvida ou questão sobre a estrutura do frontend, os comentários no código servem de guia para integração futura.