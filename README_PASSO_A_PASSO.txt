VALORIA V13.2 - BANCO DE PREÇOS + COTAÇÃO + ROBÔ + ENCERRAR COTAÇÃO

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


NOVIDADES DA V13
- Importação corrigida para dois modelos reais:
  1) linhas com PEÇA / CÓD.
  2) tabela GRADE / CÓDIGO DA PEÇA
- Serviços são ignorados na importação.
- Prévia mostra padrão detectado, linha da planilha, código original, código alternativo, quantidade, valor unitário e total.
- Cabeçalho redesenhado com visual comercial.
- Cadastro do estabelecimento ganhou nicho e ícone editável.
- Nichos prontos: autopeças/oficina, construção, farmácia, agro/pet, informática, mercado, papelaria, restaurante, hotelaria, estética, marcenaria, ferragens, elétrica, hidráulica, limpeza, EPI, eventos, clínicas e transportes.


CORREÇÃO V13.2
- Corrigido travamento da página causado por escrita no Firebase durante a renderização dos botões de fornecedor.
- Links de fornecedor agora são gravados somente quando você clica em Abrir WhatsApp, Copiar mensagem, Enviar com robô ou Abrir formulário.
- Mantida a importação inteligente da V13.

ABRIR COM CACHE LIMPO:
https://tsvalencio-ia.github.io/valor_IA/index.html?v=13.1


NOVIDADES DA V13.2
- Nova opção de criar orçamento/cotação manualmente, sem planilha.
- Cadastro completo dos dados do veículo:
  cliente/referência, marca, modelo, ano, placa, chassi, KM, prefixo/frota e observação.
- Adição manual de peças:
  código original, código alternativo, descrição, quantidade, preço base unitário e tipo.
- Orçamento fica salvo no Firebase com todos os dados do veículo e todas as peças usadas.
- A tela de cotações agora exibe os dados completos do veículo.
- Cada cotação tem uma seção “Peças salvas neste orçamento”.
- Continua importando planilha quando existir.


NOVIDADES DA V13.3
- Corrigido importador para não transformar cabeçalho "DESCRIÇÃO / CÓDIGO DA PEÇA" em peça.
- Formulário do fornecedor redesenhado para ficar mais simples, bonito e agradável.
- O vendedor agora pode responder por cartões interativos com botões rápidos de disponibilidade.
- Admin/cotador agora pode editar orçamentos/cotações existentes.
- Admin/cotador agora pode excluir orçamentos/cotações existentes.
- Cada cotação continua salvando dados completos do veículo e as peças usadas.
- Assinatura mantida: Powered by thIAguinho Soluções Digitais.

ROBÔ WHATSAPP
O robô é sempre o mesmo enquanto o Firebase e a estrutura da fila não mudarem. 
Você não precisa reinstalar o robô em toda atualização do GitHub Pages.
Atualize o robô somente quando houver uma pasta robo-whatsapp nova e a melhoria for específica do robô.


NOVIDADES DA V13.4
- Em cada cotação, o cotador pode selecionar mais de um fornecedor.
- Botão “Enviar selecionados com robô” cria várias mensagens na fila do Firebase.
- Mantém botões de abrir WhatsApp, copiar mensagem e abrir formulário por fornecedor.
- A cotação agora tem seção “Respostas diretas recebidas no WhatsApp”.
- A pasta robo-whatsapp foi atualizada para ler mensagens recebidas no WhatsApp:
  - salva o texto bruto no orçamento;
  - tenta interpretar item, código, marca, código da marca, descrição, preço e disponibilidade;
  - quando consegue, preenche a resposta do item no orçamento;
  - quando não consegue, mantém a mensagem bruta para revisão.

IMPORTANTE SOBRE RESPOSTAS NO WHATSAPP
O formulário por link continua sendo o método mais seguro e organizado.
A leitura de texto livre no WhatsApp é apoio, porque vendedor pode responder de qualquer jeito.

NOVIDADES DA V13.5
- Corrigido problema das áreas que fechavam sozinhas.
- Seleção de fornecedores estável.
- Envio para vários fornecedores de uma vez corrigido.
- Campo novo: WhatsApp do gestor para avisos.
- Robô avisa o gestor pelo WhatsApp quando chega resposta de cotação.
- Resposta bruta do fornecedor fica salva na cotação.
- Link do fornecedor não grava mais no Firebase durante renderização, evitando loop/travamento.

Atualize também a pasta robo-whatsapp nesta versão.
