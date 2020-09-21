import java.awt.Color;
import java.awt.event.ActionEvent;
import java.awt.event.ActionListener;
import java.awt.event.KeyEvent;
import java.awt.event.KeyListener;
import java.awt.event.MouseEvent;
import java.awt.event.MouseListener;
import java.util.Random;

import javax.swing.JFrame;
import javax.swing.JPanel;
import javax.swing.Timer;

public class Pacman extends JFrame implements KeyListener, MouseListener{

	JPanel jp;
	protected static int x;
	protected static int y;
	protected static int arcAngle;
	protected static int sAngle;
	Timer t;
	protected static int jump;
	
	public Pacman() {		
		jp = new PacmanPaintPanel();
		add(jp);
		addKeyListener(this);
		addMouseListener(this);
		
		x = 10;
		y = 10;
		arcAngle = 300;
		sAngle = 30;
		jump =0;
		
//		ActionListener al = new ActionListener() {
//			
//			@Override
//			public void actionPerformed(ActionEvent e) {
//				x = new Random().nextInt(700);
//				y = new Random().nextInt(500);
//				jump++;
//				
//				if(jump >= 5) {
//					t.stop();
//				}
//				repaint();				
//			}
//		};
//		
//		t = new Timer(2000,al);
//		t.start();
		
		
		
		t = new Timer(200, new ActionListener() {
			
			@Override
			public void actionPerformed(ActionEvent e) {
				if(arcAngle >= 360) {
					arcAngle = arcAngle - 90;
				}
				repaint();
			}
		});
		t.start();
		
	}

	@Override
	public void keyTyped(KeyEvent e) {
		// TODO Auto-generated method stub
		
	}

	@Override
	public void keyPressed(KeyEvent e) {
		if(e.getKeyCode() == KeyEvent.VK_RIGHT){
			x = x + 5;
			if(x>770) {
				x = -30;
			}
			arcAngle = arcAngle + 10;
			repaint();
		}
		
		if(e.getKeyCode() == KeyEvent.VK_DOWN){
			y = y + 5;
			sAngle = -60;
			repaint();
		}
	}

	@Override
	public void keyReleased(KeyEvent e) {
		if(e.getKeyCode() == KeyEvent.VK_RIGHT){
			arcAngle = 300;
			repaint();
		}
	}

	@Override
	public void mouseClicked(MouseEvent e) {
		Color bg = new Color(new Random().nextInt(255),new Random().nextInt(255),new Random().nextInt(255));
		jp.setBackground(bg);
		
		
	}

	@Override
	public void mousePressed(MouseEvent e) {
		// TODO Auto-generated method stub
		
	}

	@Override
	public void mouseReleased(MouseEvent e) {
		// TODO Auto-generated method stub
		
	}

	@Override
	public void mouseEntered(MouseEvent e) {
		jp.setBackground(Color.white);
		
	}

	@Override
	public void mouseExited(MouseEvent e) {
		jp.setBackground(Color.black);
		
	}
}
