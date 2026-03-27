# 🚩 Missão 04 - Operação Escudo Digital

### 🛡️ Prevenção de Erros e Robustez

Este projeto foi desenvolvido como parte da disciplina de **Interação Humano-Computador (IHC/UX)** com foco na **5ª Heurística de Nielsen: Prevenção de Erros**.

---

## 💡 Sobre o Projeto

O objetivo deste sistema é evitar que erros simples do usuário (como digitar letras em vez de números) causem falhas no programa.

Em vez de “quebrar” ou mostrar mensagens técnicas confusas, o sistema:

✅ Captura erros com `try-catch`
✅ Exibe mensagens amigáveis
✅ Mantém o programa funcionando
✅ Melhora a experiência do usuário

---

## 🖥️ Tecnologias Utilizadas

* C#
* .NET (Console App)
* Visual Studio Code

---

## ⚙️ Como Executar o Projeto

```bash
cd SistemaRobusto
dotnet run
```

---

## 🧠 Conceito Principal: Try-Catch

O `try-catch` é uma estrutura usada para **tratar erros (exceções)** no código.

### 🔹 Funcionamento:

* `try`: onde o código “arriscado” é executado
* `catch`: captura o erro caso ele aconteça
* `finally`: executa sempre (com erro ou não)

### 💻 Exemplo do projeto:

```csharp
try 
{
    int idade = int.Parse(entrada);
}
catch (FormatException)
{
    Console.WriteLine("Erro: Digite apenas números!");
}
```

👉 Isso evita que o programa feche inesperadamente.

---

## 🚀 Alternativa Profissional: TryParse

Desenvolvedores mais experientes utilizam:

```csharp
int.TryParse(entrada, out idade);
```

✔️ Não gera erro
✔️ Mais eficiente
✔️ Mais limpo

---

## 📸 Evidências

### ✅ Caminho Feliz (Entrada correta)
<img width="890" height="649" alt="image" src="https://github.com/user-attachments/assets/be91afaa-e92b-437e-a93a-3859a8261d71" />


### ❌ Caminho do Erro (Entrada inválida)

<img width="855" height="730" alt="image" src="https://github.com/user-attachments/assets/aa4d9d06-971e-4bf1-8613-eae1f336ef78" />


---

## 🎯 Relação com IHC (UX)

Segundo a **Heurística de Nielsen (Prevenção de Erros)**:

> Um bom sistema evita que erros aconteçam, ao invés de apenas tratá-los.

### 💥 Sem tratamento de erro:

* Programa fecha sozinho
* Usuário fica confuso 😕
* Perda de confiança

### 🛡️ Com tratamento de erro:

* Mensagens claras
* Usuário entende o problema
* Sistema parece mais profissional

---

## 🧠 Reflexão

> Quando o programa “crasha” por um erro simples, o usuário sente frustração, insegurança e perde a confiança no sistema.

Já com mensagens amigáveis:

✨ O usuário se sente orientado
✨ Entende o que fazer
✨ Continua usando o sistema com confiança

---

## 📂 Estrutura do Repositório

```
una-ihcux-lista04/
│
├── SistemaRobusto/
│   ├── Program.cs
│   └── SistemaRobusto.csproj
│
├── evidencia-sucesso.png
├── evidencia-erro.png
└── README.md
```

---

## ✅ Checklist de Entrega

* [x] Repositório público criado
* [x] Tratamento de erro implementado
* [x] Mensagens amigáveis com cores
* [x] Evidências adicionadas
* [x] README completo

---

## 👨‍💻 Autor

Desenvolvido para fins acadêmicos - UNA 💙
