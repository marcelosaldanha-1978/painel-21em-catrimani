# Painel 21EM — Op CATRIMANI II

Situação dos créditos orçamentários da **Operação CATRIMANI II**, para consulta do Estado-Maior.

**Site:** https://marcelosaldanha-1978.github.io/painel-21em-catrimani/

## O que o painel mostra

- **Ação imediata:** créditos com prazo de empenho vencido ou vencendo em até 7 dias, empenho imediato e crédito retido nos gestores.
- **Números da operação:** destacado, descentralizado, empenhado, liquidado, pago e disponível.
- **Cadeia do recurso:** MD → DCont → EME → gestores (COTER, COEx, DGO) → OM executoras.
- **Detalhe**, em abas: saldo por Nota de Crédito, créditos recebidos por OM, executoras, crédito retido nos gestores, empenhos sem vínculo a uma NC e método.

## Fonte e escopo

- **Fonte:** Tesouro Gerencial (relatórios R1 Créditos e R2 Empenhos).
- **Escopo:** Ação 21EM, **PTRES 251050** (PO 0003), órgão 52121 — Comando do Exército. O filtro pelo PTRES isola a CATRIMANI II de outras operações custeadas pela mesma Ação.
- **Posição:** a da última carga do SIAFI no Tesouro Gerencial, indicada no topo da página. Não é tempo real.

## Atualização

Automática, em dias úteis. Os relatórios do Tesouro Gerencial chegam por envio agendado depois da carga diária do SIAFI. Cada carga é processada, conferida e publicada aqui sem intervenção manual.

## Conferências antes de publicar

Cada carga só é publicada se passar nestas conferências:

1. **Identidade por UG:** recebido + destaque recebido − concedido − empenhado = disponível, no centavo, em todas as UG.
2. **Empenhos:** o total do relatório de empenhos é igual ao empenhado do relatório de créditos.
3. **Saldo por NC:** a soma dos saldos por Nota de Crédito é igual ao crédito disponível de cada UG e Plano Interno.
4. **Leiaute:** os relatórios têm as colunas esperadas.

Se alguma falhar, o site continua na posição anterior.

## Como ler os números

- **Saldo por NC — exato × estimado:** o saldo é **exato** quando todo empenho da UG cita a NC de origem no histórico. Quando não cita, o empenho é rateado da NC mais antiga para a mais nova, e o saldo aparece como **estimado**.
- **Teto:** valor da NC menos o empenho que a cita e o recolhimento vinculado a ela. O saldo real não passa do teto.
- **Prazo de empenho:** lido do texto da NC ("empenhar até…", "prazo de empenho…", "imediato"). NC sem prazo escrito aparece como "sem prazo".

## Limites

Este painel é **ferramenta de acompanhamento, não fonte oficial**. Em qualquer divergência, prevalece o Tesouro Gerencial e o SIAFI. Os CPF que aparecem em históricos de empenho são mascarados antes da publicação.

## Responsável

D10 — Finanças, Op CATRIMANI II.

## Repositório

Contém apenas o `index.html` do site, com os dados embutidos, e este README. Os arquivos brutos do Tesouro Gerencial **não** são publicados aqui.
