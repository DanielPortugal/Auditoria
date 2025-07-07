# 🗄️ Oracle Tuning & Auditoria - SQL Scripts

Este repositório contém um conjunto de scripts SQL para análise de performance, auditoria padrão e criação de políticas FGA (*Fine-Grained Auditing*) em bancos de dados Oracle. O objetivo é fornecer ferramentas úteis para DBAs e desenvolvedores monitorarem e ajustarem o ambiente de forma prática.  

---

## 📑 Sumário

- [📊 Performance](#-performance)
- [🔐 FGA (Fine-Grained Auditing)](#-fga-fine-grained-auditing)
- [🛡️ Auditoria Padrão](#-auditoria-padrão)
- [🚀 Como usar](#-como-usar)
- [🛠️ Tecnologias](#-tecnologias)
- [📂 Organização](#-organização)
- [👨‍💻 Autor](#-autor)
- [📝 Licença](#-licença)

---

## 📊 Performance

Scripts voltados para análise e diagnóstico de performance:  

| 📄 Script                                           | 📝 Descrição                                                                                     |
|-----------------------------------------------------|---------------------------------------------------------------------------------------------------|
| `alterar_configuracoes_awr.sql`                     | Altera as configurações do AWR (*Automatic Workload Repository*).                                 |
| `consultar_awr_parametro.sql`                       | Consulta os parâmetros atualmente configurados no AWR.                                            |
| `consultar_buffer_busy_waits.sql`                   | Verifica ocorrências de *buffer busy waits*.                                                      |
| `consultar_carga_bd_horas_uso_e_IO_diaria.sql`      | Analisa a carga do banco por hora e o uso de I/O diário.                                          |
| `consultar_estatisticas_services_waits.sql`         | Consulta estatísticas de espera agrupadas por serviços.                                           |
| `consultar_estatisticas_servicos.sql`               | Lista estatísticas gerais de performance por serviço.                                             |
| `consultar_historico_leituras_full_X_index.sql`     | Verifica histórico de leituras full table e uso de índices.                                       |
| `consultar_leituras_full_X_index.sql`               | Analisa leituras full table versus leituras por índice.                                           |
| `consultar_linhas_encadeadas.sql`                   | Identifica linhas encadeadas (*chained rows*) no banco.                                           |
| `consultar_tamanho_shared_pool_reserved.sql`        | Consulta o tamanho da área reservada no *shared pool*.                                            |
| `consultar_total_waits.sql`                         | Lista os eventos de espera totais no banco.                                                       |
| `consultar_wait_events_awr.sql`                     | Consulta eventos de espera registrados no AWR.                                                    |
| `verificar_IO_estatisticas_servicos_background.sql` | Analisa estatísticas de I/O e serviços de background.                                             |
| `verificar_cache_hit_ratio.sql`                     | Verifica o *cache hit ratio* da instância.                                                        |
| `verificar_desempenho_sorts.sql`                    | Analisa o desempenho de operações de *sort*.                                                      |
| `verificar_library_cache_hit_ratio.sql`             | Verifica o hit ratio do *library cache*.                                                          |
| `verificar_qtde_transacoes.sql`                     | Consulta a quantidade de transações executadas no banco.                                          |
| `verificar_tabelas_estatisticas_scan.sql`           | Identifica tabelas com estatísticas desatualizadas ou varreduras completas (*full scan*).         |

---

## 🔐 FGA (Fine-Grained Auditing)

Scripts para criação e gerenciamento de políticas de auditoria FGA:  

| 📄 Script                            | 📝 Descrição                                                                 |
|--------------------------------------|-------------------------------------------------------------------------------|
| `criar_policy_auditoria_fga.sql`     | Cria uma policy de auditoria *Fine-Grained Auditing (FGA)* no banco de dados. |

---

## 🛡️ Auditoria Padrão

Scripts para consultar, habilitar e gerenciar a auditoria padrão do Oracle:  

| 📄 Script                                               | 📝 Descrição                                                                                          |
|---------------------------------------------------------|--------------------------------------------------------------------------------------------------------|
| `consultar_auditoria_sistema_habilitada_por_usuario.sql`| Lista auditorias habilitadas no sistema por usuário.                                                  |
| `consultar_objetos_auditados.sql`                       | Consulta os objetos que possuem auditoria ativada.                                                    |
| `consultar_privilegios_auditados.sql`                   | Lista os privilégios auditados no banco.                                                              |
| `consultar_registros_auditoria_padrao.sql`              | Consulta registros de auditoria padrão.                                                               |
| `consultar_registros_auditoria_padrao_filtros.sql`      | Consulta registros de auditoria padrão com filtros aplicados.                                         |
| `consumo_cpu_mensal_por_usuario.sql`                    | Verifica o consumo de CPU mensal agrupado por usuário.                                                |
| `gerar_auditoria_itens.sql`                             | Gera auditoria para itens específicos.                                                                |
| `habilita_auditoria_todos_objetos_schema.sql`           | Habilita auditoria para todos os objetos de um schema.                                                |
| `habilitar_desabilitar_auditoria_por_usuario.sql`       | Habilita ou desabilita auditoria para usuários específicos.                                           |
| `limpar_registros_auditoria.sql`                        | Limpa os registros de auditoria do banco.                                                             |
| `manutencao_tabela_registros_auditoria.sql`             | Realiza manutenção na tabela de registros de auditoria.                                               |

---


