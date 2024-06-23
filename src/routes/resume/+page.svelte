<script lang="ts">
  import Seo from "$lib/components/Seo.svelte";
  import Workplace from "./Workplace.svelte";
</script>

<Seo title="Kushal Juneja – Resume" />

<section class="layout-md py-12">
  <h2 class="heading2">Education</h2>

  <div class="mb-4">
    <div class="flex justify-between items-end">
      <h3 class="text-black text-lg">IIIT-Delhi</h3>
      <div class="text-neutral-500 mb-0.5">2019 — 2023</div>
    </div>
    <p class="byline">B.Tech. in Computer Science Engg</p>
  </div>

  <h4 class="font-medium mt-4 mb-1">Teaching:</h4>
  <ul>
    <li>TA for Distributed Systems, Winter 2023</li>
  </ul>

  <h4 class="font-medium mt-4 mb-1">Graduate-level technical coursework:</h4>
  <ul>
    <li>Theory of Computation</li>
    <li>Mobile Computing</li>
    <li>Statistical Machine Learning</li>
    <li>Big Data Analysis</li>
    <li>Natural Language Processing</li>
    <li>Graph Theory</li>
    <li>Data Mining</li>
  </ul>

  <h4 class="font-medium mt-4 mb-1">Undergraduate coursework:</h4>
  <ul>
    <li>Computer Networks</li>
    <li>Operating Systems</li>
    <li>Database Systems</li>
    <li>Data Structures and Algorithms</li>
    <li>Algorithm Design and Analysis</li>
    <li>Linear Algebra</li>
    <li>Probability and Statistics</li>
    <li>Prototyping Interactive Systems</li>
    <li>Abstract Algebra</li>
    <li>Microeconomics</li>
    <li>Foundations of Finance</li>
    <li>Portfolio Valuation and Management</li>
  </ul>
</section>

<section class="layout-md">
  <h2 class="heading2">Professional Experience</h2>

  <Workplace
    title="Analyst"
    company="Goldman Sachs"
    url="https://www.goldmansachs.com/"
    dates="July 2023 – Current"
    location="Bangalore, India"
  >
    <li>Doing something here...</li>
  </Workplace>

  <Workplace
    title="Summer Intern"
    company="Droom"
    url="https://droom.in"
    dates="May 2022 - July 2023"
    location="Gurugram, IN"
  >
    <li>Did something here using Golang, Oauth2 and micro-services...</li>
  </Workplace>

  <Workplace
    title="Research Intern"
    company="CAS-IITD"
    url="https://dcecm.iitd.ac.in/index.html"
    dates="Aug 2022 - May 2023"
    location="New Delhi, IN"
  >
    <li>Did some work on Climate Science here...</li>
  </Workplace>

  <Workplace
    title="Undergrad Researcher"
    company="LCS2-IIITD"
    url="https://lcs2.in"
    dates="Jan 2022 to May 2023"
    location="New Delhi, IN"
  >
    <li>Did some work on AI here...</li>
  </Workplace>

  <Workplace
    title="Intern"
    company="CAI - IIITD"
    url="https://iiitd.ac.in/"
    dates="Feb 2022 to March 2022"
    location="New Delhi, IN"
  >
    <li>Designed initial website for Centre for CAI, IIIT-Delhi.</li>
  </Workplace>

  <Workplace
    title="Teacher"
    company="Summer Camp - IIITD"
    url="https://iiitd.ac.in/"
    dates="May 2022 to July 2022"
    location="New Delhi, IN"
  >
    <li>
      Volunteered to teach school students logical reasoning and english via
      online zoom lessons during covid times. Also gave a talk on JEE prep.
    </li>
  </Workplace>
</section>

<style lang="postcss">
  b {
    @apply font-medium;
  }

  ul {
    @apply list-disc pl-7 marker:text-neutral-400;
  }

  .byline {
    @apply font-serif italic;
  }
</style>
