VALOR_IA — SISTEMA DE COTAÇÃO POR LINK — V6

OBJETIVO
O WhatsApp envia apenas um convite curto. O fornecedor abre um formulário, preenche marca, código da marca, descrição, preço e disponibilidade. O painel da oficina atualiza em tempo real.

ARQUIVOS
- index.html: painel do administrador/oficina
- fornecedor.html: formulário público do fornecedor
- firebase-config.js: configuração do Firebase
- firebase-rtdb-rules.json: regras do Realtime Database

PASSO 1 — FIREBASE
1. Acesse console.firebase.google.com
2. Crie um projeto.
3. Crie um Web App no projeto.
4. Copie a configuração firebaseConfig.
5. Ative Authentication > Sign-in method > Email/Password.
6. Crie um usuário admin com e-mail e senha.
7. Ative Realtime Database.
8. Em Rules/Regras, cole o conteúdo de firebase-rtdb-rules.json e publique.

PASSO 2 — CONFIGURAÇÃO
Opção mais simples:
- Abra index.html no GitHub Pages.
- Cole a configuração do Firebase na tela inicial do sistema.
- O sistema vai salvar no seu navegador e gerar links de fornecedor com a configuração embutida.

Opção mais limpa:
- Abra firebase-config.js.
- Substitua COLE_AQUI pela configuração real do Firebase.
- Suba os arquivos para o GitHub Pages.

PASSO 3 — GITHUB PAGES
Suba estes arquivos no repositório:
- index.html
- fornecedor.html
- firebase-config.js

Seu link ficará parecido com:
https://tsvalencio-ia.github.io/valor_IA/

PASSO 4 — USO
1. Abra o painel.
2. Entre com o e-mail e senha do administrador criados no Firebase Auth.
3. Cadastre fornecedor.
4. Importe a planilha XLSX.
5. O sistema importa SOMENTE linhas PEÇA / CÓD.
6. Gere link para o fornecedor.
7. Envie o convite pelo WhatsApp.
8. O fornecedor responde pelo formulário.
9. O painel mostra o melhor preço em tempo real.

IMPORTAÇÃO
Este importador foi feito para a planilha no formato:
Coluna B: PEÇA / CÓD.
Coluna D: DESCRIÇÃO
Coluna E: QTD
Coluna F: UNITÁRIO
Coluna G: DESCONTO
Coluna H: TOTAL

Serviços são ignorados automaticamente.

IMPORTANTE
A configuração Web do Firebase não é senha. A segurança depende das regras do Realtime Database e do Firebase Auth.
