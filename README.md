# aula1-github
import javax.swing.JOptionPane;

public class Teste{
	public static void main(String arg[]){
		try{
			
		int x,y,z,result;
		String xVal,yVal,zVal;
		
		xVal=JOptionPane.showInputDialog("Enter first number");
		x=Integer.parseInt(xVal);
		
		yVal=JOptionPane.showInputDialog("Enter second number");
		y=Integer.parseInt(yVal);
	
		zVal=JOptionPane.showInputDialog("Enter third number");
		z=Integer.parseInt(zVal);
		
		result = (x+y+z)/3;
		
		JOptionPane.showMessageDialog(null,"Saída\t"+ result);
	}//Fecha try.
	catch(NumberFormatException erro){
		JOptionPane.showMessageDialog(null,"Erro" + erro);
	}
	finally{
		JOptionPane.showMessageDialog(null,"Nice to meet you!!!!");
	}
	System.exit(0);
	
	}
}
