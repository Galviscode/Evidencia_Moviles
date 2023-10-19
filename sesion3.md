<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 3 


<!-- Su documentación aquí -->

## Clase jugadores
//Atributos.

public class Jugadores {
    private String nombre;
    private int edad;
    private String posicion;
    private int numero_camiseta;
    private String equipo;

//Constructor.

public Jugadores(String nombre, int edad, String posicion, int numero_camiseta, String equipo) {
        this.nombre = nombre;
        this.edad = edad;
        this.posicion = posicion;
        this.numero_camiseta = numero_camiseta;
        this.equipo = equipo;
    }
//Metodos getter y setter.

    public String getNombre() {
        return nombre;
    }
    public void setNombre(String nombre) {
        this.nombre = nombre;
    }
    public int getEdad() {
        return edad;
    }
    public void setEdad(int edad) {
        this.edad = edad;
    }
    public String getPosicion() {
        return posicion;
    }
    public void setPosicion(String posicion) {
        this.posicion = posicion;
    }
    public int getNumero_camiseta() {
        return numero_camiseta;
    }
    public void setNumero_camiseta(int numero_camiseta) {
        this.numero_camiseta = numero_camiseta;
    }
    public String getEquipo() {
        return equipo;
    }
    public void setEquipo(String equipo) {
        this.equipo = equipo;
    }
    public String toString() {
        return "Jugadores{" +
                "nombre='" + nombre + '\'' +
                ", edad=" + edad +
                ", posicion='" + posicion + '\'' +
                ", numero_camiseta=" + numero_camiseta +
                ", equipo='" + equipo + '\'' +
                '}';
    }
## Main
    public static void main(String[] args) {
        Jugadores jugador1 = new Jugadores("Juan", 25, "Delantero", 10, "EquipoA");

        System.out.println("Nombre: " + jugador1.getNombre());
        System.out.println("Edad: " + jugador1.getEdad());
        System.out.println("Posición: " + jugador1.getPosicion());
        System.out.println("Número de Camiseta: " + jugador1.getNumero_camiseta());
        System.out.println("Equipo: " + jugador1.getEquipo());
        System.out.println(jugador1.toString());
    }
}




