# Polimorfismo-Dinamico
public class Empregado {
		protected String nome;
		protected String cargo;
		protected double salario;
		Empregado (String nome,String cargo,double salario){
			this.nome=nome;
			this.cargo=cargo;
			this.salario=salario;}

		public String getNome(){
			return this.nome;}
		public double calcSalario (){
			return this.salario;
		}}
    
    public class Vendedor extends Empregado {
	Vendedor (String nome,String cargo,double salario){
		super (nome,cargo,salario);}
	public double calcSalario(){
		return this.salario+200;}}
    
public class Analista extends Empregado {
	
	Analista (String nome,String cargo,double salario){
		super (nome,cargo,salario);}
	
	public double calcSalario(){
		return this.salario+700;}}
  
public class TesteEmpregado {
	public static void main(String []args){
		Empregado e = new Empregado("Joao","secretario",1000);
		Vendedor v = new Vendedor ("maria","Vendedor",1000);
		Analista a = new Analista ("pedro","Analista",1000);
		
		System.out.println(e.getNome());
		System.out.println(e.calcSalario());
		System.out.println(v.getNome());
		System.out.println(v.calcSalario());
		System.out.println(a.getNome());
		System.out.println(a.calcSalario());
		}}





    
    
