# MODULO-PRUEBA

package Electro;

public abstract class Electrodomestico{
	
	//Constantes
	String COLORDEF="blanco";
	char CONSUMODEF='F';
	double PRECIODEF=100;
	double PESODEF=5;
	
	
     // ATRIBUTOS
	
	String Color;
	char Consumo;
	double Precio;
	double Peso;


	// CONSTRUCTOR POR DEFECTO
	
	
	
	
	public Electrodomestico() {  /// CONSTRUCTOR VACIO A
		super();
		this.Consumo=CONSUMODEF;
		this.Color=COLORDEF;
		this.Precio=PRECIODEF;
		this.Peso=PESODEF;
		
	}


	
		// CONSTRUCTOR POR DEFECTO CON 2 PARAMETROS
		
	public Electrodomestico(String cOLORDEF, char cONSUMODEF, double pRECIODEF, double pESODEF, double precio,
			double peso) {
		super();
		COLORDEF = cOLORDEF;
		CONSUMODEF = cONSUMODEF;
		PRECIODEF = pRECIODEF;
		PESODEF = pESODEF;
		Precio = precio;
		Peso = peso;
	}

// CONSTRUCTOR CON TODOS LOS ATRIBUTOS
	
public Electrodomestico(String color, char consumo, double precio, double peso) {
		super();
		Color = color;
		Consumo = consumo;
		Precio = precio;
		Peso = peso;
	}
   ///METODO GET

	public String getColordef() {
		return COLORDEF;
	}


	public void setColordef(String colordef) {
		COLORDEF = colordef;
	}


	public char getConsumodef() {
		return CONSUMODEF;
	}


	public void setConsumodef(char consumodef) {
		CONSUMODEF = consumodef;
	}


	public double getPreciodef() {
		return PRECIODEF;
	}


	public void setPreciodef(double preciodef) {
		PRECIODEF = preciodef;
	}


	public double getPesodef() {
		return PESODEF;
	}


	public void setPesodef(double pesodef) {
		PESODEF = pesodef;
	}


	public String getColor() {
		return Color;
	}


	public void setColor(String color) {
		Color = color;
	}


	public char getConsumo() {
		return Consumo;
	}


	public void setConsumo(char consumo) {
		Consumo = consumo;
	}


	public double getPrecio() {
		return Precio;
	}


	public void setPrecio(double precio) {
		Precio = precio;
	}


	public double getPeso() {
		return Peso;
	}


	public void setPeso(double peso) {
		Peso = peso;
	}
	
	public void comprobarConsumoEnergetico(char consumo){
		
		String consumos[]={"A","B","C","D","F"};
		
		
		boolean encontrado = false;
		for (int i=0; i<consumos.length && !encontrado;i++){
			if (consumos[i].equals(consumo))
				encontrado=true;
		}
	}
			
	
		
		
		public void comprobarColor(String color){	
			String colores[]={"blanco", "negro", "rojo", "azul", "gris"};
			
		
			boolean encontrado = false;
			for (int i = 0; i < colores.length; i++) {
				
				
			}
		
	}
}


		
    
    package Electro;
import java.util.Scanner;
public class Lavadora extends Electrodomestico {
	

	
		
		
	
	
	//CONSTANTE
	
	Integer CARGADEF=5;
	
	// atributo propio de la clase
	
	Integer carga;
	
	
	//SETER AND GETER

	public Integer getCarga() {
		return carga;
	}

	public void setCarga(Integer carga) {
		this.carga = carga;
	}

	
	
	public Lavadora() {
		super();
		
		this.carga=CARGADEF;
		
		
	}
      // CONSTRUCTOR PROPIO
	public Lavadora(Integer carga) {
		super();
		this.carga = carga;
	}
