VALOR_IA COTAÇÃO V8 — SISTEMA PRONTO

Esta versão já vem com o Firebase configurado em firebase-config.js.
O index.html abre direto no sistema. Não existe mais tela para colar configuração.

ARQUIVOS PARA SUBIR NO GITHUB PAGES
- index.html
- fornecedor.html
- firebase-config.js
- firebase-rtdb-rules.json
- firebase-rtdb-rules-TESTE_FUNCIONA_AGORA.json

COMO INSTALAR NO SEU REPOSITÓRIO valor_IA
1. Extraia este ZIP.
2. Copie os arquivos para a raiz do repositório valor_IA.
3. Suba no GitHub.
4. Abra:
   https://tsvalencio-ia.github.io/valor_IA/index.html

CONFIGURAÇÃO DO FIREBASE
1. Firebase Console > Realtime Database.
2. Rules.
3. Para teste imediato, cole o conteúdo de:
   firebase-rtdb-rules-TESTE_FUNCIONA_AGORA.json
4. Publique.

ATENÇÃO SOBRE SEGURANÇA
As regras de teste deixam leitura/escrita aberta para validar o sistema agora.
Depois que o fluxo estiver aprovado, precisa fechar as regras com login/admin e token por fornecedor.

COMO USAR
1. No painel, cadastre fornecedores.
2. Para fornecedor que cota tudo, coloque tipos:
   todas as peças
3. Importe a planilha XLSX.
4. O sistema importa somente linhas PEÇA / CÓD. e ignora SERVIÇO.
5. Crie a cotação online.
6. Clique em Gerar convite WhatsApp para o fornecedor.
7. Envie a mensagem curta no WhatsApp.
8. O fornecedor abre o formulário, responde e salva.
9. O painel atualiza automaticamente em tempo real.

CAMPOS DO FORNECEDOR
- Tenho / Não tenho
- Marca
- Código da marca ou referência
- Descrição do vendedor
- Preço unitário
- Disponibilidade / prazo
- Observação

IMPORTAÇÃO DA PLANILHA I52203
A lógica correta espera importar 34 peças e ignorar serviços.
Ela usa apenas linhas onde a coluna ITEM / CÓDIGO começa com PEÇA e contém CÓD.
