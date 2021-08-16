# Learn-0.2
## Python

You  guys might've finished the previous module, [Learn-0.1](https://github.com/Training-2024/Learn-0.1), if not, make sure you finish that first!<!--first finish that and then visit this module.--> Now we're going to discuss about the most widely used programming language that can be used in every technical domain, some of them are:<!--stating some of them,--> Artificial Intelligentce, Machine Learning, Data Science, Ethical Hacking, and the list goes on!<!--if I state everything then it'll take another repo for explaining the applications only -->Let us get into the topic now.

Python is a widely used high-level programming language for general-purpose programming, created by Guido van Rossum and first released in 1991. Python features a dynamic type system and automatic memory management and supports multiple programming paradigms, including object-oriented, imperative, functional programming, and procedural styles. It has a large and comprehensive standard library.

As <!--previously-->told in the First Module, our **Robotics Club** <!--is promoting-->encourages and expects **_SELF LEARNING_**. So you guys might have understood what to do now...

This is the most important & essential step in this whole Training-2024 Program. <!--So-->Learning python is mandatory. Use these resources that we have curated for you to learn Python.

- [Python Tutorials](https://github.com/Training-2024/Learn-0.2/tree/main/python_tutorials)

You can ask your doubts to the assigned mentors.
<hr/>
<h2>Task Description</h2>
<li>
<a href='https://github.com/Training-2024/Learn-0.2/tree/main/task1'>Task files</a>
</li>
<h2><a class="header" href="#aim" id="aim">Aim</a></h2>
<p>You are TA (Teaching Assistant) under a Professor in an academic institution. The end semester exams have been conducted for 5 subjects. Now the crucial task of gathering the data is to be done.</p>
<p>Professor has given you a CSV file with 6 columns, where the first column contains the name of student and the subsequent 5 columns contain the marks of that particular student gained in 5 subjects.</p>
<ul>
<li>
<p>Read the given CSV file and store the data in a Python dictionary. You need to then calculate the percentage of each student and give them a grade accordingly.</p>
</li>
<li>
<p>The grades are to be given by following the below rule:</p>
<ul>
<li>Percentage <strong>equal to or above 90%</strong> is given the grade <strong>'O'</strong></li>
<li>Percentage <strong>equal to or above 70%</strong> is given the grade <strong>'A'</strong></li>
<li>Percentage <strong>equal to or above 60%</strong> is given the grade <strong>'B'</strong></li>
<li>Percentage <strong>equal to or above 50%</strong> is given the grade <strong>'C'</strong></li>
<li>Percentage <strong>equal to or above 40%</strong> is given the grade <strong>'D'</strong></li>
<li>Percentage <strong>below 40%</strong> is given the grade <strong>'Fail'</strong></li>
</ul>
</li>
<li>
<p>Generate the Grade Card for all in the form of Python dictionary in the following manner:</p>
<pre><code class="language-python">{
	'name_of_the_student': {
		'subject_wise_marks': [subject1_marks, subject2_marks, subject3_marks,
								subject4_marks, subject5_marks],
		'grade_received': 'A'
	}
}
</code></pre>
</li>
<li>
<p>The skeleton code stub provided is to be used. It calls the functions <strong><code>readMarkSheet()</code></strong> and <strong><code>generateGradeCard()</code></strong>. Your task is to modify and complete these functions.</p>
</li>
</ul>
<hr />
<h2><a class="header" href="#given" id="given">Given</a></h2>
<p>Two files are provided to solve this task.</p>
<ul>
<li>Skeleton program file: <strong><code>task1.py</code></strong>
<ul>
<li>The skeleton consists of three functions which you have to modify:
<ul>
<li><strong><code>readMarkSheet()</code></strong></li>
<li><strong><code>generateGradeCard()</code></strong></li>
</ul>
</li>
</ul>
</li>
<li>Sample CSV file: <strong><code>task1_sample.csv</code></strong>
<ul>
<li>The CSV file has 6 columns: <strong><code>name</code></strong>, <strong><code>subject_1</code></strong>, <strong><code>subject_2</code></strong>, <strong><code>subject_3</code></strong>, <strong><code>subject_4</code></strong> and <strong><code>subject_5</code></strong>.</li>
</ul>
</li>
</ul>
<hr />
<h2><a class="header" href="#procedure" id="procedure">Procedure</a></h2>
<ul>
<li>
<p>Open the skeleton program file, <strong><code>task1.py</code></strong>.</p>
</li>
<li>
<p>You will notice pre-written comments included in skeleton program for your assistance to solve this task.</p>
</li>
<li>
<p>Two functions to modify are:</p>
<ul>
<li>
<h3><a class="header" href="#readmarksheet" id="readmarksheet"><strong><code>readMarkSheet()</code></strong></a></h3>
<table><thead><tr><th>Function Name</th><th align="center"><code>readMarkSheet()</code></th></tr></thead><tbody>
<tr><td><strong>Purpose</strong></td><td align="center">Reads the input CSV file of Mark Sheet and creates a mapping of student name with his/her marks for each subject.</td></tr>
<tr><td><strong>Input Arguments</strong></td><td align="center"><strong><code>file_name</code></strong> : [ <em><strong>str</strong></em> ] <br> CSV file name of Mark Sheet</td></tr>
<tr><td><strong>Output Arguments</strong></td><td align="center"><strong><code>name_marks_mapping</code></strong> : [ <em><strong>dict</strong></em> ] <br>Mapping of each student's name and his/her marks for each subject as { Key : Value } pair</td></tr>
<tr><td><strong>Example Call</strong></td><td align="center"><em><strong>name_marks_mapping = readMarkSheet(csv_file_name)</strong></em></td></tr>
</tbody></table>
<br>
</li>
<li>
<h3><a class="header" href="#generategradecard" id="generategradecard"><strong><code>generateGradeCard()</code></strong></a></h3>
<table><thead><tr><th>Function Name</th><th align="center"><code>generateGradeCard()</code></th></tr></thead><tbody>
<tr><td><strong>Purpose</strong></td><td align="center">Generate the Grade Card for all students in the given mapping of student and their scores in all subjects with the grade each one has received.</td></tr>
<tr><td><strong>Input Arguments</strong></td><td align="center"><strong><code>mapping_dict</code></strong> : [ <em><strong>dict</strong></em> ] <br>Mapping of each student's name and his/her marks for each subject as { Key : Value } pair</td></tr>
<tr><td><strong>Output Arguments</strong></td><td align="center"><strong><code>grade_card</code></strong> : [ <em><strong>dict</strong></em> ] <br>Grade Card for all students with their scores in all subjects and the grade each one has received</td></tr>
<tr><td><strong>Example Call</strong></td><td align="center"><em><strong>grade_card = generateGradeCard(name_marks_mapping)</strong></em></td></tr>
</tbody></table>
<br>
</li>
</ul>
</li>
<h2><a class="header" href="#expected-output" id="expected-output">Expected Output</a></h2>
<ul>
<li>
<p>The provided sample CSV file, <strong><code>task1_sample.csv</code></strong> consists data with fields <em><strong>name</strong></em>, <em><strong>subject_1</strong></em>, <em><strong>subject_2</strong></em>, <em><strong>subject_3</strong></em>, <em><strong>subject_4</strong></em> and <em><strong>subject_5</strong></em>.</p>
</li>
<li>
<p>The content of this CSV file is shown below:</p>
<pre><code class="language-spreadsheet">name,subject_1,subject_2,subject_3,subject_4,subject_5
Artus Syne,43,71,55,16,51
Evey Reburn,49,7,53,50,63
Giff Wickmann,63,37,21,87,9
Garrot Casetta,22,3,91,75,52
Roselle Maes,71,90,96,79,48
Torin Ziehms,71,31,83,1,25
Jaye Etock,92,9,2,78,55
Thomasina Tinkham,25,78,46,46,90
Adolphus Biernat,91,96,98,94,100
Rex Aspinell,34,75,51,38,99
</code></pre>
</li>
<li>
<p>The expected output of program <strong><code>task1.py</code></strong> i.e., to generate the Grade Card for each student is shown below:</p>
<pre><code class="language-python">
{
	  'Artus Syne': {'marks': [43.0, 71.0, 55.0, 16.0, 51.0]},
    'Evey Reburn': {'marks': [49.0, 7.0, 53.0, 50.0, 63.0]},
    'Giff Wickmann': {'marks': [63.0, 37.0, 21.0, 87.0, 9.0]},
    'Garrot Casetta': {'marks': [22.0, 3.0, 91.0, 75.0, 52.0]},
    'Roselle Maes': {'marks': [71.0, 90.0, 96.0, 79.0, 48.0]},
    'Torin Ziehms': {'marks': [71.0, 31.0, 83.0, 1.0, 25.0]},
    'Jaye Etock': {'marks': [92.0, 9.0, 2.0, 78.0, 55.0]},
    'Thomasina Tinkham': {'marks': [25.0, 78.0, 46.0, 46.0, 90.0]},
    'Adolphus Biernat': {'marks': [91.0, 96.0, 98.0, 94.0, 100.0]},
    'Rex Aspinell': {'marks': [34.0, 75.0, 51.0, 38.0, 99.0]}
}
{
	'Artus Syne': {'subject_wise_marks': [43.0, 71.0, 55.0, 16.0, 51.0], 'grade_received': 'D'}, 
	'Evey Reburn': {'subject_wise_marks': [49.0, 7.0, 53.0, 50.0, 63.0], 'grade_received': 'D'}, 
	'Giff Wickmann': {'subject_wise_marks': [63.0, 37.0, 21.0, 87.0, 9.0], 'grade_received': 'D'}, 
	'Garrot Casetta': {'subject_wise_marks': [22.0, 3.0, 91.0, 75.0, 52.0], 'grade_received': 'D'}, 
	'Roselle Maes': {'subject_wise_marks': [71.0, 90.0, 96.0, 79.0, 48.0], 'grade_received': 'A'}, 
	'Torin Ziehms': {'subject_wise_marks': [71.0, 31.0, 83.0, 1.0, 25.0], 'grade_received': 'D'}, 
	'Jaye Etock': {'subject_wise_marks': [92.0, 9.0, 2.0, 78.0, 55.0], 'grade_received': 'D'}, 
	'Thomasina Tinkham': {'subject_wise_marks': [25.0, 78.0, 46.0, 46.0, 90.0], 'grade_received': 'C'}, 
	'Adolphus Biernat': {'subject_wise_marks': [91.0, 96.0, 98.0, 94.0, 100.0], 'grade_received': 'O'}, 
	'Rex Aspinell': {'subject_wise_marks': [34.0, 75.0, 51.0, 38.0, 99.0], 'grade_received': 'C'}
}
</code></pre>
</li>
<li>
 <p>The first twelve lines above are the output of <strong><code>readMarkSheet</code></strong> function i.e. variable <strong><code>name_marks_mapping</code></strong> and,</p>
<p>the lines 13 to 24 are the output of <strong><code>generateGradeCard</code></strong> function i.e. variable <strong><code>grade_card</code></strong>.</p>
</li>
</ul>
<hr />
