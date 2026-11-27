# Loterias 24 Horas

Site dos bolões da Lotérica da Avenida (Vilela & Granhani), Pirassununga/SP: https://loterias24horas.com.br

## Atualizar os bolões

Tudo fica no `dados.json`:

- `boloes`: um item por bolão: `lot` (mega, quina, loteca, milionaria, dupla, timemania, lotofacil), `concurso`, `quando` (sorteio, ou fim das apostas na Loteca, com `-03:00`), `premio`, `formato`, `cotas` (total), `restam`, `valor` (cota no balcão) e, se houver, `app` (cota no app da Caixa), `nome`, `selo`, `link`.
- `virada.boloes`: os bolões da Mega da Virada.

O bolão some sozinho 15 minutos antes de `quando`. As cotas só mudam com o print oficial da Caixa.

O `index.html` é montado por script e já traz os bolões escritos (melhor para o Google). Se só o `dados.json` mudar, o site continua certo: o navegador relê o arquivo ao abrir.
