<h1>SQL100</h1>
<h2> 100 Exercises on Structured Query Language</h2>

<a href="https://sql100.pythonanywhere.com" target="_blank">https://sql100.pythonanywhere.com</a>

<img src="https://github.com/Oyebamiji-Micheal/Sql100/blob/main/images/img_pc.png" height="500" width="500"/>

<br/>

<h2>Table of Contents</h2>

- [Project Description](#project-description)
- [Limitations](#limitations)
- [Running Locally](#running-locally)
- [Resources](#resources)
- [Source Code](#source-code)
- [Contact](#contact)


<br/>

<a id='description'></a>

## Project Description
<p align="justify">
    Thus far have I come in my learning. This is the second project in the <a href="https://github.com/Oyebamiji-Micheal/100-Days-of-SQL-Beginner-to-Advance">100daysofsql challenge</a> I started a few months ago. During the challenge, one of the major issues I faced was finding a site with a lot of practice questions. Most sites either require paying a stipend while others require a relatively high amount before users can run queries. The primary objective of this project is to provide an alternative to anyone who wishes to practice structured query language for free. I am not an SQL expert nor a database analyst but the little I can offer have I offered. <br/>
    This project was deployed to <a href="https://www.pythonanywhere.com/">PythonAnywhere</a> using a free tier account, any support to help scale it up is very much welcomed. You can reach me using any of the media outlined in the <a href="#contact">contact section</a>.
</p>

<br/>

<a id='limitations'></a>

## Limitations
<p align="justify">
    While working on this project locally, I used MySQL Server 8.0.28 which allowed the flexibility of using <strong>Window Functions, Stored Procedures, Functions</strong> and some other cool concepts. However, the problem started during deployment to PythonAnywhere's free tier account which uses a MySQL server version of 5.7.34. A lot of problems were encountered due to a change in server versions.
    The first problem came with Window Functions which was not supported until version 8.0 (April 19, 2018). To my surprise, the queries below are not equivalent i.e. one can't be used in place of the other

  ```SQL
      SELECT * FROM Students LIMIT 5;
      SELECT * FROM students LIMIT 5;
  ```

  To further this conundrum 😞, queries that involve ordering on a column containing duplicates yield different results when execute multiple times. To this end, most questions had to be adjusted and a few queries had to be rewritten to allow for compatibility. If you, therefore, notice an unusual output, consider the server version while writing queries. If you encountered a bug or observed something else such as an incorrect answer or query result, kindly use the discussion section or reach me using any of the media outlined in the <a href="#contact">contact section</a>. This project wasn't meant to be deployed to a specific website from the start, if server versions had been considered, issues involving compatibility and the ones mentioned earlier would be completely avoided. 

</p>

<br/>

<a id='running-locally'></a>

## Running Locally
<p align="justify">
    For the sake of practice with different RDMS and server versions, all datasets used in this project have been made available and can be found <a href="https://github.com/Oyebamiji-Micheal/Sql100/tree/main/datasets">here</a>. <br/>
    NB: These datasets were generated programmatically with a few python scripts; they are not and should not be assumed to be a reflecting of a real world data!
</p>

<br/>

<a id='resources'></a>

## Resources
- [MySQL Documentation(5.7)](https://dev.mysql.com/doc/refman/5.7/en/)
- [MySQL Documentation(8.0)](https://dev.mysql.com/doc/refman/8.0/en/)
- [javaTpoint](https://javatpoint.com/)
- MySQL Beginner to Expert - Colt Steele

<br/>

## Source Code
This project's source code has been pushed to a private repository. If you wish to contribute by adding more features or questions, kindly reach out to me.

<br/>

## Contact
You can contact me using any of the media below
- Gmail - oyebamijimicheal10@gmail.com
- LinkedIn - https://www.linkedin.com/in/oyebamiji-micheal
- Twitter - @MichealOjuri
- WhatsApp - +234 7019113012

<br/><br/>

<img src="https://github.com/Oyebamiji-Micheal/Sql100/blob/main/images/home_page_pc.png" height="550" width="550"/>