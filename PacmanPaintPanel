import java.awt.Color;
import java.awt.Graphics;

import javax.swing.JPanel;

public class PacmanPaintPanel extends JPanel{

	@Override
	public void paint(Graphics g) {
		super.paint(g);
		
//		g.drawLine(10,10,100,100);
//		g.drawRect(20, 20, 30, 40);
//		g.drawString("Hello", 700, 500);
//		
		g.drawOval(50, 50, 50, 50);
		g.setColor(Color.blue);
		g.fillOval(200,200,30,30);
		g.setColor(Color.yellow);
		g.fillArc(Pacman.x,Pacman.y,70,70,Pacman.sAngle,Pacman.arcAngle);
		
		g.setColor(Color.black);
		g.drawString("Number of Jumps = " + Pacman.jump + "", 650, 550);
		
	}

}
