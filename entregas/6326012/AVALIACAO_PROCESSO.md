# Ficha de Avaliação de Processo (PDD) — Questão 5

**Cenário escolhido:** A

1. **Nome do processo e descrição resumida:**
   Arquivamento de comprovantes PDF. Renomeação e arquivamento diário de comprovantes em PDF. O robô lê a data
   e o número do documento no nome do arquivo, renomeia o arquivo pela regra
   fixa e o move para a pasta de arquivo.

2. **Volume / frequência estimados:**
   Diário, cerca de 200 arquivos por dia.

3. **As entradas são estruturadas?** (sim/não + justificativa)
   Sim. A data e o número do documento vêm no nome do arquivo, em padrão fixo.

4. **As regras são claras e determinísticas?** (sim/não + justificativa)
   Sim. A regra de nomenclatura é fixa e não exige julgamento humano. A mesma
   entrada gera sempre a mesma saída.

5. **Veredito — o processo é elegível a RPA?** (justifique com base em regras
   claras, dados estruturados e repetibilidade)

   Sim. O processo atende aos três critérios:
   - **Regras claras (item 4):** a nomenclatura é fixa e determinística.
   - **Dados estruturados (item 3):** a data e o número vêm no nome do
     arquivo, em padrão previsível.
   - **Repetibilidade (item 2):** a tarefa se repete todo dia, com cerca de
     200 arquivos.

   Se o nome de um arquivo estiver fora do padrão, o robô registra o caso no
   log e move o arquivo para uma pasta de exceções, para revisão humana. Assim
   o processo continua sem travar.
