# Analista de Dados - MaisTODOS

Hoje na maisTODOS temos rodando um motor de recorrencia, onde todas as cobranças de mensalidades dos projetos do grupo são executadas e realizadas, com inteligência de retentativas, melhor dia de pagamento, melhor tipo de pagamento, codigos mais retornados, etc.

![image](https://user-images.githubusercontent.com/3420133/143287102-cc146909-84f7-40ca-8571-486aedbb40b7.png)

Dicionário de dados
===================
- subscription: id da assinatura
- cycle_id: ciclo da assinatura
- cycle_starts_at: inicio do periodo de pagamento
- cycle_ends_at: final do periodo de pagamento
- payment_date: data do pagamento
- payment_code: codigo do pagamento
- payment_attempt: numero da retentativa 1,2,3,4,5,6
- payment_authorized: autorizado
- payment_bin: primeiros numeros do cartao
- payment_processor: processadora cielo, adyen, rede, pagseguro
- payment_amount: valor do pagamento

A base está em CSV, neste link:
https://github.com/MaisTodos/data-analytics-challenge/blob/main/teste_tecnico.csv.zip


Problemas
=========

1 - Analisado os dias de pagamentos com mais conversões (transação autorizada), qual é o melhor dia de conversão?

2 - Quantas conversões ocorrem por mês?

3 - Qual foi a arrecadação de todas a retentivas por mês? (`payment_atttempt > 1`)

4 - Considerando as taxas: cielo com `0.05`, a rede `0.065`, adyen `0.123`, pagseguro `0.04`. Qual processadora é mais rentável para o sistema considerando valor arrecadado e pago?

5 - Qual foi a retentativa (`payment_attempt > 1`) e processadora que mais converteram?

6 - Qual foi o `payment_code` com maior aprovação em retentativas?

7 - Qual foi o `payment_code` com menor aprovação em retentativas?

8 - Analisado os números de retentativas, qual é o melhor dia de pagamento por quantidade de retentativas?



Pontos de Atenção
=================

A resolução deve ser entregue da forma que preferir, mais recomendamos fortemente utilizar o **jupyter** (https://jupyter.org/). É interessante documentar de forma  que o time consiga refazer os passos para a resolução.
Fique livre para nos contatar em caso de dúvidas, sugestões ou problemas encontrados.


Boa sorte, Equipe MaisTodos!

![Luck](https://media.giphy.com/media/l49JHz7kJvl6MCj3G/giphy.gif)
