# **2025-OBJPROG-LAB022**
Week 05 - Methods in Java

Laboratory # 22 - Week 05 - Guided Coding Exercise 1: Basic Class Creation and Object Instantiation

## **Instructions**

### **Step 1.1: Accept the Assignment**

   1. Click on the assignment link provided by your instructor.
   2. GitHub Classroom will create a **private repository** under your GitHub account.
   3. After the repository is created, click **"Go to Repository"** to view your assignment.

---

### **Step 1.2: Setup your Git Environment**
Only perform this if this is the first time you will setup your Git Environment

   1. Create a GitHub Account:
   ```bash
   https://github.com/signup?source=login
   ```
      
   2. Download and Install Git on your Laptop/Desktop:
   ```bash
   https://git-scm.com/downloads
   ```
   
   3. Create a Folder in your Laptop/Desktop
   4. Right-click anywhere in the created folder and select "Open Git Bash Here".
   5. In the Git Bash Terminal, set your git name, perform command:
   ```bash
   git config --global user.name "Your Name"
   ```
   
   6. In the Git Bash Terminal, set your git email, perform command:
   ```bash
   git config --global user.email "your.email@example.com"
   ```
   
   7. Create your SSH Key, just follow the instructions, no need to provide filename and passphrase. In the Git Bash Terminal, perform command:
   ```bash
   ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
   ```
   
   8. Copy your SSH Keys into clipboard. In the Git Bash Terminal, perform command:
   ```bash
   clip < ~/.ssh/id_rsa.pub
   ```
   
   9. Log in to your GitHub account.
   10. In the upper-right corner of GitHub, click your profile picture and select Settings.
   11. In the left sidebar, click on SSH and GPG keys.
   12. Click the New SSH key button.
   13. In the Title field, give the key a recognizable name (e.g., "My Windows Laptop").
   14. In the Key field, CTRL + V or paste the keys copied into your clipboard. Save the key.
   15. Go Back to terminal, use command:
   ```bash
   ssh -T git@github.com
   ```

### **Step 2: Clone the Repository to Your Local Machine**

   1. On your repository page, click the green **"Code"** button.
   2. Copy the repository URL (choose HTTPS for simplicity).
   3. Open your terminal (or Git Bash, Command Prompt, or PowerShell) and run:
   
   ```bash
   git clone <git_repo_url>
   ```
   
   4. Navigate into the cloned folder:
   
   ```bash
   cd <git_cloned_folder>
   ```

### **Step 3: Complete the Assignment**

**Laboratory # 22 - Week 05 - Guided Coding Exercise 1: Basic Class Creation and Object Instantiation**

   **Objective:**
   - Discuss the concepts of objects and classes.
   - Create a simple class with attributes and methods, and instantiate an object.

   **File Naming Convention:**
   - `CarDemo.java`

   **Desired Output:**
   ```txt
   Car: 2020 Toyota Corolla
   ```

   **Notable Observations:**
   - The Car class acts as a blueprint for creating Car objects.
   - The myCar object is an instance of the Car class.
   - The displayInfo method defines the behavior of the Car object.

   **Java Programming Best Practices:**
   - Use meaningful class and variable names that clearly describe their purpose.
   - Use comments to explain your code and the purpose of classes and methods.
   - Follow Java naming conventions (e.g., class names start with an uppercase letter).
      
   **Step-by-Step Instructions:**

   1. Create the Car Class
      - Create a new Java file named `CarDemo.java`.
      - Define a class called `Car`.
      ```Java      
      class Car {
          // Code will go here
      }
      ```
            
   2. Add Attributes (Data Fields)
      - Inside the Car class, declare three instance variables (attributes):
         - make of type String
         - model of type String
         - year of type int
      ```Java
      class Car {
          String make;
          String model;
          int year;
      }
      ```

   3. Add a displayInfo Method
      - Inside the Car class, create a method named displayInfo.
      - This method should not return any value (void).
      - Inside the displayInfo method, add a println statement to print the car's information in the format: "Car: [year] [make] [model]"
      ```Java
      class Car {
          //... (attributes)...
      
          public void displayInfo() {
              System.out.println("Car: " + year + " " + make + " " + model);
          }
      }
      ```

   4. Create the main Method
      - In the same file (CarDemo.java), outside the Car class, create the main method. This is where your program will start running.
      ```Java
      public class CarDemo {
          public static void main(String[] args) {
              // Code will go here
          }
      }
      ```

   5. Create a Car Object
      - Inside the main method, create an object of the Car class named myCar. Use the new keyword to instantiate the object.
      ```Java
      Car myCar = new Car();
      ```

   6. Assign Values to Attributes
      - In the main method, assign values to the attributes of the myCar object:
         - Set the make to "Toyota".
         - Set the model to "Corolla".
         - Set the year to 2020.
      ```Java
      myCar.make = "Toyota";
      myCar.model = "Corolla";
      myCar.year = 2020;
      ```

   7. Call the displayInfo Method
      - In the main method, call the displayInfo() method on the myCar object.
      ```Java
      myCar.displayInfo();
      ```

   8. Compile and Run
       - Save the file as `CarDemo.java`.
       - Compile the code using `javac CarDemo.java` in your terminal or command prompt.
       - Run the compiled code using `java CarDemo`.

   **Conclusion**
   This exercise introduced the fundamental concepts of classes and objects in Java. Classes are blueprints for creating objects, and objects are instances of classes. Classes define the attributes and behaviors of objects. By understanding these concepts, you can start building more complex and organized Java programs that model real-world entities and their interactions.

### **Step 4: Push Changes to GitHub**
Once you've completed your changes, follow these steps to upload your work to your GitHub repository.

1. Check the status of your changes:
   Open the terminal and run:
   
   ```bash
   git status
   ```
   This command shows any modified or new files.
   
2. Stage the changes:
   Add all modified files to staging:
   
   ```bash
   git add .
   ```
   
3. Commit your changes:
   Write a meaningful commit message:
   
   ```bash
   git commit -m "Submitting OBJPROG Week 05 - Laboratory # 22"
   ```
   
4. Push your changes to GitHub:
   Upload your changes to your remote repository:
   
   ```bash
   git push origin main
   ```
