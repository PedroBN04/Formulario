# Formulário e Perfil de Usuário

Sistema de cadastro e exibição de perfil de usuário desenvolvido com HTML, CSS e JavaScript puro. O fluxo cobre entrada de dados, validação em tempo real, armazenamento temporário em sessão e renderização do perfil em página dedicada — com suporte a tema claro/escuro.

---

## Sumário

1. [Tecnologias](#tecnologias)
2. [Funcionalidades](#funcionalidades)
3. [Estrutura do Projeto](#estrutura-do-projeto)
4. [Como Executar](#como-executar)
5. [Melhorias Futuras](#melhorias-futuras)
6. [Autor](#autor)
7. [Licença](#licença)

---

## Tecnologias

| Tecnologia | Uso |
|------------|-----|
| HTML5 | Estrutura semântica das páginas |
| CSS3 | Estilização, responsividade e temas claro/escuro |
| JavaScript ES6+ | Manipulação de DOM, validação de formulário e `sessionStorage` |

---

## Funcionalidades

**Cadastro de usuário**
Coleta nome, e-mail e idade com validação dinâmica de campos obrigatórios e regras de formato aplicadas antes do envio.

**Armazenamento temporário**
Dados persistem via `sessionStorage` enquanto a sessão do navegador está ativa. Ao fechar a aba, os dados são descartados automaticamente.

**Exibição de perfil**
A página `perfil.html` carrega e renderiza automaticamente os dados salvos na sessão. Caso não haja dados disponíveis, o usuário é redirecionado ao formulário.

**Tema claro/escuro**
Alternância de tema disponível em ambas as páginas para melhor experiência de leitura.

**Encerramento de sessão**
Botão de saída limpa os dados do `sessionStorage` e retorna o usuário ao formulário.

---

## Estrutura do Projeto

```
/
├── index.html          # Página do formulário de cadastro
├── perfil.html         # Página de exibição do perfil
├── css/
│   ├── design.css      # Estilização do formulário
│   └── user.css        # Estilização da página de perfil
├── js/
│   ├── test.js         # Validação do formulário e gravação no sessionStorage
│   └── usuario.js      # Leitura e renderização dos dados do perfil
├── img/                # Recursos de imagem
└── README.md
```

---

## Como Executar

O projeto não requer servidor ou dependências externas — basta abrir o HTML no navegador.

```bash
# 1. Clone o repositório
git clone https://github.com/PedroBN04/Formulario.git

# 2. Acesse a pasta do projeto
cd Formulario

# 3. Abra a página inicial no navegador
open index.html        # macOS
xdg-open index.html    # Linux
start index.html       # Windows
```

Ou arraste o arquivo `index.html` diretamente para o navegador de sua preferência.

---

## Melhorias Futuras

- Substituição do `sessionStorage` por `localStorage` ou integração com banco de dados para persistência entre sessões.
- Sistema de autenticação com login e senha.
- Expansão da cobertura de acessibilidade (ARIA labels, navegação por teclado, contraste WCAG AA).
- Testes automatizados de validação de formulário.

---

## Autor

**Pedro Humberto Bitencourt Nascimento**

- [GitHub](https://github.com/PedroBN04)
- [LinkedIn](https://www.linkedin.com/in/seu-perfil)

---

## Licença

Distribuído sob a licença MIT. Consulte o arquivo [LICENSE](https://github.com/PedroBN04/Formulario/blob/main/LICENSE) para mais detalhes.
