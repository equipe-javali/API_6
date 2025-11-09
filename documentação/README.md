<span id="topo">
<h1 align='center'>
:boar: EQUIPE JAVALI :boar:

APRENDIZAGEM POR PROJETOS INTEGRADOS

DOCUMENTAÇÃO
</h1>

<h1 align='center'> :keyboard:  :keyboard: </h1>

## :mag_right: Índice
<p align='center'> 
    <a href="#checklist">Checklist DoR e DoD</a>  |
    <a href="#estrategia">Estratégia de Branches</a>  |
    <a href="#usuario">Manual de Usuário</a> |
    <a href="#instalacao"> Manual de Instalação</a>
</p>

<span id="checklist">

## :pushpin: Checklist DoR e DoD 
### DoR - Definition of Ready
- User Stories com DoD
- Subtarefas divididas a partir das User Stories
- Design no Figma
- Modelagem do Banco de Dados
- Modelo de Boletim e Datasets
### DoD - Definition of Done
- Manual de Usuário
- Manual de Instalação
- Documentação do Sistema
- Atendimento aos requisitos
- Vídeos de cada etapa de entrega

<span id="estrategia">

## :twisted_rightwards_arrows: Estratégia de Branches

### Padrão de branch
As branches devem seguir o padrão: Task-{numero da tarefa}

Exemplos:
- Task-1
- Task-2

### Padrão de Commit
Existem **duas formas aceitas**:  

1. **Relacionado à tarefa da branch**:  {numero da tarefa} - {descrição do que foi feito}"    

Exemplos:
- 1 - Adição da rota de cadastro de usuário
- 2 - Criação da tela de Login

2. **Baseado em tipo de commit (Conventional Commits)**: {tipo de commit} - {descrição do que foi feito}"

Exemplos:
- fix - Correção na exibição do email do usuário
- test - Adição de testes da rota de cadastro

### Tipos de Commit
* **fix** - Indica que o trecho de código commitado está solucionando um problema ou bug.
* **docs** - Indica que houve mudanças na documentação.
* **test** - Indica que houve alterações criando, alterando ou excluindo testes;
* **build** - Indica que houve alterações relacionadas a build do projeto/dependências.
* **refactor** - Indica que uma parte do código foi refatorada sem alterações nas funcionalidades.
* **ci** - Indica mudanças relacionadas a integração contínua (Continuous Integration).
* **cleanup** - Indica a remoção de código comentado ou trechos desnecessários no código-fonte.
* **remove** - Indica a exclusão de arquivos, diretórios ou funcionalidades obsoletas ou não utilizadas.

→ [Voltar ao topo](#topo)

<span id="usuario">

## :bust_in_silhouette: Manual de Usuário

Bem-vindo ao manual de usuário do projeto Javali, desenvolvido no contexto da Aprendizagem por Projetos Integrados. Este documento tem como objetivo guiar os usuários em como utilizar a aplicação de forma eficiente e sem problemas. Abaixo, você encontrará instruções detalhadas de como interagir com as funcionalidades da aplicação.

1. Introdução

A aplicação foi desenvolvida para a partir da dataset fornecido pelo cliente Dom Rock, capaz de interpretar e responder perguntas dos usuários por meio de um agente de inteligência artificial integrado ao chat interativo. Além disso, deverá ter a funcionalidade de enviar um boletim, baseado no modelo fornecido pelo cliente, gerado pela ia com os dados de um dado período do dataset diretamente a um email. Este manual tem como objetivo fornecer as informações necessárias para que os usuários possam utilizar as funcionalidades da aplicação com facilidade.

2. Acesso ao Sistema
2.1 Como Acessar a Plataforma

Abra o navegador de sua escolha e vá até o seguinte endereço: [URL da aplicação].

Você verá a tela de login. Insira seu e-mail e senha para acessar.

2.2 Primeiros Passos

2.2.1 Administrador

Após o login, você será redirecionado à página inicial. A partir daqui, você poderá navegar pelas funcionalidades principais, como gerenciamento dos demais usuários (cria, deleta e modifica os usuparios, além de habilitar e desabilitar o envio do boletim).

2.2.2 Usuário comum

Após o login, você verá o chat por onde você poderá tirar dúvidas sobre a base de dados. Você poderá também, trocar a própria senha.

3. Funcionalidades
3.1 Boletim

Há um botelim enviado semanalmente com uma análise dos dados das últimas semanas da base de dados.

O boletim chega via e-mail para os usuários que estão habilitados.

3.2 Chat

O chat possibilita que os usuários tirem dúvidas sobre a base de dados com linguagem natural.

4. Conclusão

Obrigado por utilizar a plataforma Clara! Esperamos que este manual tenha sido útil e que você aproveite a experiência.

→ [Voltar ao topo](#topo)

<br>
<br>

<span id="instalacao">
    
## :floppy_disk: Manual de Instalação

<p align='center'> 
    <a href="#instalacao-back">Back End</a>  |
    <a href="#instalacao-front">Front End</a>  |
    <a href="#instalacao-banco">Banco de dados</a>
</p>

<span id="instalacao-back">

---

### Back End

**⚙️ Requisitos mínimos**

Antes de começar, certifique-se de ter instalado:

| Ferramenta | Versão recomendada | Link de instalação |
|-------------|--------------------|--------------------|
| **Python** | 3.10 ou superior | [python.org/downloads](https://www.python.org/downloads/) |
| **Git** | 2.x ou superior | [git-scm.com/downloads](https://git-scm.com/downloads) |
| **Editor de código** | VS Code, PyCharm ou similar | [code.visualstudio.com](https://code.visualstudio.com) |
| **Pip** | incluído com Python | — |

---

<br>

**📥 Instalação do projeto**

1. **Clonar o repositório**
   ```bash
   git clone https://github.com/equipe-javali/API_6_BACK.git
   ```

2. **Acessar o diretório**

    ```bash
    cd API_6_BACK
    ```

3. **Criar e ativar ambiente virtual**
    
    ```bash
    # Windows
    python -m venv venv
    venv\Scripts\activate
    
    # Linux / Mac
    python3 -m venv venv
    source venv/bin/activate
    ```

4. **Instalar as dependências**

    ```bash
    pip install -r requirements.txt
    ```
---
<br>

**▶️ Executar o servidor**

 1. Rodar o servidor FastAPI (garanta que continua no diretório `API_6_BACK`, se não acesse com `cd API_6_BACK`)
    
    ```bash
    python run
    ```

2. Acessar a documentação interativa
    - Swagger UI: http://127.0.0.1:8000/docs

3. Executar o frontend (API_6_FRONT)
   - Para testar integração, garanta que o backend esteja rodando localmente antes de iniciar o app Flutter.

<br>

<span id="instalacao-front">

### Front End

**⚙️ Requisitos mínimos**

Antes de começar, certifique-se de que as seguintes ferramentas estão instaladas:

| Ferramenta | Versão recomendada | Link de instalação |
|-------------|--------------------|--------------------|
| **Flutter SDK** | 3.x ou superior | [flutter.dev/docs/get-started/install](https://flutter.dev/docs/get-started/install) |
| **Git** | 2.x ou superior | [git-scm.com/downloads](https://git-scm.com/downloads) |
| **Editor de código** | VS Code ou Android Studio | [code.visualstudio.com](https://code.visualstudio.com) |
| **Emulador Android / iOS** | Opcional (para testes locais) | via Android Studio ou Xcode |

---

**📥 Instalação do projeto**

1. **Clonar o repositório**
   ```bash
   git clone https://github.com/equipe-javali/API_6_FRONT.git
   ```

2. **Acessar o diretório do projeto**
   ```bash
   cd API_6_FRONT
   ```

3. **Instalar as dependências**
   ```bash
   flutter pub get
   ```

4. **Executar o projeto**
   ```bash
   flutter run
   ```

> 💡 Dica: se houver mais de um dispositivo/emulador conectado, use  
> `flutter devices` para listar e `flutter run -d <device_id>` para escolher o destino.

---

**🧼 Solução de problemas**

| Problema | Solução recomendada |
|-----------|---------------------|
| **Erro “pub get failed”** | Execute `flutter clean` e depois `flutter pub get`. |
| **App não abre no emulador** | Verifique se há um dispositivo ativo (`flutter devices`). |
| **Erro de conexão com API** | Confirme o IP e a porta no arquivo de configuração da API. |
| **Erro de versão do Flutter** | Execute `flutter --version` e atualize se necessário. |

---

**🧪 Teste rápido**

Após `flutter run`, o app deve abrir exibindo a tela inicial (login). Utilize o seu login e senha para acessar a aplicação.

Verifique se os componentes estão sendo renderizados corretamente e se o log do terminal indica carregamento do frontend com sucesso.

---

<br>

<span id="instalacao-banco">

### Banco de dados

O backend utiliza um banco de dados PostgreSQL hospedado na plataforma **Neon.tech**, com autenticação restrita à equipe do projeto.

**🌐 Acesso e Conexão Segura**

As credenciais **não são públicas** e não estão versionadas no repositório.

A aplicação utiliza variáveis de ambiente armazenadas em um arquivo `.env` (não commitado no GitHub), com a seguinte estrutura:

```env
DATABASE_URL=postgresql+psycopg2://usuario:senha@ep-nome-do-banco.us-east-1.aws.neon.tech/db_nome
```

> ⚠️ Atenção:
> O arquivo .env deve ser criado manualmente pelos desenvolvedores autorizados.
> Para solicitar acesso ao banco, entre em contato com o responsável pela infraestrutura da equipe.


Caso queira subir um banco local, a nossa estrutura está documentada nos seguintes links:
- [Modelo de dados](https://github.com/equipe-javali/API_6_BD?tab=readme-ov-file#modelo)
- [Dicionário de dados](https://github.com/equipe-javali/API_6_BD?tab=readme-ov-file#scroll-dicion%C3%A1rio-de-dados)


→ [Voltar ao topo](#topo)
