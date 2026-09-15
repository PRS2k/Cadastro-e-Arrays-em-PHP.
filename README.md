# 🔞 Verificador de Maioridade em PHP

Aplicação web simples desenvolvida em PHP e HTML para validar se um usuário é maior de idade (18 anos ou mais) e registrar os acessos permitidos em um arquivo de log local.

---

## 🚀 Como Funciona

1. O usuário preenche o formulário com o seu **Nome** e **Ano de Nascimento**.
2. O PHP intercepta a requisição via método `POST` e calcula a idade subtraindo o ano de nascimento do ano atual (`date('Y')`).
3. **Validação:**
   - **Idade ≥ 18 anos:** Exibe um alerta JavaScript de **Acesso Permitido** e grava o registro no arquivo `log_acessos.txt`.
   - **Idade < 18 anos:** Exibe um alerta JavaScript de **Acesso Negado** (sem gravação de log).

---

📁 Estrutura do Projeto

**5a_desafio1_.php**: Arquivo principal contendo a estrutura da página HTML e o script PHP responsável por processar o formulário e gerenciar a escrita no arquivo de log.
**log_acessos.txt**: Arquivo texto de log onde são armazenados os registros dos usuários com acesso permitido (criado/atualizado automaticamente via PHP).
**usuarios.txt**: Arquivo de texto contendo dados cadastrais de usuários do sistema.

---

## 🛠️ Tecnologias Utilizadas

**PHP** (Processamento do formulário no servidor e manipulação de arquivos com fopen, fwrite e fclose)
**HTML5** (Estruturação do formulário de entrada)
**JavaScript** (Notificações em tela via alert)

---

## 💻 Como Executar o Projeto

1. **Requisitos:** É necessário ter um ambiente de desenvolvimento PHP instalado, como [XAMPP](https://www.apachefriends.org/), [WAMP](https://www.wampserver.com/) ou [Laragon](https://laragon.org/).
2. **Instalação:**
   * Clone ou copie os arquivos do projeto para a pasta raiz do servidor web (ex: htdocs no XAMPP).
3. **Execução:**
   * Inicie o serviço do servidor **Apache**.
   * Abra o navegador e acesse: `http://localhost/5a_desafio1_.php`.

---

## 📄 Formato dos Arquivos de Dados

### log_acessos.txt
Armazena o nome e a idade do usuário aprovado separados por ;:
textDANIEL PIRES CRISOSTOMO DE OLIVEIRA;26
