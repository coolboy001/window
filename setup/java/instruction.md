To install the Java Development Kit (JDK) on Windows, follow these steps:

### 1. **Download JDK**

1. **Visit the official Oracle JDK download page:**
   - Go to the [Oracle JDK download page](https://www.oracle.com/java/technologies/javase-downloads.html).
   
2. **Choose the JDK version:**
   - For the latest version, click on **JDK (Latest Release)**.
   - You’ll be redirected to a page where you can download the installer for Windows.

3. **Download the installer:**
   - Scroll down to the **"Windows"** section.
   - Select the appropriate installer:
     - **.exe** for a standard installer.
     - **.zip** for a manual installation (less common for most users).

4. **Accept the License Agreement** (if prompted), and then download the executable file (e.g., `jdk-xx.x.x_windows-x64_bin.exe`).

### 2. **Install JDK**

1. **Run the downloaded installer**:
   - Double-click the `.exe` file you downloaded to start the installation.

2. **Choose the installation directory**:
   - By default, the JDK will be installed in a directory like `C:\Program Files\Java\jdk-xx.x.x`. You can change the directory if needed, but it's best to leave it at the default location.

3. **Follow the installation prompts**:
   - The installer will offer options such as installing the JDK and the JRE. Keep the default selections and click **Next**.
   - It may also offer to install additional tools such as the **Java Mission Control** and **Oracle JDK updates**. You can select or deselect those as needed.

4. **Complete the installation**:
   - Once the installation is complete, click **Close**.

### 3. **Set Environment Variables**

To make sure your system can find Java, you need to set the **`JAVA_HOME`** environment variable and add Java to the **`PATH`**.

#### Set `JAVA_HOME`

1. **Right-click** on the **Start Menu** and select **System** or **System Properties**.
2. Click **Advanced system settings** on the left.
3. Click the **Environment Variables** button under the **Advanced** tab.
4. Under the **System variables** section, click **New** to add a new environment variable.
   - Variable name: `JAVA_HOME`
   - Variable value: The path to the JDK installation directory (e.g., `C:\Program Files\Java\jdk-xx.x.x`).
   
#### Add Java to the `PATH`

1. In the same **Environment Variables** window, under **System variables**, find the **Path** variable and click **Edit**.
2. In the Edit window, click **New** and add the path to the `bin` directory inside the JDK folder (e.g., `C:\Program Files\Java\jdk-xx.x.x\bin` or `%JAVA_HOME%\bin`).
3. Click **OK** to close all the windows.

### 4. **Verify the Installation**

1. **Open Command Prompt**:
   - Press **Windows + R**, type `cmd`, and hit Enter.
   
2. **Check Java version**:
   - Type the following command and press Enter:
     ```bash
     java -version
     ```
     - If Java is installed correctly, you should see output displaying the installed Java version, like:
       ```
       java version "xx.x.x"
       Java(TM) SE Runtime Environment (build xx.x.x-bxx)
       Java HotSpot(TM) 64-Bit Server VM (build xx.x.x-bxx, mixed mode)
       ```

3. **Check JDK version**:
   - Type:
     ```bash
     javac -version
     ```
     - You should see something like:
       ```
       javac xx.x.x
       ```

### 5. **Optional: Set Up IDE for Java Development**

To start writing Java code efficiently, you may want to install an Integrated Development Environment (IDE) like:

- **[IntelliJ IDEA](https://www.jetbrains.com/idea/)** (Community Edition is free)
- **[Eclipse](https://www.eclipse.org/downloads/)**
- **[NetBeans](https://netbeans.apache.org/)**

These IDEs offer features like syntax highlighting, code completion, and debugging tools for Java development.

Steps to access documents, release motes, developer guides
-  https://docs.oracle.com/en/java/javase/23/index.html
---

That's it! Java is now installed and ready for development.
