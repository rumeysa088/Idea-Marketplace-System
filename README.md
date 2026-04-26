<h1> Idea Marketplace System (Console-Based)</h1>

<h2> Project Description</h2>
<p>
The Idea Marketplace System is a console-based C++ application designed to connect innovators 
(who generate ideas) with investors (who are interested in funding or supporting ideas).
</p>

<p>
The system allows innovators to post ideas, and investors to browse, search, and show interest 
in those ideas. It also includes an evaluation system that analyzes ideas and assigns a score 
based on predefined criteria.
</p>

<h2> Core OOP Concepts Used</h2>
<ul>
  <li><strong>Encapsulation:</strong> Data is protected using private members with getters/setters.</li>
  <li><strong>Inheritance:</strong> Innovator and Investor inherit from the User class.</li>
  <li><strong>Polymorphism:</strong> Virtual functions like displayMenu() are overridden to provide role-specific behavior.</li>
  <li><strong>Abstraction:</strong> The Evaluator class defines a general evaluation structure using pure virtual functions.</li>
  <li><strong>File Handling:</strong> Persistent data storage is managed via text files to ensure data longevity.</li>
</ul>

<h2>Group Members</h2>
<p>
Name: Rumaisa Abbasi | Student ID: 25K-0585 <br>
Name: Rahia Sarfraz | Student ID: 25K-0546
</p>
<hr>

<h2> System Workflow </h2>

<ol>
  <li><strong>Initialization:</strong> The program starts and loads existing data from text files.</li>
  <li><strong>Authentication:</strong> The user chooses to Sign Up or Login to access their specific dashboard.</li>
  <li><strong>Role-Based Interaction:</strong>
    <ul>
      <li><strong>Innovator:</strong> Can post new ideas and trigger the evaluation engine.</li>
      <li><strong>Investor:</strong> Can browse, filter, and show interest in various ideas.</li>
    </ul>
  </li>
  <li><strong>Termination:</strong> Upon exiting the application, all data is automatically saved back to the files.</li>
</ol>

<h2> Use Cases </h2>

<ul>
    <li><strong>User Registration:</strong> A new user signs up as either an Innovator or Investor.</li>
    <li><strong>User Login:</strong> Existing users log in using username and password.</li>
    <li><strong>Post Idea (Innovator):</strong> Innovator enters idea details (title, description, category, value).</li>
    <li><strong>Browse Ideas (Investor):</strong> Investor views all available ideas posted by innovators.</li>
    <li><strong>Search/Filter Ideas:</strong> Investor searches ideas by title, category, or minimum value.</li>
    <li><strong>Show Interest in Idea:</strong> Investor selects an idea and submits an offer with a message.</li>
    <li><strong>View Personal Data:</strong> 
        <ul>
            <li>Innovator views their ideas</li>
            <li>Investor views their interests</li>
        </ul>
    </li>
    <li><strong>Idea Evaluation:</strong> System evaluates ideas and assigns a score and level (Beginner / Intermediate / Expert).</li>
</ul>

<hr>

<h2> Compilation Instructions</h2>
<p>Make sure all <code>.cpp</code> and <code>.h</code> files are in the same folder.</p>

<pre>
g++ *.cpp -o main
</pre>

<h2> Run Instructions</h2>
<pre>
./main
</pre>

<hr>

<h2> How to Use the System</h2>
<ol>
    <li>Start the program</li>
    <li>Choose from the main menu:
        <ul>
            <li>Sign Up</li>
            <li>Login</li>
            <li>Exit</li>
        </ul>
    </li>
    <li>After login:
        <ul>
            <li><strong>Innovators can:</strong>
                <ul>
                    <li>Post ideas</li>
                    <li>View their ideas</li>
                    <li>Evaluate ideas</li>
                </ul>
            </li>
            <li><strong>Investors can:</strong>
                <ul>
                    <li>Browse ideas</li>
                    <li>Search/filter ideas</li>
                    <li>Show interest</li>
                    <li>View interests</li>
                </ul>
            </li>
        </ul>
    </li>
    <li>Data is automatically saved to files when exiting</li>
</ol>

<hr>

<h2> File Handling</h2>
<p>The system uses text files to store persistent data:</p>
<ul>
    <li><code>innovators.txt</code></li>
    <li><code>investors.txt</code></li>
    <li><code>ideas.txt</code></li>
    <li><code>interests.txt</code></li>
</ul>

<hr>

<h2> Assumptions & Limitations</h2>
<ul>
    <li>Maximum users are limited (50 innovators, 50 investors)</li>
    <li>Maximum ideas/interests per user are fixed using arrays</li>
    <li>No GUI (console-based only)</li>
    <li>No password encryption (plain text storage)</li>
    <li>No real-time notifications (simulated via console)</li>
    <li>Idea evaluation is rule-based, not actual AI</li>
</ul>

<hr>

<h2> Key Features Summary</h2>
<ul>
    <li>Role-based system (Innovator / Investor)</li>
    <li>Idea posting and browsing</li>
    <li>Search and filtering functionality</li>
    <li>Interest submission system</li>
    <li>Evaluation scoring system</li>
    <li>File-based data persistence</li>
    <li>Proper OOP implementation</li>
</ul>
