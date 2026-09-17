# aaPanel Plugins

Plugins de terceiros e open source para aaPanel.

## Storm Analytics

**Storm Analytics** é uma alternativa self-hosted para analytics de sites administrados pelo aaPanel. Ele foi desenvolvido de forma independente, usando apenas interfaces públicas e comportamento documentado do aaPanel.

A versão `0.1.0` já inclui PV/UV/sessões, tempo real, fontes e UTM, navegador/SO/dispositivo, Web Vitals, heatmap opt-in, múltiplos sites, importação dos sites do aaPanel e injeção automática para Nginx com rollback.

Os dados ficam no próprio servidor. O collector escuta apenas em `127.0.0.1:19991` e o IP bruto do visitante não é persistido.

### Instalação rápida

Baixe o ZIP de distribuição e importe como plugin de terceiros no aaPanel, ou instale a partir do código:

```bash
cd /tmp
git clone https://github.com/danilostorm/aapanel-plugins.git
cd aapanel-plugins
cp -a storm_analytics /www/server/panel/plugin/
bash /www/server/panel/plugin/storm_analytics/install.sh install
bt restart
```

Consulte [`storm_analytics/README.md`](storm_analytics/README.md) para detalhes de uso, segurança e limitações.

> Projeto independente. Não contém código proprietário do aaPanel Pro e não tenta contornar o licenciamento do plugin comercial.
