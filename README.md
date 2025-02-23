# fp_tp2

public class Cilindro {
    private double raio; //os atributos do objeto sao sempre privados
    private double altura; // a unica coisa que distingue os objetos de uma classe e o seu valor - o estado dos objetos

    //aceder a um atributo - raio
    public double getRaio() { //metodo que retorna um double - o raio.

        return raio; //devolve o valor do atributo raio
    }
    //aceder ao atributo - altura
    public double getAltura() {
        return altura;
    }
    //metodo de modificacao permite alterar o valor do atribuito. comecam sempre com set. recebem um valor que será atualizado
    //este metodo nao devolve nada - dai ser void - apenas altera o valor dos atributos
    public void setRaio(double raio) {
        this.raio = raio; //this - referencia para o proprio objeto. este objeto. neste caso, refere-se ao atributo altura deste objeto
    }
    public void setAltura(double altura) {
        this.altura = altura; //atribuimos ao atributo altura deste objeto - this - o valor passado por parametro
    }
    public double calcularVolume () {
        double vol = Math.PI * Math.pow(raio,2) * altura;
        return vol;
    }
}
