#Feito por Joelliton,João,Isabela Garcia
viaturas = int(input("Quantas viaturas tem no bairro de Jordanópolis? "))
postos = input("Tem policiamento pelo bairro 24h? ")

if viaturas < 5 and postos.lower() == "não":
    print("O bairro não é seguro")
    drones = input("Já consideraram o uso de drones para patrulhamento? (s/n) ")
    if drones.lower() == "não":
        print("Seria interessante patrulhamento de drones para aumentar a segurança.")
elif viaturas > 5 and postos.lower() == "sim":
    print("O bairro é seguro")
elif viaturas > 5 and postos.lower() == "não":
    resposta = int(input("Quantos postos tem sua cidade? "))
    if resposta < 6:
        print("O bairro não é seguro na questão de policiamento")
        drones = input("Já consideraram o uso de drones para patrulhamento? (sim/não) ")
        if drones.lower() == "não":
            print("Seria interessante patrulhamento drones para aumentar a segurança.")
    elif resposta > 6:
        print("Está tudo ok")
else:
    print("O bairro é seguro")
