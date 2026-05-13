VALOR_IA COTAÇÃO V9 — SISTEMA COMPLETO

O QUE TEM NESTA VERSÃO
1. Sistema web para GitHub Pages.
2. Firebase Realtime Database já configurado no arquivo firebase-config.js.
3. Importação de planilha XLSX somente com linhas PEÇA / CÓD.
4. Serviços são ignorados.
5. Formulário do fornecedor por link.
6. Cálculo de melhor preço, venda unitária, custo de compra e lucro por peça.
7. Transformação dos vencedores em Ordem de Compra.
8. Exportação XLSX do comparativo e da ordem de compra.
9. Importação de planilha gerada pelo próprio sistema.
10. Robô local opcional para enviar convites pelo WhatsApp Web automaticamente.
11. Cores suaves para usar o dia todo.

COMO SUBIR NO GITHUB PAGES
1. Extraia o ZIP.
2. Suba para a raiz do repositório valor_IA estes arquivos:
   - index.html
   - fornecedor.html
   - firebase-config.js
   - firebase-rtdb-rules-TESTE_FUNCIONA_AGORA.json
   - firebase-rtdb-rules-PRODUCAO_BASE.json
3. Não suba a pasta inteira dentro de outra pasta.
4. Abra:
   https://tsvalencio-ia.github.io/valor_IA/index.html?v=9

REGRAS DO FIREBASE PARA TESTE
No Firebase > Realtime Database > Rules, cole o conteúdo de:
firebase-rtdb-rules-TESTE_FUNCIONA_AGORA.json

Depois que tudo funcionar, troque pelas regras de produção base e ajustamos segurança.

COMO TESTAR DO ZERO
1. Abra o index.html publicado no GitHub Pages.
2. Vá em Fornecedores e cadastre um fornecedor.
   Exemplo:
   Nome: FURLAN AUTO PEÇAS
   WhatsApp: 17997631210
   Tipos: todas as peças
3. Vá em Importar planilha.
4. Coloque o número da OS, exemplo I52203.
5. Escolha a planilha XLSX.
6. Clique em Importar somente PEÇAS.
7. Confira a prévia. Para I52203, deve importar 34 peças e ignorar serviços.
8. Clique em Criar cotação online.
9. Volte ao Painel.
10. Na cotação, gere o link do fornecedor ou clique em Abrir formulário.
11. Preencha algumas peças no formulário.
12. Volte ao painel. Ele deve mostrar melhor preço e lucro por peça.
13. Clique em Transformar vencedores em Ordem de Compra.
14. Vá em Ordens de compra e exporte XLSX.

ROBÔ WHATSAPP
O robô está na pasta robo-whatsapp.
Ele é opcional. O sistema web funciona sem ele.

Para usar:
1. Abra a pasta robo-whatsapp.
2. Clique em CLIQUE_AQUI_INSTALAR_E_ABRIR_ROBO.bat.
3. Escaneie o QR Code.
4. No painel web, clique em Enviar convite com robô.
5. O robô envia o convite que estiver na fila.

INSTALAR PARA ABRIR AO LIGAR O COMPUTADOR
Dentro da pasta robo-whatsapp, clique em:
INSTALAR_ROBO_INICIAR_COM_WINDOWS.bat

Atenção: o robô só abre depois que o Windows entrar no usuário. Se o WhatsApp desconectar, escaneie o QR Code novamente.

LIMITE
O robô tem limite local de 100 mensagens por dia.
Use somente com fornecedores cadastrados e conhecidos. Não use para propaganda ou disparo em massa.
