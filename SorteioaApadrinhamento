import random
import tkinter as tk
from tkinter import messagebox

def sortear_nome(nomes):
    if nomes:
        nome = nomes.pop()
        label_nome.config(text=f"{nome}", fg="white", bg="#4CAF50", font=("Arial", 24, "bold"), width=50, height=5)
    else:
        messagebox.showinfo("Fim", "Todos os nomes já foram sorteados!")

def iniciar_sorteio():
    nomes = ["Alice", "Bob", "Carlos", "Diana", "Eduardo", "Fernanda", "Gabriel", "Helena", "Igor", "Julia"]
    random.shuffle(nomes)
    label_nome.config(text="Clique em 'Sortear Nome'", fg="black", bg="white", font=("Arial", 20), width=50, height=5)
    botao_sortear.config(command=lambda: sortear_nome(nomes))

# Criando a janela principal
root = tk.Tk()
root.title("Sorteio de Nomes")
root.geometry("800x600")
root.configure(bg="#2C3E50")

label_titulo = tk.Label(root, text="Sorteador de Nomes", font=("Arial", 28, "bold"), bg="#2C3E50", fg="white")
label_titulo.pack(pady=20)

label_nome = tk.Label(root, text="Clique em 'Sortear Nome'", font=("Arial", 20), bg="white", width=50, height=5)
label_nome.pack(pady=40)

botao_sortear = tk.Button(root, text="Sortear Nome", font=("Arial", 18, "bold"), bg="#3498DB", fg="white", width=25, height=3)
botao_sortear.pack(pady=20)

botao_reiniciar = tk.Button(root, text="Reiniciar Sorteio", command=iniciar_sorteio, font=("Arial", 18, "bold"), bg="#E74C3C", fg="white", width=25, height=3)
botao_reiniciar.pack(pady=20)

iniciar_sorteio()
root.mainloop()
