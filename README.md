#  Validação de Formato de CPF com Regex e PowerShell

Este projeto apresenta a construção, explicação lógica e testes práticos de uma Expressão Regular (Regex) desenvolvida para validação do formato de CPF (`NNN.NNN.NNN-NN`).




![Demonstração no PowerShell](./Captura%20de%20tela%202026-08-23%20211440.png)

---

## 💻 Tecnologias e Ferramentas Utilizadas
- **Expressões Regulares (Regex)**
- **Windows PowerShell** (Operador `-match`)
- **Git & GitHub**

---

## ⚙️ Expressão Regular Desenvolvida

```regex
^(\d{3}\.){2}\d{3}-\d{2}$
