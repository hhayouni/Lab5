
<h2>I/O Redirection: Standard Output</h2>
<ul>
  <li><strong>Default Standard Output</strong>: The screen is the default for standard output.</li>
  <li><strong>Redirection to File</strong>: Use <code>></code> after a command (e.g., <code>ls > file.txt</code>) to redirect output to a file.</li>
  <li><strong>Command Example</strong>: <code>cat file.txt</code> displays the content of <code>file.txt</code>.</li>
</ul>

<br>

<h3>Appending Output:</h3>
<ul>
  <li><strong>Append using <code>>></code></strong>: Adds output to an existing file or creates a new one if it doesn’t exist (e.g., <code>echo "Hello" >> file.txt</code>).</li>
</ul>

<hr>

<h2>I/O Redirection: Standard Input</h2>
<ul>
  <li><strong>Default Standard Input</strong>: From the keyboard.</li>
  <li><strong>Input from File</strong>: Redirect input from a file using <code><</code> (e.g., <code>command < inputfile.txt</code>).</li>
  <li><strong>Combining Input and Output Redirection</strong>: Both <code><</code> and <code>></code> can be used together on the same line.</li>
</ul>

<hr>

<h2>Pipelines (<code>|</code>)</h2>
<ul>
  <li><strong>Chaining Commands</strong>: Use a pipeline to pass the output of one command to the input of another (e.g., <code>command1 | command2 | command3</code>).</li>
</ul>

<hr>

<h2>Expansion</h2>
<ul>
  <li><strong>Special Characters</strong>: Characters like <code>*</code>, <code>?</code>, and others have expanded meanings in shell commands.</li>
</ul>

<hr>

<h2>Tip: Backslash (<code>\</code>)</h2>
<ul>
  <li><strong>Multi-line Command</strong>: Use a backslash to continue a long command over multiple lines (e.g., <code>command \</code> followed by pressing "Enter").</li>
</ul>

<hr>

<h2>Permissions in Linux</h2>
<ul>
  <li><strong>Multi-User System</strong>: Linux supports multiple users, and permissions are assigned differently to the owner, group, and others.</li>
  <li><strong>Changing Permissions</strong>: Use the <code>chmod</code> command to change file or directory permissions.</li>
</ul>

<pre><code># Example:
chmod 600 file.txt  # rw- for the owner, no permissions for others.
</code></pre>

<hr>

<h2>Superuser (<code>sudo</code>)</h2>
<ul>
  <li><strong>System Administration</strong>: A superuser has administrative privileges.</li>
  <li><strong>Running Commands with <code>sudo</code></strong>: Some commands require superuser access. Prefix such commands with <code>sudo</code>.</li>
</ul>

<pre><code>sudo command  # Run the command with superuser privileges.
</code></pre>

<hr>

<h2>Text Editors in Linux</h2>
<ul>
  <li><strong>Options</strong>: CLI-based and GUI-based text editors are available. Examples include <code>nano</code>, <code>vim</code>, and graphical editors.</li>
</ul>

<hr>

<h2>Shell Script</h2>
<ul>
  <li><strong>Writing Scripts</strong>: You can write and execute shell scripts. If issues arise in a text editor, files can be edited with a simple text editor like Notepad.</li>
</ul>

<hr>

<h2>Command History</h2>
<ul>
  <li><strong>Viewing History</strong>: Use the <code>history</code> command to display previously executed commands. You can save this output to a file.</li>
</ul>

<hr>

<h2><code>wget</code></h2>
<ul>
  <li><strong>Downloading Files</strong>: The <code>wget</code> command is used to download files directly from the internet into the current directory.</li>
</ul>

<pre><code>wget http://example.com/file.zip
</code></pre>

<hr>

<h2><code>curl</code></h2>
<ul>
  <li><strong>Fetching Data</strong>: The <code>curl</code> command is for fetching, uploading, and managing data over the Internet.</li>
</ul>

<pre><code>curl [options] [URL]
</code></pre>

<hr>

<h2><code>grep</code></h2>
<ul>
  <li><strong>Searching Text</strong>: Use <code>grep</code> to search for text within files.</li>
</ul>

<pre><code>grep "search_term" file.txt
</code></pre>

<h3>Common <code>grep</code> Options:</h3>
<ul>
  <li><code>-i</code>: Case-insensitive search.</li>
  <li><code>-v</code>: Invert match (exclude lines with the search term).</li>
  <li><code>-n</code>: Show line numbers with matches.</li>
  <li><code>-r</code>: Recursive search through directories.</li>
</ul>

<h3>grep supports powerful regular expressions for more complex searches.</h3>
<ul>
  <li><code>.*</code>: Matches any character zero or more times.</li>
  <li><code>/d</code>: Matches any digit(0~9).</li>
  <li><code>[abc]</code>: Matches any single character within the brackets.</li>
  <li><code>^</code>: Matches the beginning of a line.</li>
  <li><code>$</code>: Matches the end of a line.</li>
</ul>
<hr><li><code>^</code>: Recursive search through directories.</li>
