# 🏧 Caixa Eletrônico em Python

Este projeto é uma simulação simples de um **caixa eletrônico**, que entrega notas de dinheiro conforme o valor solicitado. Ideal para quem está começando em Python e quer praticar **lógica de programação** e **estrutura de repetição**! 💡🐍

---

## 💻 Sobre o Programa

🔹 O usuário informa o valor que deseja sacar.  
🔹 O programa calcula quantas notas de cada valor são necessárias.  
🔹 Sempre começa pelas **notas de maior valor** para **minimizar a quantidade de cédulas**.  
🔹 O valor é decomposto nas notas disponíveis: `R$100`, `R$50`, `R$20`, `R$10` e `R$5`.  

---

## 🎯 Exemplo de Funcionamento

Se o usuário quiser sacar **R$180**, o programa irá:

Sacando R$ 180...

1 nota(s) de R$ 100

1 nota(s) de R$ 50

1 nota(s) de R$ 20

1 nota(s) de R$ 10

---

✅ Saque realizado com o menor número de notas possível!

---

## 🧠 Lógica Utilizada

1. Define uma lista com os valores das notas disponíveis.
2. Para cada nota:
   - Verifica quantas podem ser entregues.
   - Atualiza o valor restante do saque.
3. Repete até que todo o valor seja "entregue".

---


✅ Saque realizado com o menor número de notas possível!

---

## 🧠 Lógica Utilizada

1. Define uma lista com os valores das notas disponíveis.
2. Para cada nota:
   - Verifica quantas podem ser entregues.
   - Atualiza o valor restante do saque.
3. Repete até que todo o valor seja "entregue".

---

## 📜 Código Fonte

```python
def saca_dinheiro(valor):
    notas = [100, 50, 20, 10, 5]
    print(f"Sacando R$ {valor}...")
    for nota in notas:
        quantidade = valor // nota
        if quantidade > 0:
            print(f"{quantidade} nota(s) de R$ {nota}")
            valor %= nota

valor_saque = int(input("Digite o valor do saque: "))
saca_dinheiro(valor_saque)











