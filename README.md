# Mocky

> Um servidor Mock HTTP simples e configurável para facilitar testes e desenvolvimento de APIs.

---

## 📌 O que é o Mocky?
O **Mocky** é um servidor HTTP leve e configurável, feito para ajudar desenvolvedores a **simular APIs locais** quando os serviços reais não estão acessíveis.  

✅ Fácil de configurar (JSON/YAML)  
✅ Simula **status codes personalizados** (200, 400, 500, etc.)  
✅ Permite **delays para testar latência**  
✅ Registra requisições para depuração  
✅ Código open-source sob a licença **GPL-3.0**  

---

## 🚀 **Funcionalidades Planejadas**
🔹 **Configuração via JSON/YAML** – Definir endpoints sem precisar escrever código  
🔹 **Respostas personalizadas** – Status code, headers e body customizados  
🔹 **Simulação de delays e falhas** – Para testar cenários de erro  
🔹 **Registro de requisições** – Logs detalhados para debugging  
🔹 **Interface Web (futuro)** – Para criar mocks dinamicamente via UI  
🔹 **Modo Proxy (futuro)** – Encaminha requisições para a API real quando necessário  

---

## 🏗 **Status do Desenvolvimento**
O Mocky está em fase inicial de desenvolvimento.  

📌 **Etapas atuais:**  
✅ Definição da arquitetura  
✅ Planejamento das principais funcionalidades  
🚧 Implementação inicial em GoLang  
📌 Interface de configuração baseada em JSON/YAML  

Se quiser acompanhar o progresso, fique de olho nos commits e issues! 🛠️  

---

## 📂 **Exemplo de Configuração**
O Mocky permitirá definir endpoints usando um arquivo JSON ou YAML.  

Exemplo (`config.json`):
```json
{
  "endpoints": [
    {
      "method": "GET",
      "path": "/users",
      "response": {
        "status": 200,
        "body": [{ "id": 1, "name": "Alice" }, { "id": 2, "name": "Bob" }]
      }
    },
    {
      "method": "POST",
      "path": "/login",
      "requestBody": { "username": "admin", "password": "1234" },
      "response": {
        "status": 200,
        "body": { "token": "fake-jwt-token" }
      }
    }
  ]
}
```
A ideia é que os devs possam **editar esse arquivo e definir endpoints personalizados rapidamente**.

---

## 💡 **Contribuindo**
Quer ajudar a desenvolver o Mocky?  
1️⃣ Faça um **fork** deste repositório 🍴  
2️⃣ Crie uma branch (`feature/minha-feature`) 🌱  
3️⃣ Faça um **Pull Request** 🚀  

Se tiver ideias ou sugestões, abra uma **issue** no GitHub! 💡  

---

## 📜 **Licença**
Este projeto é distribuído sob a licença **GPL-3.0**.  
Isso significa que o Mocky será sempre **livre e de código aberto**, garantindo que melhorias feitas na comunidade continuem acessíveis para todos.  

🔗 Leia mais sobre a [GPL-3.0](https://www.gnu.org/licenses/gpl-3.0.pt-br.html).
