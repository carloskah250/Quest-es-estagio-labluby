# Quest-es-estagio-labluby

Logica da programação

1.1)

/* Calculando o Fatorial do Número Natural 5 */

public class Fatorial {

public static void main (String args[]){
    
    double x = 5;
    double f = x;
    
    while (x>1) {
        f = f*(x-1);
        x--;
        
    }
    
     System.out.println(f);
} }

1.2)

import java.util.Scanner;

public class CalculandoPremio { public static void main(String args[]) {

   Scanner sc = new Scanner(System.in);
    
   System.out.println("Informe o valor do premio:"); 
      int premio = sc.nextInt();
      
if (premio>0) {
    
    System.out.println("premio basic: " + premio*1);
    System.out.println("O premio é vip é = " + premio*1.2);
    System.out.println("O premio é premium é = " + premio*1.5);
    System.out.println("O premio é deluxe é = " + premio*1.8);
    System.out.println("O premio é special é = " + premio*1.8);
    }
      
else (premio<0) {
    
    System.out.println("O valor do premio nao pode ser 0 ou negativo"");
       
   }

}
}

1.3)

public class ConteNumerosPrimos {

public static void main(String[] args) {    
    for (int i = 1; i <= 200; i++) {
        if( NPrimo(i) )
            System.out.println(i + " é primo.");
    }    
}

private static boolean NPrimo(int numero) {
    for (int j = 2; j < numero; j++) {
        if (numero % j == 0)
            return false;   
    }
    return true;
}
}

1.4)

public class Vogalcount{

public static void main(String[] args) {
    
    String texto;
    int vA = 0, vE = 0, vI = 0, vO = 0, vU = 0, vTotal = 0;

    palavra = //informe a palavra

    
    for (int i = 0; i < palavra.length(); i++) {

        if (palavra.charAt(i) == 'a' || palavra.charAt(i) == 'A') {
            vA++;
        }
        if (palavra.charAt(i) == 'e' || palavra.charAt(i) == 'E') {
            vE++;
        }
        if (palavra.charAt(i) == 'i' || palavra.charAt(i) == 'I') {
            vI++;
        }
        if (palavra.charAt(i) == 'o' || palavra.charAt(i) == 'O') {
            vO++;
        }
        if (palavra.charAt(i) == 'u' || palavra.charAt(i) == 'U') {
            vU++;
        }

    } 

    
    JOptionPane.showMessageDialog(null, "a palavra digitada foi: " + palavra
            + "\n\nVogal A: " + vA
            + "\nVogal E: " + vE
            + "\nVogal I: " + vI
            + "\nVogal O: " + vO
            + "\nVogal U: " + vU
            + "\n\nTotal de vogal(is): " + (vA + vE + vI + vO + vU));
} 
}

1.5)

package javaapplication9; import javax.swing.JOptionPane;

public class Desconto{

public static void main (String[]args){
double valorp, valord, valore;

    valorp = Double.parseDouble(JOptionPane.showInputDialog("digite o valor do produto "));
    

    valord =  0.30;
    valore = valord*valorp;
    JOptionPane.showMessageDialog(null,"o valor do seu produto é "+valorp+"com desconto de 30% fica"+valore);





}
}

1.6)

public class Carlos {

public static void main(String[] args) {
    
    throws ParseException {
    DateFormat df = new SimpleDateFormat ("dd/MM/yyyy");
    df.setLenient(false);
    Date d1 = df.parse ("07/09/1822");
    System.out.println (d1);
    Date d2 = df.parse ("05/06/2006");
    System.out.println (d2);
    long dt = (d2.getTime() - d1.getTime()) + 3600000; 
    System.out.println (dt / 86400000L); 
}
}

}
1.7) public class Carlos {

public static void main(String[] args) {
    
    int vetor = new int [5];
    int contPar = 0;

    if (vetor[i] % 2 ==0) {

    contPar++;
    
    }
    
    System.out.println("A quantidade de numeros pares neste vetor é: " + contPar);


}
}

1.8) package vetores; import java.util.Scanner;

public class Carlos {

public static void main(String[] args) {
    
    Scanner in = new Scanner (System.in);
    
  string[] vetor = new string[] {
  "John Doe",
  "Jane Doe",
  "Alice Jones",
  "Bobby Louis",
  "Lisa Romero"
  
  };
  
  int termo;
  
  
  System.out.println("Digite o termo para procurar no vetor");
  termo = int.nextInt();
  
  for(int i = 0; i < vetor.lenghth; i++) {
  
      if(vetor[i] == termo) {
          System.out.println("No vetor o que encontramos com esse termo foi: " + i);
        }
      else if(i == vetor.length-1){
          System.out.println("O termo não existe no vetor");
          
        }
    }
  
  


}
}

1.9) package vetores;

public class Carlos {

public static void main(String[] args) {
    

    
 int[] array = new int[6];
 
 int x = array.length;
 
 int[] a = new int [x/3];
 int[] b = new int [x/3];
 int[] c = new int [x/3];
 
int z = array.concat(int a, int b, intc)
 

}
}

SQL

2.1) SELECT id

FROM tabela_pessoa

SELECT evento, pessoa_id

JOIN RELACAO

ON (id = pessoa_id)

JOIN Relacao2

ON (pessoa_id = evento)

2.2) SELECT nome FROM tabela_pessoa WHERE nome LIKE '%Doe'

2.3) INSERT INTO tabela_evento (id, evento, pessoa_id) VALUES (5, "EVENTO E", 5 )

2.4) UPDATE tabela_evento SET pessoa_id = 1 WHERE evento = evento D

2.5) DELETE FROM tabela_evento WHERE evento = evento D

2.6) DELETE FROM tabela_pessoa WHERE id = (1,4,5) and nome = ("john Doe", "Bobby Louis", "Lisa Romero")

2.7) ALTER TABLE tabela_pessoa ADD idade, int(5)

2.8) CREATE TABLE tabela_telefone

(

id: int primary key, telefone: varchar(200), pessoa_id: int foreign key

)

2.9) CREATE UNIQUE INDEX ix_telefone on tabela_telefone (telefone)

2.10) DROP TABLE tabela_telefone;

DESAFIO

Máquina de refrigerante
MENU (principal):

public class Carlos {

public static void main(String[] args) {
    
    Venda vendaRefri = new Venda();   
   boolean loop = true;  
   int iopçao = -1;  
   System.out.println(" Bem vindo a Vending Machine");  
 
   while (loop)  
   {  
      
      printOpcoes();  
     
      DataInputStream in = new DataInputStream(System.in);  
      try 
      {  
        iopçao = Integer.parseInt(in.readLine());
      } catch (Exception ex) {ex.printStackTrace();}  
      
   
      switch(iopçao) {  
         case 1:  
          
            System.out.println(vendaRefri.hasRefriMsg());  
          
            break;  
         case 2:  
           
            System.out.println(vendaRefri.getNumerodeRefri());  
           
            break;  
         case 3:  
            
            System.out.println(vendaRefri.saleRefri());  
        
            break;  
         case 4:  
      
            System.out.println("Obrigado.");  
            
            loop = false;  
            
            break;  
         default:  
             
             System.out.println("Desculpe, não entendemos o pedido");  
      }  
   }  
}  
  
public static void printOpcoes() {  
   System.out.println();  
   System.out.println("1 - Para refrigerantes");  
   System.out.println("2 - Para quantidade de refrigerantes");  
   System.out.println("3 - Para comprar 1 refrigerante");  
   System.out.println("4 - Sair");  
   System.out.println();  
}
}

VENDA:

public class Venda {

private MaquinaDeRefri maquina = new MaquinaDeRefri(10);

public String hasRefriMsg() 
{
	
	if (this.maquina.getEstoque() > 0)
		return "Sim, temos refrigerante.";
	
	else
		return "Desculpe-me, os refrigerantes acabaram.";
}

public String getNumerodeRefri() 
{
	
	if (this.maquina.getEstoque() > 1)
		return "Temos " + this.maquina.getEstoque()+ " refrigerantes em estoque";
	
	else if (this.maquina.getEstoque() == 1)
		return "Temos 1 refrigerante em estoque";
	
	else
		return "Desculpe os refrigerantes acabaram.";
}


public String saleRefri() 
{
	
	if (this.maquina.venda()) 
	{
		return "Pronto Sr., está aqui o seu refrigerante";
	} else
		return "Desculpe-me Sr., os refrigerantes acabaram.";
}
}

ESTOQUE:

public class MaquinaDeRefri { private int quantidade = 0;

public MaquinaDeRefri(int quantidade) 
{
	
	this.quantidade = quantidade;
}
public int getEstoque()
{
	return this.quantidade;
}

public boolean venda() 
{
	
	if (this.quantidade > 0) 
	{
		
		this.quantidade--;
		
		return true;
		
	} 
	else 
	{
		
		return false;
	}
}
}
