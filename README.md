## Soap-Provedor-Database 
Exemplo de criação de WebServices utilizando SOAP com banco de dados SQL-Server.

### Requisitos
- Se necessário Acessar Visual Studio como administrador.
- Se necessário atribuir acesso de usuário NT Service\MSSQLSERVER a pasta App_Data.

### O que você vai encontrar neste projeto
- **SOAP** - Serviços de rede que permitem a troca de informações estruturadas (via XML) entre aplicações.

### Execução da aplicação
Para executar a aplicação é necessário: 

- Acessar link de referência da documentação: (http://localhost:54222/PessoaService.asmx)

### String de conexão do banco
Modifique o [DIRETORIO] na string de conexão no arquivo **PessoaService.asmx**, no trecho indicado:

```bash
Data Source=(LocalDB)\\MSSQLLocalDB;AttachDbFilename=[DIRETORIO]\\App_Data\\BancoTesteSoap.mdf;Integrated Security=True;"
```
O script para criação da Database do exemplo encontra-se na pasta **Database**.

### Frontend Web 
Projeto vinculado a **Razor-Consumir-SOAP** que se encontra no Github.
  - [Razor-Consumir-SOAP](https://github.com/Marcelofazan/razor-consumir-soap)
