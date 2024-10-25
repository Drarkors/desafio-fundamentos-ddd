# Entidades de domínio

-> Produto
  ->> id
  
-> Tamanho
-> Cor


-> Venda
  -> Item da Venda

-> Ordem de compra
-> Compra
-> Items da Compra

-> Movimentação de estoque
-> Estoque de Produto
  ->> Quantidade mínima

-> Fornecedor

-> Alerta (registros temporários)


# Casos de uso

-> Registro de tamanhos e cores para produtos
-> Registro de produto
-> Edição de produto
-> Remover (logicamente) produto

-> Definir quantidade mínimas de estoque para produtos

-> Alertar quando um produto estiver com essa quantidade mínima (ou menos)
  ->> Gerar notificação
  ->> Gerar email 
  ->> Gerar ordem de compra (automaticamente)

-> Venda de produtos
  ->> Gerar movimentação de saída do estoque

-> Registrar fornecedor
-> Editar fornecedor

-> Gerar ordem de compra (manual)

-> Verificar ordems de compra
  -> Compra de produtos (automática)
    ->> Integrar com fornecedor(es) e gerar remessas para rastreio
    ->> Gerar movimentação de entrada do estoque

-> Compra de produtos (manual)
  -> Integrar com fornecedor(es) e gerar remessas para rastreio
  -> Gerar movimentação de entrada do estoque

-> Vendas e seus produtos por intervalo de tempo
-> Lucro gerado por produto
-> Produtos mais vendidos (recentemente, normalmente no mês)
-> Produtos mais vendidos em um período