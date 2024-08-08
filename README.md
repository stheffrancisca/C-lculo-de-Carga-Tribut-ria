# C-lculo-de-Carga-Tribut-ria
Cálculo de Carga Tributária

(Lembrando, não se atente ao funcionamento real da carga tributária, é apenas um exemplo imaginário para treinarmos as functions com algo mais prático)

Imagine que você trabalha no setor contábil de uma grande empresa de Varejo. 

Crie uma function que calcule qual o % de carga tributária que está sendo aplicado sobre um determinado produto, dado o preço de venda, o "lucro" e os custos (com exceção do imposto) dele.

preco = 1500
custo = 400
lucro = 785

Repare que preço - custo não é igual ao lucro, porque ainda foi descontado o imposto. Sua functiona deve calcular qual foi o % de imposto aplicado sobre o preço total.

#crie sua function aqui
def carga_tributaria(preco, custo, lucro):
    imposto = preco - custo - lucro
    return imposto / preco

    #aplique sua function nos valores fornecidos para ver se ela está funcionando corretamente
print('A carga tributária foi de {:.1%}'.format(carga_tributaria(preco, custo, lucro)))   
