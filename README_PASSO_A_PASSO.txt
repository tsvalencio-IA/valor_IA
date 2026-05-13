VALORIA V12 - BANCO DE PREÇOS + COTAÇÃO + ROBÔ + ENCERRAR COTAÇÃO

ARQUIVOS PARA SUBIR NO GITHUB PAGES
Suba estes arquivos na raiz do repositório valor_IA:
- index.html
- fornecedor.html
- firebase-config.js
- firebase-rtdb-rules-TESTE_FUNCIONA_AGORA.json
- firebase-rtdb-rules-PRODUCAO_BASE.json
- README_PASSO_A_PASSO.txt

A pasta robo-whatsapp fica no computador da loja. Não precisa subir no GitHub Pages.

COMO TESTAR
1. Abra: https://tsvalencio-ia.github.io/valor_IA/index.html?v=12
2. No Firebase Realtime Database, cole temporariamente as regras de teste.
3. Cadastre o estabelecimento.
4. Cadastre fornecedores.
5. Use o Banco de preços para cadastrar produtos/preços conhecidos.
6. Selecione itens do banco de preços e clique em "Criar cotação de conferência".
7. Envie link ao fornecedor com robô ou WhatsApp manual.
8. O fornecedor preenche o formulário.
9. O painel atualiza e calcula melhores preços/lucro.
10. Clique em "Gerar ordem de compra".
11. Exporte OC em XLSX.

ENCERRAR COTAÇÃO
Na aba Cotações, clique em "Encerrar cotação". O fornecedor que abrir o link verá "Cotação encerrada" e não poderá responder.

BANCO DE PREÇOS
Serve para pesquisar preços já conhecidos e mandar ao fornecedor confirmar:
- se ainda tem disponível
- se o valor continua o mesmo
- marca
- código da marca
- descrição
- disponibilidade

ASSINATURA
Rodapé e planilhas exportadas usam:
Powered by thIAguinho Soluções Digitais
