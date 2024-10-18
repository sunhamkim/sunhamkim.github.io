<h1 id="teaching"></h1>

<h2 style="margin: 0px 0px 10px;">
    Teaching
    <button class="toggle-btn" id="toggle-icon" onclick="toggleSection('teaching-content')">Show</button>
</h2>

<div id="teaching-content" style="display:none;">
  <!-- Purdue University Section -->
  <h4 style="margin:0 10px 0;">Instructor, Purdue University</h4>
  <ul style="margin:0 0 5px;">
    <li>Microeconomics (Summer 2019), <a href="./files/pdf/TeachingEvalSU19.PDF" target="_blank">Instructor Eval 4.7/5.0</a> (Award: Krannert Certificate for Distinguished Teaching)</li>
    <li>Intro to Causal Inference (Fall 2022), Volunteer for Purdue Econ Assoc. (Undergrad Club)</li>
  </ul>

  <!-- Purdue TA Section -->
  <h4 style="margin:0 10px 0;">Teaching Assistant, Purdue University</h4>
  <ul style="margin:0 0 5px;">
    <li>Undergraduate: Principles of Economics (Fall 2017), Macroeconomics (Spring 2018), International Trade (Spring 2021, 2023), Labor Economics (Summer 2022, Spring 2023)</li>
    <li>PhD: Microeconomics II (Fall 2018)</li>
  </ul>

  <!-- Yonsei University Section -->
  <h4 style="margin:0 10px 0;">Teaching Assistant, Yonsei University</h4>
  <ul style="margin:0 0 5px;">
    <li>Undergraduate: Labor Economics (Spring 2014-2016), Microeconomics (Spring 2015-2016)</li>
    <li>Graduate: Labor Economics (Spring 2014-2016)</li>
    <li>MBA: Personnel Economics (Fall 2015-Spring 2016), Microeconomics (Spring 2015-2016)</li>
  </ul>
</div>

<!-- JavaScript to toggle the section -->
<script>
  function toggleSection(id) {
    var section = document.getElementById(id);
    var button = document.getElementById('toggle-icon');
    if (section.style.display === "none") {
      section.style.display = "block";
      button.innerHTML = "Hide";
    } else {
      section.style.display = "none";
      button.innerHTML = "Show";
    }
  }
</script>

<!-- Optional CSS for button styling -->
<style>
  .toggle-btn {
    background: none;
    border: none;
    cursor: pointer;
    font-size: 16px;
  }
</style>