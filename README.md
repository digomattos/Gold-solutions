#Participantes: Rodrigo Mattos, Pedro Maluli,Bernarndo Bittencurt, Guilherme Lôbo e Roberto Forti.


exemplos = [
    (3500, "Barbosa Iron"),
    (10000, "Dona Maria Ferro"),
    (5000, "JP Ferro"),
]

def compara_valor(valor):
    resultados = []
    for exemplo in exemplos:
        if valor >= exemplo[0]:
            resultados.append(exemplo[1])
    return resultados


valor_recebido = int(input("Qual o orçamento disponivel: "))


resultados = compara_valor(valor_recebido)

 
print(f"Visto o seu orçamento de {valor_recebido} os fornecedores ao seu alcance são: {', '.join(resultados)}")

