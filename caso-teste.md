# Casos de Teste - Cadastro de Aluno no EduConnect

Este arquivo contém os cenários de teste para validar o processo de cadastro de alunos na plataforma **EduConnect**.

## Cenários de Teste

### ✅ Cenário Positivo 1 - Cadastro com Idade Válida

**ID:** CT001  
**Descrição:** Realizar o cadastro de um aluno com idade dentro da faixa permitida (16 a 80 anos).  
**Pré-condições:** O usuário está na página de cadastro da plataforma.  

**Passos:**  
1. Digitar o nome completo: "Ana Souza"  
2. Inserir o e-mail: "ana@email.com"  
3. Informar a data de nascimento: "2000-05-10" (24 anos)  
4. Criar a senha: "senha123"  
5. Marcar o checkbox "Aceito os termos de uso"  
6. Clicar no botão "Cadastrar"  

**Resultado Esperado:** O sistema exibe a mensagem "Cadastro realizado com sucesso" e salva os dados no banco de dados.

---

### ✅ Cenário Positivo 2 - Cadastro com Senha Válida

**ID:** CT002  
**Descrição:** Realizar o cadastro de um aluno com a senha válida contendo mais de 6 caracteres.  
**Pré-condições:** O usuário está na página de cadastro da plataforma.  

**Passos:**  
1. Digitar o nome completo: "Amanda Souza"  
2. Inserir o e-mail: "ana@email.com"  
3. Informar a data de nascimento: "1999-05-10" (25 anos)  
4. Criar a senha: "senhaSegura123"  
5. Marcar o checkbox "Aceito os termos de uso"  
6. Clicar no botão "Cadastrar"  

**Resultado Esperado:** O sistema exibe a mensagem "Cadastro realizado com sucesso" e salva os dados no banco de dados.

---

### ✅ Cenário Positivo 3 - Campo Nome Válido

**ID:** CT003  
**Descrição:** O campo nome deve ter entre 3 e 50 caracteres.  
**Pré-condições:** O usuário está na página de cadastro da plataforma.  

**Passos:**  
1. Digitar o nome completo: "Luís Carlos" (nome com 10 caracteres, válido dentro da faixa permitida)  
2. Inserir o e-mail: "luis@email.com"  
3. Informar a data de nascimento: "1998-05-10" (26 anos)  
4. Criar a senha: "senhanova321"  
5. Marcar o checkbox "Aceito os termos de uso"  
6. Clicar no botão "Cadastrar"  

**Resultado Esperado:** O sistema exibe a mensagem "Cadastro realizado com sucesso" e salva os dados no banco de dados.

---

### ❌ Cenário Negativo 1 - Campo Nome Inválido

**ID:** CT004  
**Descrição:** Validar que o sistema não permite o cadastro de um nome com menos de 3 ou mais de 50 caracteres.  
**Pré-condições:** O usuário está na página de cadastro da plataforma.  

**Passos:**  
1. Digitar o nome completo: "Ka" (nome com menos de 3 caracteres)  
2. Inserir o e-mail: "ka@email.com"  
3. Informar a data de nascimento: "2000-12-10" (24 anos)  
4. Criar a senha: "senhaka321"  
5. Marcar o checkbox "Aceito os termos de uso"  
6. Clicar no botão "Cadastrar"  

**Resultado Esperado:** O sistema exibe a mensagem "Nome inválido".

---

### ❌ Cenário Negativo 2 - Idade Inválida

**ID:** CT005  
**Descrição:** Validar que o sistema não permite o cadastro de pessoas com menos de 16 ou mais de 80 anos.  
**Pré-condições:** O usuário está na página de cadastro da plataforma.  

**Passos:**  
1. Digitar o nome completo: "Carolina Santos"  
2. Inserir o e-mail: "Carolinasantos@email.com"  
3. Informar a data de nascimento: "2011-10-11" (14 anos, idade inválida)  
4. Criar a senha: "senhaminha210"  
5. Marcar o checkbox "Aceito os termos de uso"  
6. Clicar no botão "Cadastrar"  

**Resultado Esperado:** O sistema exibe a mensagem "Idade inválida" e impede o cadastro.

---

### ❌ Cenário Negativo 3 - Senha Inválida

**ID:** CT006  
**Descrição:** Validar que o sistema não permite o cadastro com senha de menos de 6 caracteres.  
**Pré-condições:** O usuário está na página de cadastro da plataforma.  

**Passos:**  
1. Digitar o nome completo: "Susan Almeida"  
2. Inserir o e-mail: "Susanalmeida@email.com"  
3. Informar a data de nascimento: "2001-01-06" (23 anos)  
4. Criar a senha: "senha" (senha com menos de 6 caracteres)  
5. Marcar o checkbox "Aceito os termos de uso"  
6. Clicar no botão "Cadastrar"  

**Resultado Esperado:** O sistema exibe a mensagem "Senha inválida".

