<h1 align="center">Hi 👋, I'm Shubhangi Kore</h1>
<h3 align="center">Final-Year IT Student  • Java Developer • Full-Stack Developer •Frontend Developer </h3>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=18&pause=1000&color=0F62FE&center=true&vCenter=true&width=500&lines=Java+%7C+React.js+%7C+Developer;AWS+Cloud+Practitioner+Certified;Building+Real-World+Projects;Open+to+Software+Developer+Roles" alt="Typing SVG" />
</p>

---

### 👩‍💻 About Me

- 🎓 Final-year **B.E. Information Technology** student at Amrutvahini College of Engineering (CGPA: **9.4**)
- 💼 Seeking **Associate System Engineer / Software Engineer** roles
- 🔭 Currently working on: **Real-Time Collaborative Code Editor** (React.js + Node.js)
- ⚡ Fun fact: I love breaking problems into smaller piece — both in code and in life!

---

### 🛠️ Tech Stack

<p align="center">
  <img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white"/>
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black"/>
  <img src="https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white"/>
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white"/>
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white"/>
</p>
<p align="center">
  <img src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB"/>
  <img src="https://img.shields.io/badge/MySQL-00000F?style=for-the-badge&logo=mysql&logoColor=white"/>
  <img src="https://img.shields.io/badge/JDBC-007396?style=for-the-badge&logo=java&logoColor=white"/>
</p>
<p align="center">
  <img src="https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazon-aws&logoColor=white"/>
  <img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black"/>
  <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white"/>
  <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"/>
  <img src="https://img.shields.io/badge/VS_Code-007ACC?style=for-the-badge&logo=visual-studio-code&logoColor=white"/>
</p>

---
### 🚀 Featured Projects

#### 🖥️ Real-Time Collaborative Code Editor
> React.js • Node.js • Express.js • Socket.io • React Router

- Multi-user real-time code collaboration with sub-100ms latency
- Modular REST APIs + event-driven WebSocket architecture
- Session-based access control and secure routing
- 🔗 [View Repository](https://github.com/shubhangickore/Code_Editor)

---

#### 📝 Online Examination System
> Java Servlets • JSP  • JDBC • MySQL • MVC Architecture

- Secure authentication + time-bound assessments with role-based access
- Normalised MySQL schema with transaction management
- Clean MVC separation — maintainable, production-style codebase
- 🔗 [View Repository](https://github.com/shubhangickore/OnlineExamSystem.git)

---

#### ☕ Java Coding Practice
> Java • LeetCode • Data Structures & Algorithms

- Organized solutions across Arrays, Strings, LinkedLists, Trees and more
- Actively growing with consistent daily practice
- 🔗 [View Repository](https://github.com/shubhangickore/Coding-Practice)



---
### 📬 Connect With Me

<p align="center">
  <a href="/cdn-cgi/l/email-protection#98f3f7eafdebf0edfaf0f9f6fff1aaa1a9d8fff5f9f1f4b6fbf7f5">
    <img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white"/>
  </a>
  <a href="https://linkedin.com/in/shubhangi-kore" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/>
  </a>
  <a href="https://github.com/shubhangickore" target="_blank">
    <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"/>
  </a>
  <a href="https://leetcode.com/u/shubhangi_kore/" target="_blank">
    <img src="https://img.shields.io/badge/LeetCode-FFA116?style=for-the-badge&logo=leetcode&logoColor=white"/>
  </a>
</p>

---

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=shubhangickore&label=Profile+Views&color=0F62FE&style=flat" alt="profile views" />
</p>



<p>Berkeley Algorithm :</p>
 BerkeleyAlgorithm.java
import java.util.*;

public class BerkeleyAlgorithm {

   public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        System.out.print("Enter number of clocks (including server): ");
        int n = sc.nextInt();

        int[] time = new int[n];

        // Input clock times
        for (int i = 0; i < n; i++) {
            System.out.print("Enter time of clock " + i + ": ");
            time[i] = sc.nextInt();
        }

        int serverTime = time[0]; // assume first clock is server
        int sumDiff = 0;

        System.out.println("\n--- Time Differences w.r.t Server ---");

        int[] diff = new int[n];

        for (int i = 0; i < n; i++) {
            diff[i] = time[i] - serverTime;
            System.out.println("Clock " + i + " difference = " + diff[i]);
            sumDiff += diff[i];
        }

        // Calculate average difference
        int avgDiff = sumDiff / n;

        System.out.println("\nAverage Difference = " + avgDiff);

        // Adjust times
        System.out.println("\n--- Adjusted Times ---");

        for (int i = 0; i < n; i++) {
            int adjustedTime = time[i] - diff[i] + avgDiff;
            System.out.println("Clock " + i + " adjusted time = " + adjustedTime);
        }

        sc.close();
    }
}

