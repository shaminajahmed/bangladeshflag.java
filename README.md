# bangladeshflag.java
Draw a Bangladesh Flag in java
import java.awt.*;
import javax.swing.*;
class MyCanvas extends JComponent {
@Override 
public void paint(Graphics g )
{
g.drawLine(50,50,50,500);
g.setColor(Color.green);
g.fillRect(50,50,350,200);
g.drawLine(50, 50, 300, 50);
g.drawLine(300, 50, 300, 150);
g.drawLine(300, 150, 50, 150);
g.drawLine(50, 150, 50, 50);
g.setColor(Color.RED);
g.fillOval(165, 100, 100, 100);
}
}
public class BangladeshFlag {
public static void main(String[] a)
{
JFrame window = new JFrame();
window.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
window.setBounds(30, 30, 200, 200);
window.getContentPane().add(new MyCanvas());
window.setVisible(true);
}
}
