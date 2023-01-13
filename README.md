# loginpage
login  using jframe
import javax.swing.*;
import java.awt.*;

public class login extends JFrame {
    JLabel password1, l,l2;
    JCheckBox c;
    JTextField username;
    JButton b,b1;
    JPasswordField Password;
     login(){
        JPanel p = new JPanel();
        p.setLayout(null);
        add(p);
        setTitle("LOGIN PAGE");
        l = new JLabel("Username");
        l.setBounds(100, 8, 70, 20);
        p.add(l);
        username = new JTextField();
        username.setBounds(100, 27, 193, 28);
        p.add(username);
        password1 = new JLabel("Password");
        password1.setBounds(100, 55, 70, 20);
        p.add(password1);
        Password = new JPasswordField();
        Password.setBounds(100, 75, 193, 28);
        p.add(Password);
        c=new JCheckBox();
        c.setBounds(100,107,20,20);
        p.add(c);
        l2=new JLabel("Show Password");
        l2.setBounds(120,107,90,20);
        p.add(l2);
        b = new JButton("Login");
        b.setBounds(100, 130, 90, 25);
        b.setForeground(Color.WHITE);
        b.setBackground(Color.BLACK);
        p.add(b);
        b1=new JButton("cancel");
        b1.setBounds(200,130,90,25);
        b1.setForeground(Color.WHITE);
        b1.setBackground(Color.BLACK);
        p.add(b1);
       // b.addActionListener(this);
         setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
         setLocation(new Point(500, 300));
         setSize(400, 200);
         setVisible(true);
    }
    public static void main(String[] args){
        new login();
    }
}
