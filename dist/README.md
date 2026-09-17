# Storm Analytics — pacote aaPanel

Pacote instalável gerado para teste no aaPanel 8.x.

- Arquivo: `storm_analytics-aaPanel-v0.1.0.zip`
- Versão: `0.1.0`
- SHA-256: `2aede49dfebc75a876a0692fec4473a9cbc0501c4a9b7f06df8bac62d829a245`

## Instalação manual

No aaPanel, use a opção de importação de plugin de terceiros e selecione o ZIP desta pasta. O pacote foi estruturado para que os arquivos do plugin fiquem na raiz do ZIP, conforme o mecanismo `input_zip` do aaPanel.

O plugin cria um collector local em `127.0.0.1:19991`, mantém os dados em SQLite dentro do diretório do plugin e usa Nginx para a injeção automática do tracker.

> Projeto independente. Não contém código proprietário nem contorna licenciamento do Website Analytics oficial do aaPanel Pro.
