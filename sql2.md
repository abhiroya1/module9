import java.sql.*;

public class LoadDriver {
    public static void main(String[] args) {
        try {
            // Load the MySQL JDBC driver
            Class.forName("org.sqlite.JDBC");
            // If successful, print the driver name
            System.out.println("SQLite JDBC Driver Loaded Successfully!");
        } catch (ClassNotFoundException e) {
            // If the driver is not found, print an error message
            System.out.println("SQLite JDBC Driver not found.");
            e.printStackTrace();
        }
    }
}
