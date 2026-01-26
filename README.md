# UD-4-Entregable-1-Jose-Medina

## Codigo refactorizado

	public static void main(String[] args) {

	    int[] numeros = {5, 7, 3, 7, 2, 9, 7};

	    int maximo = numeros[0];
	    int contadorMaximo = 0;
	    int suma = 0;

	    // Un solo recorrido del array
	    for (int numero : numeros) {
	        suma += numero;

	        if (numero > maximo) {
	            maximo = numero;
	            contadorMaximo = 1;
	        } else if (numero == maximo) {
	            contadorMaximo++;
	        }
	    }

	    // Comprueba si el máximo se repite
	    if (contadorMaximo > 1) {
	        System.out.println("SI");
	    } else {
	        System.out.println("NO");
	    }

	    // Calcula media
	    double media = (double) suma / numeros.length;
	    System.out.println(media);

	    if (media >= 5) {
	        System.out.println("BIEN");
	    } else {
	        System.out.println("MAL");
	    }
	}
