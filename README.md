# Nishanthimport javax.swing.JFrame;
import javax.swing.JLabel;
import javax.swing.SwingUtilities;
public class SimpleLabelDemo {
 // Method to create and display the GUI
 private static void createAndShowGUI() {
 // Create a new JFrame (window) with a title
 JFrame frame = new JFrame("Simple JLabel Demo");
 
 // Set the default close operation to exit the application
 frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
 
 // Set the size of the window (width x height)
 frame.setSize(300, 100);
 
 // Create a JLabel with a text message
 JLabel label = new JLabel("Hello, Swing!", JLabel.CENTER);
 
 // Add the JLabel to the frame's content pane
 frame.getContentPane().add(label);
 
 // Make the frame visible
 frame.setVisible(true);
 }
 public static void main(String[] args) {
 // Ensure the GUI updates are handled on the Event Dispatch Thread (EDT)
 SwingUtilities.invokeLater(SimpleLabelDemo::createAndShowGUI);
 }
}
