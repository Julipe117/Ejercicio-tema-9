# Ejercicio-tema-9
Ejercicio del tema 9 de Introducción a la programación

  public class ejercicio_tema_9{

      public static void main(String[] args){
          Cliente cliente = new Cliente();
          Trabajador trabajador = new Trabajador();

          cliente.setNombre("Juan Perez");
          cliente.setEdad(26);
          cliente.setTelefono(638793572);
          cliente.setCredito(12000);

          System.out.println(cliente.getNombre());
          System.out.println(cliente.getEdad() + " años");
          System.out.println(cliente.getTelefono());
          System.out.println(cliente.getCredito());

          trabajador.setNombre("Antonio Ruiz");
          trabajador.setEdad(32);
          trabajador.setTelefono(955765562);
          trabajador.setSalario(1400);

          System.out.println(trabajador.getNombre());
          System.out.println(trabajador.getEdad() + " años");
          System.out.println(trabajador.getTelefono());
          System.out.println(trabajador.getSalario());
      }
  }

  class Persona{

      String nombre;
      int edad;
      int telefono;

      public void setNombre (String nombre){
          this.nombre = nombre;
      }
      public String getNombre(){
          return this.nombre;
      }

      public void setEdad (int edad){
          this.edad = edad;
      }
      public int getEdad(){
          return this.edad;
      }

      public void setTelefono (int telefono){
          this.telefono = telefono;
      }
      public int getTelefono(){
          return this.telefono;
      }
  }

  class Cliente extends Persona{
      int credito;

      public void setCredito (int credito){
          this.credito = credito;
      }
      public int getCredito(){
          return this.credito;
      }
  }

  class Trabajador extends Persona{
      int salario;

      public void setSalario (int salario){
          this.salario = salario;
      }
      public int getSalario(){
          return this.salario;
      }
  }
