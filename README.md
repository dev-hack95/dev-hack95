
<p>
  <h1 align="center"><b>Hello there, I'm Saiprasad Toshatwad </b></h1>
</p>

<div id="header" align="center">
  <img src="https://media0.giphy.com/media/M9gbBd9nbDrOTu1Mqx/giphy.gif?cid=790b7611021c6f00b63ed67cb3038f7ef33aff0ad0464ca1&rid=giphy.gif&ct=s" width="200"/>
</div>

<div id="badges" align="center">
  <a href="https://www.linkedin.com/in/saiprasad-toshatwad-a75449206/">
    <img src="https://img.shields.io/badge/LinkedIn-blue?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn Badge"/>
  </a>
</div>

### 👨‍💻: About Me :
#### I am a Data Scientist and Backend engineer.

- :telescope: I’m a Data Scientist and working on ML/DL models and backend for building Machine learning  applications.
- 🥅 2024 Goals: To become a Full Stack Data Scientist , MLOps and LLMOps Pro
- :zap: In my free time, I read tech articles on medium and watch anime.
- 📬 How to reach me: saiprasadtoshatwad@gmail.com

### :hammer_and_wrench: Tech Stack:

#### Data Science Stack
- Python, Data visualization, Supervised Learning algo, Unsupervised Learning algos, ANN, EDA, feature enginnering, feature selection & extraction,
Scikit-Learn, Tensorflow, Xgboost, Numpy , Pandas, Scipy, Beautiful Soup, Flask, Fastapi, .. etc


#### Devops/Mlops
- Linux,  [DVC](https://dvc.org/), [Mlflow](https://mlflow.org/), CI/CD, Jenkins, Docker, Kubernetes,  AWS, S3, EC2, lambda, boto3, [kedro](https://kedro.org/), ![](https://github.githubassets.com/images/modules/site/features/actions-icon-actions.svg)
- Go, Raspberry pi

#### Python Packges , Frameworks and Databases
- Scikit-Learn, Tensorflow, Xgboost, Numpy , Pandas, Scipy, Beautiful Soup, Flask, Fastapi
- Mysql, Postgresql

#### BI Tools
- PowerBI,  Tableau

# 📊 GitHub Stats:
![](https://github-readme-streak-stats.herokuapp.com/?user=dev-hack95&theme=vue-dark&hide_border=false)<br/>
![](https://github-readme-stats.vercel.app/api/top-langs/?username=dev-hack95&theme=vue-dark&hide_border=false&include_all_commits=false&count_private=false&layout=compact)
---

## 🏆 GitHub Trophies
![](https://github-profile-trophy.vercel.app/?username=dev-hack95&theme=chalk&no-frame=false&no-bg=true&margin-w=4)

---
<!doctype html>
<html>
<head>
  <title>D3 tutorial</title>
  <!--[if lte IE 8]><script src="r2d3.min.js" charset="utf-8"></script><![endif]-->
  <!--[if gte IE 9]><!-->
  <script src="http://d3js.org/d3.v3.min.js"></script>
  <!--<![endif]-->
  <script src="https://google-code-prettify.googlecode.com/svn/loader/prettify.js"></script>
  <link href="https://google-code-prettify.googlecode.com/svn/loader/prettify.css" type="text/css" rel="stylesheet" />
</head>
<h3>Transitions</h3>
<h4>Basic Animations in D3, part2</h4>
<a href="index.html">Back to table of contents</a>
<body onload="prettyPrint()">
<pre class="prettyprint">
    /**
     * Script draws circle, 2 seconds after drawing the circle, move the circle to the right.
     * set the time moving to the right for about 1.5 secs.
     * Also showcases the ability to have basic animated sequences:
     * move right, move down, move left.
     */
    var width = 500;
    var height = 500;
    var canvas = d3.select("body")
                  .append("svg")
                  .attr("width", width)
                  .attr("height", height);
    var circle = canvas.append("circle")
                  .attr("cx", 50)
                  .attr("cy", 50)
                  .attr("r", 25);
    // on circle object render
    circle.transition()
      // move circle to the right
      .attr("cx", 150)
      // set the length of time moving to 1.5 secs (1500 milliseconds)
      .duration(1500)
      // but start the transition 2 seconds after object render
      .delay(2000)
      // new sequence move a little to the bottom
      .transition()
      .attr("cy", 200)
      // new sequence move a little to the left.
      .transition()
      .attr("cx", 50);
</pre>
  <script>
    var width = 500;
    var height = 500;
    var canvas = d3.select("body")
                  .append("svg")
                  .attr("width", width)
                  .attr("height", height);
    var circle = canvas.append("circle")
                  .attr("cx", 50)
                  .attr("cy", 50)
                  .attr("r", 25);
    circle.transition()
      .attr("cx", 150)
      .duration(1500)
      .delay(2000)
      .transition()
      .attr("cy", 200)
      .transition()
      .attr("cx", 50);
  </script>
</body>
</html>
