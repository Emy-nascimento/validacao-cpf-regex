#  Validação de Formato de CPF com Regex e PowerShell

Este projeto apresenta a construção, explicação lógica e testes práticos de uma Expressão Regular (Regex) desenvolvida para validação do formato de CPF (`NNN.NNN.NNN-NN`).


![Demonstração no PowerShell](./Captura%20de%20tela%202026-08-23%20211440.png)

---

## 💻 Tecnologias e Ferramentas Utilizadas
- **Expressões Regulares (Regex)**
- **Windows PowerShell** (Operador `-match`)
  

---

##  Expressão Regular Desenvolvida
```regex
^(\d{3}\.){2}\d{3}-\d{2}$

Detalhamento da Sintaxe:

^ : Âncora de início de linha.

(\d{3}\.){2} : Agrupamento de 3 dígitos numéricos seguidos de ponto literal, repetido exatamente 2 vezes.

\d{3} : Terceiro bloco com 3 dígitos numéricos.

- : Hífen literal.

\d{2} : Bloco final com os 2 dígitos verificadores.

$ : Âncora de fim de linha.


🧪 Como Testar no Terminal (PowerShell)
Para executar o teste de validação no terminal Windows PowerShell:

PowerShell
"110.123.650-10" -match "^(\d{3}\.){2}\d{3}-\d{2}$"
Resultados dos Testes Práticos:
Entradas no formato NNN.NNN.NNN-NN retornam True.
Entradas sem pontos, sem hífen ou com caracteres extras retornam False.

🎥 Demonstração em Vídeo
Confira a explicação detalhada do código e a demonstração prática dos testes no terminal:
👉 Assistir à apresentação em vídeo: https://youtu.be/d9785gEtjzY?si=FTHpaKvqc6L0_IJA




