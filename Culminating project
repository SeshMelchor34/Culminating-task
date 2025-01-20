import javax.swing.*;
import java.awt.*;
import java.awt.event.*;
import javax.swing.ImageIcon;

class culminatingtask {
  public static void threePanelApp() {
    // Creating the main frame
    JFrame frame = new JFrame("Three Panels Application");
    frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
    frame.setSize(600, 400);

    // Creating the first panel with two buttons
    JPanel panel1 = new JPanel();
    panel1.setLayout(new FlowLayout());

    JButton button1 = new JButton("");
    JLabel label1 = new JLabel("Button 1");

    button1.setPreferredSize(new Dimension(50, 50));

    JButton button2 = new JButton("");
    JLabel label2 = new JLabel("This is button 2");

    // Resizing button2 and setting a rollover icon
    button2.setPreferredSize(new Dimension(50, 50));
    ImageIcon button2Icon = new ImageIcon("C:\\Users\\melchos730\\IdeaProjects\\CulminatingProject\\images\\leaf.png");
    button2.setRolloverIcon(button2Icon);

    // Add action listener to button2
    button1.addActionListener(new ActionListener() {
      @Override
      public void actionPerformed(ActionEvent e) {
        JOptionPane.showMessageDialog(frame, "Button 1 selected!");
      }
    });

    // Add action listener to button2
    button2.addActionListener(new ActionListener() {
      @Override
      public void actionPerformed(ActionEvent e) {
        JOptionPane.showMessageDialog(frame, "Button 2 selected!");
      }
    });

    panel1.add(button1);
    panel1.add(label1);
    panel1.add(button2);
    panel1.add(label2);

    // Creating the second panel with checkboxes
    JPanel panel2 = new JPanel();
    panel2.setLayout(new FlowLayout());


    Icon alienwareAuroraIcon = new ImageIcon ("C:\\Users\\melchos730\\IdeaProjects\\CulminatingProject\\images\\alienwareAurora.jpeg");
    Image alienwareAuroraImg = ((ImageIcon) alienwareAuroraIcon).getImage().getScaledInstance(100,100, java.awt.Image.SCALE_SMOOTH);
    alienwareAuroraIcon =new ImageIcon(alienwareAuroraImg);
    JCheckBox alienwareAurora = new JCheckBox("Alienware Aurora R15 - $3,306",alienwareAuroraIcon );

    Icon microsoftSurfaceIcon = new ImageIcon ("C:\\Users\\melchos730\\IdeaProjects\\CulminatingProject\\images\\microsoftSurface.jpeg");
    Image microsoftSurfaceImg = ((ImageIcon) microsoftSurfaceIcon).getImage().getScaledInstance(100,100, java.awt.Image.SCALE_SMOOTH);
    microsoftSurfaceIcon =new ImageIcon(microsoftSurfaceImg);
    JCheckBox microsoftSurface9 = new JCheckBox("microsoftSurface9 - $2399.99",microsoftSurfaceIcon);

    Icon dellXps15Icon = new ImageIcon ("C:\\Users\\melchos730\\IdeaProjects\\CulminatingProject\\images\\s-l1200.jpeg");
    Image dellXps15Img = ((ImageIcon) dellXps15Icon).getImage().getScaledInstance(100,100, java.awt.Image.SCALE_SMOOTH);
    dellXps15Icon =new ImageIcon(dellXps15Img);
    JCheckBox dellXps15 = new JCheckBox("Dell Xps 15 - $1749.99",dellXps15Icon);


    JButton calculateButton2 = new JButton("Calculate Total");
    calculateButton2.addActionListener(new ActionListener() {
      @Override
      public void actionPerformed(ActionEvent e) {
        double total = 0;
        if (alienwareAurora.isSelected())total += 3306;
        if (alienwareAurora.isSelected())alienwareAurora.setBorder(BorderFactory.createLineBorder(Color.red));
        if (microsoftSurface9.isSelected()) total += 2399.99;
        if (dellXps15.isSelected()) total += 1749.99;

        double tax = total * 0.15;  // 15% tax
        double totalPrice = total + 15 + tax;  // Adding $15 flat fee

        JOptionPane.showMessageDialog(frame, "Total: $" + totalPrice);
      }
    });

    panel2.add(alienwareAurora);
    panel2.add(microsoftSurface9);
    panel2.add(dellXps15);
    panel2.add(calculateButton2);

    // Creating the third panel with a single checkbox
    JPanel panel3 = new JPanel();
    panel3.setLayout(new FlowLayout());

    JRadioButton option4 = new JRadioButton("Option 4 - $50");

    JButton calculateButton3 = new JButton("Calculate Total");
    calculateButton3.addActionListener(new ActionListener() {
      @Override
      public void actionPerformed(ActionEvent e) {
        double total = 0;
        if (option4.isSelected()) total += 50;

        double tax = total * 0.15;  // 15% tax
        double totalPrice = total + 15 + tax;  // Adding $15 flat fee

        JOptionPane.showMessageDialog(frame, "Total: $" + totalPrice);
      }
    });

    panel3.add(option4);
    panel3.add(calculateButton3);

    // Adding all panels to the frame
    frame.setLayout(new GridLayout(1, 3));
    frame.add(panel1);
    frame.add(panel2);
    frame.add(panel3);

    // Set frame visible
    frame.setVisible(true);
    frame.setSize(1000,500);
  }


  public static void main(String[] args) {
    javax.swing.SwingUtilities.invokeLater(new Runnable() {
      public void run() {
       threePanelApp ();
      }
    });
  }
}
