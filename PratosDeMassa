public class PratosDeMassa {
    public static void main (String [] args) {
        int[] realidades = {4	,1,	15,	12	,0,	9,	9,	5	,5,	8,	7	,3	,14,	5	,12	,3};
        int vezes = 1;
        System.out.print ("original: ");
        imprimeValores(realidades);
        int[] aux = {4	,1,	15,	12	,0,	9,	9,	5	,5,	8,	7	,3	,14,	5	,12	,3};

        while (igual(aux,realidades.length,vezes)<0) {
            int posmassa = maior(realidades);
            int massas = realidades[posmassa];
            realidades[posmassa] = 0;

            while (massas > 0) {
                posmassa++;
                if (posmassa == realidades.length) posmassa = 0;
                realidades[posmassa]++;
                massas--;
            }
            System.out.print ("\nvez: " + vezes + "\t");
            imprimeValores(realidades);
            vezes++;
            aux = vetorAuxiliar(realidades, aux, vezes, realidades.length);
        }
        System.out.print ("\n\n\nVezes pra ser igual a um anterior: " + (vezes-1) + "\nVetor que repete: ");
        imprimeValores(realidades);
        System.out.print ("\nVez que esse vetor apareceu pela primeira vez: " + igual(aux,realidades.length,vezes));
        System.out.println ("\nTamanho do loop: " + ((vezes-1)-igual(aux,realidades.length,vezes)));


    }
    public static void imprimeValores (int[] vetor) {
        for(int i=0;i< vetor.length;i++) {
            System.out.print( vetor[i]+ " ");
        }
    }
    public static int maior (int[] vetor) {
        int maior = vetor[0];
        int posmaior = 0;
        for (int i=1;i<vetor.length;i++) {
            if (vetor[i]>maior) {
                maior = vetor[i];
                posmaior = i;
            }
        }
        return posmaior;
    }
    public static int[] vetorAuxiliar (int[] vetorAdicionar,int[]vetorAntes, int vezes, int tamOriginal) {
        int[] aux = new int[tamOriginal*vezes];
        for (int i=0;i<vetorAntes.length;i++) {
            aux[i]=vetorAntes[i];
        }
        int p=0;
        for (int j=vetorAntes.length;j<aux.length;j++) {
            aux[j]=vetorAdicionar[p];
            p++;
        }
        return aux;
    }
    public static int igual (int[] aux, int tamRealidades, int vezes) {
        int i=0, j=tamRealidades*(vezes-1), contagemVetor = 1;
        int igual=-1;
        if (j!=0) {
        while (i<j && j<aux.length) {
            for (int v=0;v<tamRealidades;v++) {
               if (aux[i] == aux[j]) {
                   i++;
                   j++;
                   igual=contagemVetor;
               } else {
                   igual=-1;
                   i = contagemVetor*tamRealidades;
                   j = tamRealidades*(vezes-1);
                   break;
               }
            }
            if (igual!=-1) break;
            else contagemVetor++;
            }
        }
        return (igual-1);
    }
}

