print('PROGRAMA PARA CALCULAR PERIMETRO DE TRIANGULO')

try:
    lado1=float(input('Quanto mede em cm o 1º lado?'))
except ValueError:
    print('o 1º lado deve ser um número!')
else:
    if lado1<=0:
        print('o 1º lado deve ser positivo!')
    else:
        try:
            lado2=float(input('Quanto mede em cm o 2º lado?'))
        except ValueError:
            print:('o 2º lado deve ser um número!')
        else:
            if lado2<0:
                print('o 2º lado deve ser positivo!')
            else:
                try:
                    lado3=float(input('Quanto mede em cm o 3º lado?'))
                except ValueError:
                    print('o 3º lado deve ser um número!')
                else:
                    if lado3<=0:
                        print('o 3º lado deve ser positivo!')
                    else:
                        if lado1+lado2<=lado3 or lado1+lado3<=lado2 or lado2+lado3<=lado1:
                            print('Tais lados não formam um triangulo!')
                        else:
                            perimetro=lado1+lado2+lado3
                            print('o perimetro do triangulo vale',perimetro,'cm')

print('PROGRAMA FINALIZADO COM SUCESSO!')
