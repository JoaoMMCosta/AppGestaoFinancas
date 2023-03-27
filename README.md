# AppGestaoFinancas
Ficha 4 - Engenharia de Softwear - 2022/2023


Levanatmento de Requisitos:

   01-->permitir adicionar JanelaAddUtilizador (e-mail, nome, password)
   02-->permitir adicionar JanelaAddDespesa (data, valor, categoria)
   03-->permitir adicionar JanelaAddReceita (data, valor, categoria)
   04-->permitir remover JanelaAddUtilizador
   05-->permitir remover JanelaAddDespesa
   06-->permitir remover JanelaAddReceita
   07-->permitir editar JanelaAddDespesa (data, valor, categoria)
   08-->permitir editar JanelaAddReceita (data, valor, categoria)
   09-->permitir ver movimentos por data/tipo/categoria
   10-->permitir criar categorias
   11-->permitir adicionar objetivos
   



Especificação de Requisitos:

-->Permitir adicionar despesas:
    1. O utilizador, no menu principal, clica no botão "Adicionar Despensa";
    2. O sistema mostra a janela "Adicionar Despensa";
    3. O utilizador preenche todos os campos valor, data, Descrição "Guardar";
    3.1. O utilizador clica em "Cancelar";
    3.1.1 O sistema fecha a janela "Adicionar Despensa", regressando à janela "Principal";
    3.2. O utilizador insere um montante negativo ou igual a zero;
    3.2.1. O sistema apresenta a mensagem erro "O montante tem de ser positivo";
    3.3. O utilizador insere um montante superior ao saldo atual;
    3.3.1. O sistema apresenta a mensagem erro "Valor da despesa não deve ser superior ao saldo atual";
    3.4. O utilizador insere uma data diferente do formato "dd-mm-yyyy";
    3.4.1. O sistema apresenta a mensagem erro "Formato de data inválido";
    3.5. O utilizador insere uma data superior à data atual;
    3.5.1. O sistema apresenta a mensagem erro "A data tem de ser inferior à data atual";
    4. O sistema valida que o montante é um valor decimal positivo, inferior ao saldo atual, que a categoria pertence à lista de categorias no sistema, e que a data é válida, inferior à data atual e está no formato "dd-mm-yyyy", edita a despesa, fecha a janela "Editar JanelaAddDespesa", regressando à janela principal, mostrando a mensagem de sucesso "JanelaAddDespesa Editada".

-->Permitir adicionar receitas
    1. O utilizador, no menu principal, clica no botão "Adicionar JanelaAddReceita";
    2. O O sistema mostra a janela "Adicionar JanelaAddReceita";
    3. O utilizador preenche todos os campos valor, data, Descrição "Guardar";
    3.1. O utilizador clica em "Cancelar";
    3.1.1. O sistema fecha a janela "Adicionar JanelaAddReceita", regressando à janela "Movimentos";
    3.2. O utilizador insere um montante negativo ou igual a zero;
    3.2.1. O sistema apresenta a mensagem erro "O montante tem de ser positivo";
    3.3. O utilizador insere uma data diferente do formato "dd-mm-yyyy";
    3.3.1. O sistema apresenta a mensagem erro "Formato de data inválido";
    3.4. O utilizador insere uma data superior à data atual;
    3.4.1. O sistema apresenta a mensagem erro "A data tem de ser inferior à data atual";
    4. O sistema valida que o montante é um valor decimal positivo, que a categoria pertence à lista de categorias no sistema, e que a data é válida, inferior à data atual e está no formato "dd-mm-yyyy", edita a receita, fecha a janela "Editar JanelaAddReceita", regressando à janela principal, mostrando a mensagem de sucesso "JanelaAddReceita Editada".

-->Permitir remover despesa:
    1. O utilizador carrega em "Despesas" na janela principal;
    2. O sistema mostra a janela "Despesas";
    3. O utilizador carrega no botão "Remover" da despesa a retirar;
    4. O sistema mostra uma janela "Remover JanelaAddDespesa";
    5. O utilizador confirma a remoção da despesas;
    5.1. O utilizador recusa a remoção da despesas;
    5.1.1. O sistema confirma recusa com uma mensagem de remoção não realizada e retorna à janela "Remover Despesas";
    6. O sistema confirma a remoção com uma mensagem de sucesso e retorna à janela "Remover Despesas".

-->Permitir remover receita:
    1. O utilizador carrega em "Receitas" na janela principal;
    2. O sistema mostra a janela "Receitas";
    3. O utilizador carrega no botão "Remover" da JanelaAddReceita a retirar;
    4. O sistema mostra uma janela "Remover JanelaAddReceita";
    5. O utilizador confirma a remoção da receita;
    5.1. O utilizador recusa a remoção da receita;
    5.1.1. O sistema confirma recusa com uma mensagem de remoção não realizada e retorna à janela "Remover JanelaAddReceita";
    6. O sistema confirma a ação com uma mensagem de sucesso e retorna à janela "Remover Receitas".

-->Permitir editar despesas:
    1. O utilizador, no menu principal, clica em "Movimentos";
    2. O sistema mostra a janela "Movimentos" com todos os movimentos;
    3. O utilizador clica no botão "Editar" da despesa que pertende editar;
    4. O sistema mostra a janela "Editar JanelaAddDespesa";
    5. O utilizador altera o valor do montante, data e categoria e clica em "Confirmar";
    5.1. O utilizador clica em "Cancelar";
    5.1.1. O sistema fecha a janela "Editar JanelaAddDespesa", regressando à janela "Movimentos";
    5.2. O utilizador insere um montante negativo ou igual a zero;
    5.2.1. O sistema apresenta a mensagem erro "O montante tem de ser positivo";
    5.3. O utilizador insere um montante superior ao saldo atual;
    5.3.1. O sistema apresenta a mensagem erro "O valor da despesa não deve ser superior ao saldo atual";
    5.4. O utilizador insere uma data diferente do formato "dd-mm-yyyy";
    5.4.1. O sistema apresenta a mensagem erro "Formato de data inválido";
    5.5. O utilizador insere uma data superior à data atual;
    5.5.1. O sistema apresenta a mensagem erro "A data tem de ser inferior à data atual";
    6. O sistema valida que o montante é um valor decimal positivo, inferior ao saldo atual, que a categoria pertence à lista de categorias no sistema, e que a data é válida, inferior à data atual e está no formato "dd-mm-yyyy", edita a despesa, fecha a janela "Editar JanelaAddDespesa", regressando à janela principal, mostrando a mensagem de sucesso "JanelaAddDespesa Editada".

-->Permitir editar receitas:
    1. O utilizador, no menu principal, clica em "Movimentos";
    2. O sistema mostra a janela "Movimentos" com todos os movimentos;
    3. O utilizador clica no botão "Editar" da receita que pertende editar;
    4. O sistema mostra a janela "Editar JanelaAddReceita";
    5. O utilizador altera o valor do montante, data e categoria e clica em "Confirmar";
    5.1. O utilizador clica em "Cancelar";
    5.1.1. O sistema fecha a janela "Editar JanelaAddReceita", regressando à janela "Movimentos";
    5.2. O utilizador insere um montante negativo ou igual a zero;
    5.2.1. O sistema apresenta a mensagem erro "O montante tem de ser positivo";
    5.3.O utilizador insere uma data diferente do formato "dd-mm-yyyy";
    5.3.1. O sistema apresenta a mensagem erro "Formato de data inválido";
    5.4. O utilizador insere uma data superior à data atual;
    5.4.1. O sistema apresenta a mensagem erro "A data tem de ser inferior à data atual";
    6. O sistema valida que o montante é um valor decimal positivo, que a categoria pertence à lista de categorias no sistema, e que a data é válida, inferior à data atual e está no formato "dd-mm-yyyy", edita a receita, fecha a janela "Editar JanelaAddReceita", regressando à janela principal, mostrando a mensagem de sucesso "JanelaAddReceita Editada".
