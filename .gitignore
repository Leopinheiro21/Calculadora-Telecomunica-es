import math

def calculadora_telecom():
    while True:
        print("\n--- Calculadora para Telecomunicações ---")
        print("1. Soma")
        print("2. Subtração")
        print("3. Multiplicação")
        print("4. Divisão")
        print("5. Potência")
        print("6. Raiz Quadrada")
        print("7. Logaritmo")
        print("8. Logaritmo de Base 10")
        print("9. Seno")
        print("10. Coseno")
        print("11. Tangente")
        print("12. Conversão de dB para Linear")
        print("13. Conversão de Linear para dB")
        print("14. Derivada")
        print("15. Integral (Aproximação)")
        print("16. Calcular Velocidade da Onda (v = f * λ)")
        print("17. Calcular Comprimento de Onda (λ = v / f)")
        print("18. Calcular Frequência da Onda (f = v / λ)")
        print("19. Sair")

        escolha = input("Escolha a operação (1-19): ")

        if escolha == '19':
            print("Saindo da calculadora. Obrigado!")
            break

        if escolha in ['1', '2', '3', '4', '5']:
            num1 = float(input("Digite o primeiro número: "))
            num2 = float(input("Digite o segundo número: "))

        if escolha == '1':
            print(f"Resultado: {num1 + num2}")
        elif escolha == '2':
            print(f"Resultado: {num1 - num2}")
        elif escolha == '3':
            print(f"Resultado: {num1 * num2}")
        elif escolha == '4':
            if num2 != 0:
                print(f"Resultado: {num1 / num2}")
            else:
                print("Erro: Divisão por zero!")
        elif escolha == '5':
            print(f"Resultado: {num1 ** num2}")
        elif escolha == '6':
            num = float(input("Digite o número para raiz quadrada: "))
            print(f"Resultado: {math.sqrt(num)}")
        elif escolha == '7':
            num = float(input("Digite o número para logaritmo: "))
            print(f"Resultado: {math.log(num)}")
        elif escolha == '8':
            num = float(input("Digite o número para logaritmo de base 10: "))
            print(f"Resultado: {math.log10(num)}")
        elif escolha == '9':
            num = float(input("Digite o ângulo em radianos para seno: "))
            print(f"Resultado: {math.sin(num)}")
        elif escolha == '10':
            num = float(input("Digite o ângulo em radianos para coseno: "))
            print(f"Resultado: {math.cos(num)}")
        elif escolha == '11':
            num = float(input("Digite o ângulo em radianos para tangente: "))
            print(f"Resultado: {math.tan(num)}")
        elif escolha == '12':
            num = float(input("Digite o valor em dB: "))
            print(f"Resultado (Linear): {10 ** (num / 10)}")
        elif escolha == '13':
            num = float(input("Digite o valor linear: "))
            if num > 0:
                print(f"Resultado (dB): {10 * math.log10(num)}")
            else:
                print("Erro: Valor linear deve ser positivo!")
        elif escolha == '14':
            # Derivada: Aqui usaremos uma aproximação simples
            x = float(input("Digite o valor de x para calcular a derivada: "))
            h = 1e-5  # pequeno incremento para calcular a derivada numerica
            func = lambda x: x**2  # Exemplo de função f(x) = x^2
            derivada = (func(x + h) - func(x)) / h
            print(f"Derivada aproximada em {x} é: {derivada}")
        elif escolha == '15':
            # Integral: Aproximação numérica simples (Regra do Trapézio)
            a = float(input("Digite o limite inferior da integral: "))
            b = float(input("Digite o limite superior da integral: "))
            n = int(input("Digite o número de subdivisões: "))
            func = lambda x: x**2  # Exemplo de função f(x) = x^2
            h = (b - a) / n
            integral = 0.5 * (func(a) + func(b))  # Primeiro e último ponto
            for i in range(1, n):
                integral += func(a + i * h)
            integral *= h
            print(f"Integral aproximada de {a} a {b} é: {integral}")
        elif escolha == '16':
            f = float(input("Digite a frequência (Hz): "))
            lambda_ = float(input("Digite o comprimento de onda (m): "))
            v = f * lambda_
            print(f"A velocidade da onda é: {v} m/s")
        elif escolha == '17':
            v = float(input("Digite a velocidade da onda (m/s): "))
            f = float(input("Digite a frequência (Hz): "))
            lambda_ = v / f
            print(f"O comprimento de onda é: {lambda_} m")
        elif escolha == '18':
            v = float(input("Digite a velocidade da onda (m/s): "))
            lambda_ = float(input("Digite o comprimento de onda (m): "))
            f = v / lambda_
            print(f"A frequência da onda é: {f} Hz")
        else:
            print("Opção inválida. Tente novamente.")

if __name__ == "__main__":
    calculadora_telecom()
