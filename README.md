# Projeto-Azure-database
Desafio de projeto Configurando uma instância de Banco de Dados na Azure - DIO


#  Guia de Apoio – Banco de Dados no Microsoft Azure  

Este documento reúne **resumos, anotações e dicas práticas** para configurar e gerenciar instâncias de banco de dados na plataforma **Microsoft Azure**.  

---

##  1. Introdução ao Azure Database  
- O Azure oferece **bancos de dados como serviço (DBaaS)**, eliminando a necessidade de configuração manual de servidores.  
- Principais opções:  
  - **Azure SQL Database** – Banco relacional baseado no SQL Server.  
  - **Azure Database for MySQL** – Serviço gerenciado para MySQL.  
  - **Azure Database for PostgreSQL** – Serviço gerenciado para PostgreSQL.  
  - **Cosmos DB** – Banco multimodelo, altamente escalável.  

---

##  2. Criando uma Instância de Banco no Azure  
1. Acesse o **Portal do Azure**: [https://portal.azure.com](https://portal.azure.com).  
2. Clique em **Criar um recurso** > **Banco de Dados**.  
3. Escolha o tipo (SQL, MySQL, PostgreSQL etc.).  
4. Configure:  
   - **Nome do servidor** (único na nuvem).  
   - **Usuário administrador** e senha.  
   - **Camada de desempenho** (Basic, General Purpose, Business Critical).  
   - **Região** (data center mais próximo para menor latência).  
5. Defina as regras de firewall para permitir acesso ao banco.  
6. Clique em **Revisar + Criar**.  

---

##  3. Boas Práticas de Segurança  
- Sempre habilite **autenticação com Azure Active Directory**.  
- Use **firewall** e **regras de IP** para limitar conexões.  
- Ative **TLS/SSL** para conexões criptografadas.  
- Nunca compartilhe a senha do administrador; prefira **usuários com permissões limitadas**.  

---

##  4. Monitoramento e Escalabilidade  
- O Azure fornece métricas em tempo real:  
  - Uso de **CPU**  
  - Consumo de **memória**  
  - **I/O de disco**  
- Use o recurso de **escalabilidade elástica** para aumentar ou reduzir a capacidade de acordo com a demanda.  
- Configure **alertas** para notificações de desempenho.  

---

##  5. Backup e Recuperação  
- O Azure realiza **backups automáticos** diariamente.  
- É possível configurar **ponto de restauração** para recuperar dados até os últimos 35 dias (dependendo do plano).  
- Utilize **geo-redundância** para proteger contra falhas regionais.  

---

##  6. Dicas Rápidas  
- ✅ Teste com **versão gratuita** (Free Trial) antes de contratar um plano.  
- ✅ Sempre organize os recursos dentro de **Resource Groups**.  
- ✅ Use **Azure CLI** ou **PowerShell** para automação.  
- ✅ Para estudo, utilize ferramentas como **Azure Data Studio** ou **SQL Server Management Studio (SSMS)** para gerenciar o banco.  

---

##  Referências Úteis  
- [Documentação oficial – Azure SQL Database](https://learn.microsoft.com/azure/azure-sql)  
- [Documentação oficial – Azure Database for MySQL](https://learn.microsoft.com/azure/mysql)  
- [Documentação oficial – Azure Database for PostgreSQL](https://learn.microsoft.com/azure/postgresql)  
- [Azure CLI – Comandos para banco de dados](https://learn.microsoft.com/cli/azure/db)  

---

✍️ **Autor:** *[Seu Nome]*  
📅 **Data:** *[Atualize aqui]*  
