 import json
 import os

 ARQUIVO = "usuarios_senha_pura.json"


def carregar_usuarios():



if not os.path.exists(ARQUIVO):
with open (ARQUIVO, "w", encoding="utf-8") as f:
json.dump([], f, ensure_ascii=False, indent=2)

return []

with open (ARQUIVO, "r", encoding="utf-8") as f:

return json.load(f)

 def salvar_usuarios (usuarios):

with open (ARQUIVO, "w", encoding="utf-8") as f:

json.dump(usuarios, f, ensure_ascii=False, indent=2)

 def cadastrar():

usuarios = carregar_usuarios()












usuario input("Novo usuário: ").strip()
if any(u["usuario"] == usuario for u in usuarios):
print("Usuário já existe!")
return
senha = input("Nova senha: ").strip()
usuarios.append({"usuario": usuario, "senha": senha})
salvar_usuarios (usuarios)
print("Cadastrado! (senha salva em texto puro no JSON)")

 def login():




usuarios = carregar_usuarios()
usuario = input("Usuário: ").strip()
senha = input("Senha: ").strip()


for u in usuarios:



if u["usuario"] == usuario:
if u["senha"] == senha:
print("Acesso permitido")



else:
print("Acesso negado")
return

 print("Usuário não encontrado")

 def menu():

while True:




Sair") print("3




cadastrar()


login()


print("\n=== LOGIN (SENHA PURA) ===")
print("1 Cadastrar")
print("2 Login")
op = input("Escolha: ").strip()
if op == "1":
elif op == "2":
elif op == "3":
break

else:

print("Opção inválida.")

 if_name__ == "_main__":
 menu()
