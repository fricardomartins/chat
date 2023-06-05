# chat
Chat em Python simples
Aqui está um exemplo básico de um chat de usuário em Python:

```python
def enviar_mensagem():
    mensagem = input("Digite a mensagem: ")
    return mensagem

def receber_mensagem(mensagem):
    print("Usuário: ", mensagem)

def main():
    print("Bem-vindo ao chat de usuário!")

    while True:
        # Usuário envia uma mensagem
        mensagem_enviada = enviar_mensagem()

        # Encerrar o chat se o usuário digitar "sair"
        if mensagem_enviada.lower() == "sair":
            print("Chat encerrado.")
            break

        # Simula a resposta do sistema
        # Você pode adicionar lógica aqui para processar a mensagem e fornecer uma resposta adequada
        mensagem_resposta = "Olá! Você disse: " + mensagem_enviada

        # Exibir a resposta do sistema
        receber_mensagem(mensagem_resposta)

if __name__ == "__main__":
    main()
```
