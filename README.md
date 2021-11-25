# Analista de Dados - MaisTODOS

Hoje na maisTODOS temos rodando um motor de recorrencia, onde todas as cobranças de mensalidades dos projetos do grupo são executadas e realizadas. Com inteligencia de retentativas, melhor dia de pagamento, melhor tipo de pagamento, codigos mais retornados, etc.

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


Problemas
=========

1. Qual o dia de pagamento de melhor conversão (transações autorizadas X total)
2. Qual foi a conversão desses meses? (% de assinaturas com transações autorizadas por periodos (mes))
3. Qual foi a arrecadacao de todas as retentativas(payment_attempt > 1) X periodo (Mes)
4. Considerando as taxas: cielo com 0,05, a rede 0,065, adyen 0,123, pagseguro 0,04. Qual processadora é mais rentável para o sistema considerando valor arrecadado e pago.
5. Qual foi a retentativa(payment_attempt > 1) e processadora que mais converteram.
