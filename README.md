Beginner’s Guide to Pair Programming: Building and Publishing a Simple Web Page on GitHub Pages with HTML and CSS
=================================================================================================================

Welcome to your journey into web development! This guide is designed for complete beginners and utilises a **self-directed peer-led learning approach**. By partnering with a peer, you’ll collaborate to build and publish a simple web page using HTML and CSS, then host it on GitHub Pages. Let’s get started!

(In truth, you don't need to pair on this. You can work solo. But if you are at the meetup, we do recommend working with somebody else on it.) 

Table of Contents
-----------------

1.  [Introduction to Pair Programming](#1-introduction-to-pair-programming)
2.  [Creating a GitHub Repository](#2-creating-a-github-repository)
3.  [Setting Up Your Development Environment](#3-setting-up-your-development-environment)
4.  [Cloning the Repository Using Command Line](#4-cloning-the-repository-using-command-line)
5.  [Understanding HTML Basics](#5-understanding-html-basics)
6.  [Understanding CSS Basics](#6-understanding-css-basics)
7.  [Committing HTML and CSS to GitHub](#7-committing-html-and-css-to-github)
8.  [Publishing Your Web Page with GitHub Pages](#8-publishing-your-web-page-with-github-pages)
9.  [Conclusion and Self-Test Questions](#9-conclusion-and-self-test-questions)

1\. Introduction to Pair Programming
------------------------------------

**Pair Programming** is a collaborative practice where two programmers work together at one workstation. One person, the **Driver**, writes the code, while the other, the **Navigator**, reviews each line of code as it’s written. Roles can switch frequently to enhance learning and catch errors early.

**Benefits:**
-------------

*   **Enhanced Learning:** Both participants learn from each other’s strengths.
*   **Improved Code Quality:** Continuous code review reduces bugs.
*   **Problem Solving:** Two minds can solve problems faster and more effectively.

**Peer-Led Learning:** In this approach, peers guide each other without a formal instructor, fostering a supportive learning environment.

2\. Creating a GitHub Repository
--------------------------------

A **repository (repo)** is a storage space for your project on GitHub. It tracks all changes to your code and allows collaboration with others.

### **Steps to Create a Repository:**

1.  **Log In to GitHub:**
    
    *   Go to [GitHub](https://github.com/) and log in to your account. If you don't have an account, sign up [here](https://github.com/join).
2.  **Create a New Repository:**
    
    *   Go to this organisation, and click the green "New" button to create a new repo.
3.  **Configure Repository Settings:**
    
    *   **Repository Name:** Enter a name (e.g., `my-first-webpage`).
    *   **Description:** (Optional) Briefly describe your project.
    *   **Public/Private:** Choose "Public" so others can see your project.
    *   **Initialize Repository:** Check "Add a README file."
    *   Click "Create repository."

**Concepts Introduced:**
------------------------

*   **Repository:** A project folder in GitHub to store code.
*   **README:** A markdown file that describes your project.

3\. Setting Up Your Development Environment
-------------------------------------------

Before you start coding, ensure you have the necessary tools installed.

### **For Windows Users:**

If you are using Windows then you won't have a Linux-like terminal by default so you will need to install one. Please follow [the installation instructions found here](https://code.visualstudio.com/docs/remote/wsl) to get a Linux distribution running on your Windows machine and to get it hooked up with VS Code on Windows.

Here are a couple of older but still helpful guides that have some more information about setting up and using WSL as part of your development environment:

[Set up a WSL development environment](https://learn.microsoft.com/en-us/windows/wsl/setup/environment)

[Get started using Visual Studio Code with Windows Subsystem for Linux](https://learn.microsoft.com/en-us/windows/wsl/tutorials/wsl-vscode)

### **Tools Needed:**

*   **Code Editor:** Software to write your code. [Visual Studio Code (VS Code)](https://code.visualstudio.com/) is highly recommended for beginners.
*   **Git:** Version control system to track changes. [Download Git](https://git-scm.com/downloads).
*   **Command Line Interface (CLI):**    
    *   **Windows:** Use Command Prompt or Git Bash.
    *   **macOS/Linux:** Use Terminal.


### **Installation Steps:**

1.  **Install VS Code:**
    
    *   Visit the [VS Code website](https://code.visualstudio.com/) and download the installer for your operating system.
    *   Follow the installation prompts.
2.  **Install Git:**
    
    *   Go to the [Git download page](https://git-scm.com/downloads).
    *   Download and install Git for your OS.
    *   During installation, select the option to add Git to your system PATH.

3.  **Configure Git (First-Time Setup):**
    
    *   Open your CLI.
    *   Set your username:
        
        ```bash
        git config --global user.name "Your Name"
        ```
        
    *   Set your email:
        
        ```bash
        git config --global user.email "your-email@example.com"
        ```
        

**Concepts Introduced:**
------------------------

*   **Code Editor:** Tool for writing and editing code.
*   **Git:** Version control system to manage code changes.
*   **System PATH:** Environment variable that tells the OS where to find executables.
*   **Command Line Interface (CLI):** Interact with your computer like it's 1970.

4\. Cloning the Repository Using Command Line
---------------------------------------------

**Cloning** a repository means creating a local copy of the repository on your computer. This allows you to work on your project locally.

### **Steps to Clone a Repository:**

1.  **Copy Repository URL:**
    *   On your repository page on GitHub, click the green "Code" button.
    *   Copy the HTTPS URL provided (e.g., `https://github.com/this-org-name/my-first-webpage.git`).
2.  **Open Command Line Interface (CLI)**
3.  **Navigate to Desired Directory:**
    
    ```bash
    cd path/to/your/directory
    ```
    
    Replace `path/to/your/directory` with the path where you want to store your project.
    
4.  **Run the Clone Command:**
    
    ```bash
    git clone https://github.com/your-username/my-first-webpage.git
    ```
    
    Replace `your-username` with your GitHub username.
    
5.  **Navigate to the Cloned Repository:**
    
    ```bash  
    cd my-first-webpage
    ```
    

**Concepts Introduced:**
------------------------
*   **Changing directory:** Using the `cd` command, one of many useful UNIX commands you will learn over time.
*   **Cloning:** Creating a local copy of a remote repository.

5\. Understanding HTML Basics
-----------------------------

**HTML (HyperText Markup Language)** is the standard language for creating web pages. It structures the content on the web.

### **Basic Structure of an HTML Document:**

```html

<!DOCTYPE html>
<html>
<head>
    <title>My First Web Page</title>
</head>
<body>
    <h1>Welcome to My Website</h1>
    <p>This is a paragraph of text.</p>
</body>
</html>
```

**Explanation:**
----------------

*   `<!DOCTYPE html>`: Declares the document type and version of HTML.
*   `<html>`: Root element that wraps the entire content.
*   `<head>`: Contains meta-information about the document, like the title.
*   `<title>`: Sets the title of the web page shown in the browser tab.
*   `<body>`: Contains the visible content of the web page.
*   `<h1>`: Heading level 1, used for main titles.
*   `<p>`: Paragraph tag for blocks of text.

**Concepts Introduced:**
------------------------

*   **Tags:** Enclosed in angle brackets (`< >`), define elements.
*   **Elements:** Building blocks of HTML, consisting of tags and content.
*   **Attributes:** Provide additional information about elements (not covered yet but important for future learning).

6\. Understanding CSS Basics
----------------------------

**CSS (Cascading Style Sheets)** is used to style and layout web pages—for example, to change colors, fonts, and spacing.

### **Adding CSS to Your HTML Document:**

You can add CSS directly within your HTML using the `<style>` tag.

```html

<!DOCTYPE html>
<html>
<head>
    <title>My First Web Page</title>
    <style>

        body {
            background-color: #f0f0f0;
        }
        h1 {
            color: blue;
            text-align: center;
        }
        p {
            font-family: Arial, sans-serif;
            font-size: 16px;
        }
    
</style>
</head>
<body>
    <h1>Welcome to My Website</h1>
    <p>This is a paragraph of text.</p>
</body>
</html>
```

**Explanation:**
----------------

*   `<style>`: Tag used to embed CSS in the HTML document.
*   **Selectors:** Specify which HTML elements to style (`body`, `h1`, `p`).
*   **Properties:** Define what aspect to style (e.g., `background-color`, `color`, `font-family`).
*   **Values:** Set the property’s value (e.g., `#f0f0f0`, `blue`, `Arial, sans-serif`).

**Concepts Introduced:**
------------------------

*   **CSS Syntax:** `selector { property: value; }`
*   **Selectors:** Target HTML elements for styling.
*   **Properties and Values:** Define specific styles.

7\. Committing HTML and CSS to GitHub
-------------------------------------

After creating your web page files, you need to **commit** them to your local repository and **push** the changes to GitHub.

### **Step-by-Step Guide:**

1.  **Open VS Code:**
    
    *   Open the cloned repository folder (`my-first-webpage`) in VS Code.
2.  **Create an `index.html` File:**
    
    *   In VS Code, create a new file named `index.html`.
    *   Paste the basic HTML structure from Section 5.
3.  **Add CSS Styling:**
    
    *   Within the `<head>` tag of `index.html`, add the `<style>` section from Section 6.
4.  **Save Your Changes:**
    
    *   Press `Ctrl + S` (Windows) or `Cmd + S` (macOS) to save the file.
5.  **Open Terminal in VS Code:**
    
    *   Go to `View` > `Terminal` or press `` Ctrl + ` ``.
6.  **Check Repository Status:**
    
    ```bash
    git status
    ```
    
    This shows the current status of your repository and any changes.
    
7.  **Add Changes to Staging Area:**
    
    ```bash
    git add index.html
    ```
    
    This stages your changes for committing.
    
8.  **Commit Your Changes:**
    
    ```bash
    git commit -m "Add initial index.html with HTML and CSS"
    ```
    
    The `-m` flag allows you to add a commit message describing the changes.
    
9.  **Push Changes to GitHub:**
    
    ```bash
    git push origin main
    ```
    
    This uploads your committed changes to the `main` branch on GitHub.
    

**Explanation:**
----------------

*   **Cloning:** Copies the repository from GitHub to your local machine.
*   **Creating Files:** Adding `index.html` which is the default page for web browsers.
*   **Committing:** Saves your changes with a descriptive message.
*   **Pushing:** Uploads your local commits to GitHub.

**Concepts Introduced:**
------------------------

*   **Staging Area:** Where changes are prepared before committing.
*   **Commit Message:** Describes the changes made in a commit.
*   **Branch:** A separate line of development; `main` is the default branch.

8\. Publishing Your Web Page with GitHub Pages
----------------------------------------------

GitHub Pages allows you to host your web page directly from your repository, making it accessible on the web.

### **Steps to Publish:**

1.  **Go to Your Repository on GitHub:**
    
    *   Navigate to `https://github.com/your-username/my-first-webpage`.
2.  **Access Settings:**
    
    *   Click on the "Settings" tab located on the repository page.
3.  **Navigate to GitHub Pages Section:**
    
    *   In the sidebar, click on "Pages" (previously found under "Settings" > "Pages").
4.  **Configure GitHub Pages:**
    
    *   **Source:** Select the branch to publish from (usually `main`).
    *   **Folder:** Choose `/root` if your `index.html` is in the root directory.
    *   Click "Save."
5.  **Access Your Published Web Page:**
    
    *   After a few minutes, GitHub will provide a URL (e.g., `https://your-username.github.io/my-first-webpage/`) where your web page is live.

**Concepts Introduced:**
------------------------

*   **GitHub Pages:** A service to host static websites directly from a GitHub repository.
*   **Branch:** A separate version of your repository; `main` is the default branch.
*   **Static Website:** A website with fixed content, as opposed to dynamic websites that can change based on user interaction.

9\. Conclusion and Self-Test Questions
--------------------------------------

Congratulations! You’ve successfully built and published your first web page using HTML, CSS, and GitHub Pages through pair programming. To reinforce your learning, test your understanding with the following questions.

### **Self-Test Questions**

1.  **Pair Programming**
    
    *   What are the two roles in pair programming?
    *   Name one benefit of pair programming.
2.  **GitHub Repository**
    
    *   What is a repository on GitHub?
    *   What is the purpose of a README file?
3.  **Cloning the Repository**
    
    *   What does the `git clone` command do?
    *   Why is cloning a repository useful?
4.  **Development Environment**
    
    *   What is the purpose of a code editor like VS Code?
    *   Why is Git important in web development?
5.  **HTML Basics**
    
    *   What does the `<title>` tag define?
    *   How do you create a paragraph in HTML?

6.  **CSS Basics**
    
    *   What is the syntax for a CSS rule?
    *   Name two CSS properties used to style text.
7.  **Committing Changes**
    
    *   What command stages your changes for committing?
    *   What is the purpose of a commit message?
8.  **Pushing to GitHub**
    
    *   What does the `git push` command do?
    *   Why is pushing changes to GitHub important?
9.  **GitHub Pages**
    
    *   What is GitHub Pages used for?
    *   After setting up GitHub Pages, where can you view your published web page?
10.  **General Concepts**
    
    *   What is the root element in an HTML document?
    *   How do you add CSS directly within an HTML file?
    *   What does `<!DOCTYPE html>` declare?
    *   What is a static website?
    *   What is the default branch name in a new GitHub repository?
    *   How do you navigate to a directory in the command line?
    *   What does the `<h1>` tag represent in HTML?
    *   What is the function of the `<style>` tag in HTML?

**Answers:**

1.  **Pair Programming**
    
    *   **Roles:** Driver and Navigator.
    *   **Benefit:** Enhanced learning or improved code quality.
2.  **GitHub Repository**
    
    *   **Repository:** A storage space for your project on GitHub.
    *   **README File:** Describes your project.
3.  **Cloning the Repository**
    
    *   **`git clone`:** Creates a local copy of a remote repository.
    *   **Usefulness:** Allows you to work on the project locally.
4.  **Development Environment**
    
    *   **Code Editor Purpose:** Used to write and edit code.
    *   **Git Importance:** Manages and tracks changes in the codebase.
5.  **HTML Basics**
    
    *   **`<title>` Tag:** Defines the title of the web page shown in the browser tab.
    *   **Paragraph Creation:** `<p>Your text here.</p>`
6.  **CSS Basics**
    
    *   **CSS Rule Syntax:** `selector { property: value; }`
    *   **Text Styling Properties:** `color`, `font-size`.
7.  **Committing Changes**
    
    *   **Staging Command:** `git add index.html`
    *   **Commit Message Purpose:** Describes the changes made in a commit.
8.  **Pushing to GitHub**
    
    *   **`git push`:** Uploads local commits to GitHub.
    *   **Importance:** Shares your changes with others and updates the remote repository.
9.  **GitHub Pages**
    
    *   **Purpose:** To host and publish static websites from a GitHub repository.
    *   **View Published Page:** At the provided GitHub Pages URL (e.g., `https://your-username.github.io/my-first-webpage/`).
10.  **General Concepts**
    
    *   **Root Element:** `<html>`
    *   **Adding CSS:** Using the `<style>` tag within the `<head>` section.
    *   **`<!DOCTYPE html>`:** Declares the document type and version of HTML.
    *   **Static Website:** A website with fixed content.
    *   **Default Branch Name:** `main`
    *   **Navigate Directory:** `cd path/to/directory`
    *   **`<h1>` Tag:** Represents a top-level heading.
    *   **`<style>` Tag Function:** Embeds CSS styles within an HTML document.

Keep practicing and exploring more about HTML, CSS, and GitHub to enhance your web development skills. Happy coding!
