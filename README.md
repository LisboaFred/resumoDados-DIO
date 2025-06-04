# resumoDados-DIO
# Azure DB Lab Notes 🗄️

Este repositório contém resumos, anotações e dicas práticas sobre a configuração de instâncias de banco de dados na plataforma Microsoft Azure.

## Objetivo
Registrar o aprendizado obtido durante o laboratório e servir como guia para estudos e implementações futuras.

## Conteúdo
- Introdução ao Banco de Dados no Azure
- Criação e configuração de instâncias SQL
- Regras de acesso, firewall e autenticação
- Backup, segurança e monitoramento
- Boas práticas e resolução de erros comuns

# Criação de uma Instância de Banco de Dados SQL no Azure

## Etapas principais

1. **Acessar o portal Azure**  
   👉 [https://portal.azure.com](https://portal.azure.com)

2. **Criar um recurso**  
   - Buscar por "Banco de Dados SQL"
   - Selecionar subscrição e grupo de recursos
   - Definir nome do banco de dados

3. **Configurar o servidor**  
   - Criar novo servidor (nome, login e senha de administrador)
   - Selecionar região

4. **Configurações adicionais**  
   - Escolher camada de desempenho (DTU ou vCore)
   - Habilitar backups automáticos
   - Criptografia de dados

5. **Regras de firewall**  
   - Adicionar IPs confiáveis para acesso

6. **Revisar e criar**  
   - Confirmar todas as informações e clicar em "Criar"
  
  # Boas Práticas para Banco de Dados no Azure

- Utilize **IP dinâmico + nome DNS** apenas com autenticação segura.
- Sempre ative **firewall e criptografia TDE (Transparent Data Encryption)**.
- Configure **backups automáticos** com retenção adequada.
- Use **alertas de monitoramento** para CPU, DTU, tempo de resposta e falhas de conexão.
- Separe ambientes de **produção, homologação e desenvolvimento**.
- Use **Azure Active Directory** para controle de acesso se possível.
