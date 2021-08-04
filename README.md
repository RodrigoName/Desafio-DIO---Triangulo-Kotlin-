# Desafio-DIO---Triangulo-Kotlin-

Leia 3 valores reais (A, B e C) e verifique se eles formam ou não um triângulo. Em caso positivo, calcule o perímetro do triângulo e apresente a mensagem:


Perimetro = XX.X


Em caso negativo, calcule a área do trapézio que tem A e B como base e C como altura, mostrando a mensagem


Area = XX.X

Entrada
A entrada contém três valores reais.

Saída
O resultado deve ser apresentado com uma casa decimal.


Desafio do triangulo Kotlin resolvido


fun main(args: Array<String>) {

  fun Double.format(digits: Int) = "%.${digits}f".format(this).replace(',','.')

    val (n1, n2, n3) = readLine()!!.split(" ")
    val a = n1.replace(",",".").toDouble()
    val b = n2.replace(",",".").toDouble()
    val c = n3.replace(",",".").toDouble()

  val p = (a + b + c)
  
  val r = ((a + b) * c / 2)

  
  if (a < (b + c) && b < (a + c) && c < (a + b)) println("Perimetro = $p") <br>
  else println("Area = $r")
}
                                          
                                          
Funcionando 100% dos testes, se gostou dê uma estrela!
