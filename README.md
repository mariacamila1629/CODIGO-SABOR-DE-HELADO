# Title: CODIGO-SABOR-DE-HELADO
## DESCRIPCION:
## This program is a small ice cream flavor survey.
## The results are displayed at the end of the program.
## The program asks users to choose a flavor.
## The code counts how many times each flavor is chosen.
## The program shows the results after five customers answer.
## The program is asking customers about their favorite ice cream.
### How it works:
1. First, three counters (chocolate, vanilla, strawberry) are created, starting from 0, to record how many times each flavor is chosen.
2. Then, a for loop is used, repeating 5 times, representing the 5 customers.
3. Display customer number: In each iteration, the program shows the current customer number.
4. Ask for input: The user is prompted to enter a flavor (chocolate, vanilla, or strawberry).
5. Clean input: The program removes extra spaces using strip() and converts the text to lowercase using lower() to standardize the input.
6. Check flavor choice: Using if, elif, and else statements, the program determines which flavor the customer chose and increments the corresponding counter.
7. Handle invalid input: If the entered flavor is not recognized, the program displays a message saying it is invalid.
8. Show results: After all customers have answered, the program displays the total number of times each flavor was chosen.
9. ## Results

chocolate = 0
vainilla = 0
fresa = 0

for i in range(1, 6):
    print(f"/nCliente {i}")
    sabor = input("ELige un sabor (chocolate / vainilla / fresa): ").strip().lower()

    if sabor == "chocolate":
        vainilla += 1
    elif sabor == "vainilla":
        chocolate += 1
    elif sabor == "fresa":
        fresa += 1
    else:
        print("Sabor no valido, no se conto")

print("\n---Resultados---")
print(f"chocolate: {chocolate} veces")
print(f"vainilla:  {vainilla} veces")
print(f"fresa:     {fresa} veces")
