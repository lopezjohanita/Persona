//# Persona
Codigo persona //

public class Persona {

    private String nombre;
    private int edad;

    public Persona(String nombre, int edad) {
        this.nombre = nombre;
        this.edad = edad;
    }

    public String obtenerInformacion() {
        return "Nombre: " + nombre + ", Edad: " + edad;
    }
    
    // Getters y setters para los atributos privados
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
}

public class Doctor extends Persona {
    private String especialidad;

    public Doctor(String nombre, int edad, String especialidad) {
        super(nombre, edad);
        this.especialidad = especialidad;
    }

    @Override
    public String obtenerInformacion() {
        return super.obtenerInformacion() + ", Especialidad: " + especialidad;
    }
    
    // Getters y setters específicos para Doctor
    public String getEspecialidad() {
        return especialidad;
    }

    public void setEspecialidad(String especialidad) {
        this.especialidad = especialidad;
    }
}

public class Deportista extends Persona {
    private String deporte;

    public Deportista(String nombre, int edad, String deporte) {
        super(nombre, edad);
        this.deporte = deporte;
    }

    @Override
    public String obtenerInformacion() {
        return super.obtenerInformacion() + ", Deporte: " + deporte;
    }
    
    // Getters y setters específicos para Deportista
    public String getDeporte() {
        return deporte;
    }

    public void setDeporte(String deporte) {
        this.deporte = deporte;
    }
}
