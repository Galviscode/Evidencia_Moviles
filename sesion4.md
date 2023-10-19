<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 4


<!-- Su documentación aquí -->

## Main

package com.mycompany.actividad4;

public class Actividad4 {

    public static void main(String[] args) {
        Producto producto1 = new Producto("Producto A", 13.500, "Fabricante X", "Marca1", "Electronica");
        Producto producto2 = new Producto("Producto B", 50.000, "Fabricante Y", "Marca2", "Ropa");
        
        System.out.println("Informacion del producto 1:");
        producto1.mostrarInformacion();
        
        System.out.println("\nInformacion del producto 2:");
        producto2.mostrarInformacion();
        
        producto1.setPrecio(15.900);
        producto2.setCantidad(12);
        
        System.out.println("\nInformacion actualizada del producto 1:");
        producto1.mostrarInformacion();
        System.out.println("\nInformacion actualizada del producto 2:");
        
        System.out.println("\nMarca del Producto 1: " + Producto.getMarca());
        System.out.println("Marca del producto 2: " + Producto.getMarca());
        
        Producto.setMarca("Nueva Marca");
        
        System.out.println("\nMarca del producto 1 despues del cambio: " + Producto.getMarca());
        System.out.println("Marca del producto 2 despues del cambio: " + Producto.getMarca());
    }
}

## Producto

package com.mycompany.actividad4;

public class Producto {
    public String nombre;
    private double precio;
    protected int cantidad;
    final String fabricante;
    static String marca;
    String categoria;

    public Producto(String nombre, double precio, String fabricante, String categoria, String electronica) {
        this.nombre = nombre;
        this.precio = precio;
        this.cantidad = cantidad;
        this.fabricante = fabricante;
        this.categoria = categoria;
    }

    public double getPrecio() {
        return precio;
    }

    public void setPrecio(double precio) {
        this.precio = precio;
    }

    protected int getCantidad() {
        return cantidad;
    }

    protected void setCantidad(int cantidad) {
        this.cantidad = cantidad;
    }

    public String getNombre() {
        return nombre;
    }

    String getCategoria() {
        return categoria;
    }

    void setCategoria(String categoria) {
        this.categoria = categoria;
    }

    public static String getMarca() {
        return marca;
    }

    public static void setMarca(String marca) {
        Producto.marca = marca;
    }
    
    public void mostrarInformacion() {
        System.out.println("Nombre: " + nombre);
        System.out.println("Precio: " + precio);
        System.out.println("Cantidad: " + cantidad);
        System.out.println("Fabricante: " + fabricante);
        System.out.println("Marca: " + marca);
        System.out.println("Categoria: " + categoria);
    }
}


