<h1 id="teaching"></h1>

<h2 style="margin: 0px 0px 10px;">
    Teaching
    <a href="#" class="btn btn-sm z-depth-0" role="button" style="font-size:12px; color: #000000; border: 1px solid #000000; padding-left: 0.25rem; padding-right: 0.25rem;" onclick="event.preventDefault(); toggleSection(this, 'teaching-content');">
        Expand
    </a>
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
  function toggleSection(button, contentId) {
    var content = document.getElementById(contentId);
    if (content.style.display === "none" || content.style.display === "") {
      content.style.display = "block";
      button.innerHTML = "Collapse";
    } else {
      content.style.display = "none";
      button.innerHTML = "Expand";
    }
  }
</script>

<!-- Optional CSS for button styling -->
<!-- <style>
  .toggle-button {
    background: none;
    border: none;
    cursor: pointer;
    font-size: 12px;
    text-decoration: underline;
    color: #007bff;
  }

  .toggle-button:hover {
    text-decoration: none;
  }

  h2 {
    display: inline;
  }
</style> -->