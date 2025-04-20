Exercício Estrutura de Dados - 2º segundo semestre - Sitemas para Internet - FATEC

Código Comementado

Código em Java com comentários linha a linha para explicar o que cada parte faz:
public class Main {
    public static void main(String[] args) {
        // Vetor de salários brutos com valores iniciais
        double[] SalarioBruto = {1245.45, 1455.11, 1850.00};
        
        // Vetor para armazenar os salários líquidos, com o mesmo tamanho do vetor de salários brutos
        double[] SalarioLiquido = new double[SalarioBruto.length];
        
        // Loop para calcular o salário líquido de cada salário bruto
        for (int i = 0; i < SalarioBruto.length; i++) {
            // Calcula o salário líquido aplicando um desconto de 11%
            SalarioLiquido[i] = SalarioBruto[i] * (1 - 0.11);
        }
        
        // Exibir os salários líquidos na saída padrão
        System.out.println("Salários Líquidos:");
        
        // Loop para imprimir cada salário líquido
        for (double salario : SalarioLiquido) {
            // Formata e exibe o salário com duas casas decimais
            System.out.printf("%.2f%n", salario);
        }
    }
}
Comentários Detalhados:
1.	public class Main {
o	Define a classe pública chamada Main. Em Java, todas as aplicações começam com uma classe.
2.	public static void main(String[] args) {
o	Este é o ponto de entrada da aplicação. O método main é o que o Java executa quando inicia o programa.
3.	double[] SalarioBruto = {1245.45, 1455.11, 1850.00};
o	Declara e inicializa um vetor chamado SalarioBruto que contém os valores dos salários brutos fornecidos.
4.	double[] SalarioLiquido = new double[SalarioBruto.length];
o	Cria um novo vetor chamado SalarioLiquido para armazenar os salários líquidos após os descontos. Seu tamanho é igual ao do vetor SalarioBruto.
5.	for (int i = 0; i < SalarioBruto.length; i++) {
o	Inicia um loop for que percorre todos os índices do vetor SalarioBruto. A variável i é usada como índice.
6.	SalarioLiquido[i] = SalarioBruto[i] * (1 - 0.11);
o	Calcula o salário líquido para o salário bruto correspondente, aplicando um desconto de 11% (multiplicando por 0,89) e armazena o resultado no vetor SalarioLiquido na mesma posição i.
7.	System.out.println("Salários Líquidos:");
o	Imprime uma mensagem na saída padrão para indicar que a lista de salários líquidos a seguir.
8.	for (double salario : SalarioLiquido) {
o	Inicia um loop for-each que itera sobre cada valor do vetor SalarioLiquido.
9.	System.out.printf("%.2f%n", salario);
o	Imprime cada salário líquido, formatando-o para que apareça com duas casas decimais, seguido de uma nova linha.
