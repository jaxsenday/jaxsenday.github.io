---
layout: default
title: CV
permalink: /cv/
---

<div class="section-head">
  <div>
    <p class="eyebrow">Curriculum Vitae</p>
    <h1>Jaxsen R. Day</h1>
  </div>
  {% if site.data.site.profile.cv_file and site.data.site.profile.cv_file != "" %}
    <a class="button-link button-link--solid" href="{{ site.data.site.profile.cv_file | relative_url }}">Download CV (.docx)</a>
  {% endif %}
</div>

<section class="section grid two-up">
  <section class="panel">
    <h2>Current Appointment</h2>
    <p>{{ site.data.site.profile.title }}</p>
    <p>{{ site.data.site.profile.institution }}</p>
    <p>{{ site.data.site.profile.location }}</p>
    <p><a href="mailto:{{ site.data.site.profile.email }}">{{ site.data.site.profile.email }}</a></p>
  </section>

  <section class="panel accent-panel">
    <h2>Research Interests</h2>
    <ul class="pill-list" aria-label="Research interests">
      {% for item in site.data.site.research_interests %}
        <li>{{ item }}</li>
      {% endfor %}
    </ul>
  </section>
</section>

<section class="section">
  <div class="section-head">
    <h2>Educational Background</h2>
  </div>
  <ul class="card-list">
    <li>
      <h3>Ph.D., Information Studies</h3>
      <p class="meta">In progress &middot; iSchool, The University of Texas at Austin</p>
      <p><strong>Doctoral Committee:</strong> Dr. Kenneth R. Fleischmann (Chair), Dr. R. David Lankes, Dr. Danna Gurari, Dr. Soo Young Rieh, Dr. Abigale Stangl</p>
    </li>
    <li>
      <h3>M.Ed., Management of Technical Education</h3>
      <p class="meta">2019 &middot; College of Education, Texas State University</p>
    </li>
    <li>
      <h3>B.B.A., Computer Information Systems</h3>
      <p class="meta">2017 &middot; Emmett &amp; Miriam McCoy College of Business Administration, Texas State University</p>
    </li>
  </ul>
</section>

<section class="section">
  <div class="section-head">
    <h2>Research and Employment Background</h2>
  </div>
  <ul class="timeline">
    <li>
      <p class="eyebrow">2025-2026</p>
      <h3>Graduate Research Assistant, Enterprise Technology on AI and Accessibility</h3>
      <p><strong>Supervisor:</strong> Mario Guerra</p>
      <p><strong>Summary:</strong> Assisting the Enterprise Technology team and experimenting with and deploying AI solutions to solve digital accessibility problems across the university.</p>
    </li>
    <li>
      <p class="eyebrow">2024-2025</p>
      <h3>Teaching Assistant, Capstone Course (INF 388L)</h3>
      <p><strong>Supervisor:</strong> Dr. John Neumann</p>
      <p><strong>Funded by:</strong> The School of Information</p>
      <p><strong>Summary:</strong> Grading and course communications for the iSchool capstone.</p>
    </li>
    <li>
      <p class="eyebrow">2023-2024</p>
      <h3>Teaching Assistant for Ethics in AI</h3>
      <p><strong>Supervisor:</strong> Dr. Ken Fleischmann</p>
      <p><strong>Funded by:</strong> Computer &amp; Data Science Online (CDSO)</p>
      <p><strong>Summary:</strong> Led the teaching support team; created a facilitation guide (Fall 2023); led Learning Facilitators (Spring 2024) to manage and grade the course.</p>
    </li>
    <li>
      <p class="eyebrow">2022-2023</p>
      <h3>IMLS LADDER Fellow for Training Future Faculty in Library, AI, and Data-Driven Education and Research (LADDER) Project</h3>
      <p><strong>Supervisors:</strong> Dr. Soo Young Rieh, Dr. Ken Fleischmann, and Dr. David Lankes</p>
      <p><strong>Funded by:</strong> The Institute of Museum and Library Services</p>
      <p><strong>Summary:</strong> Led development of an AI Discussion Group curriculum on AI's role in work and life; collaborated with school, academic, and public librarians.</p>
    </li>
    <li>
      <p class="eyebrow">Spring 2022</p>
      <h3>Assistant Instructor for Ethical Foundations for Informatics</h3>
      <p><strong>Supervisor:</strong> Dr. Ken Fleischmann</p>
      <p><strong>Funded by:</strong> iSchool, The University of Texas at Austin</p>
      <p><strong>Summary:</strong> Taught a discussion section for Ethical Foundations for Informatics.</p>
    </li>
    <li>
      <p class="eyebrow">Fall 2021</p>
      <h3>Assistant Instructor for Introduction to Informatics</h3>
      <p><strong>Supervisor:</strong> Dr. Craig Blaha</p>
      <p><strong>Funded by:</strong> iSchool, The University of Texas at Austin</p>
      <p><strong>Summary:</strong> Taught a discussion section for a course helped design in prior semesters.</p>
    </li>
    <li>
      <p class="eyebrow">Summer 2021</p>
      <h3>Graduate Research Assistant, Providing Equitable Access to Higher Education: The Role of Academic Libraries</h3>
      <p><strong>Supervisor:</strong> Dr. Ken Fleischmann</p>
      <p><strong>Funded by:</strong> Scott &amp; Vickie Reeve Endowed Fellowship, iSchool, The University of Texas at Austin</p>
      <p><strong>Summary:</strong> Conducted interviews with university librarians on accessibility of library materials.</p>
    </li>
    <li>
      <p class="eyebrow">2020-2021</p>
      <h3>Teaching Assistant, Introduction to Informatics</h3>
      <p><strong>Supervisor:</strong> Dr. Craig Blaha</p>
      <p><strong>Funded by:</strong> iSchool, The University of Texas at Austin</p>
      <p><strong>Summary:</strong> Supported Fall 2020 and Spring 2021 offerings; contributed to new course version.</p>
    </li>
    <li>
      <p class="eyebrow">2019-2020</p>
      <h3>Graduate Research Assistant, Microsoft Ability Initiative</h3>
      <p><strong>Supervisor:</strong> Dr. Kenneth R. Fleischmann</p>
      <p><strong>Funded by:</strong> Graduate School, The University of Texas at Austin</p>
      <p><strong>Summary:</strong> Studied how people with blindness/low vision experience visual information and feature needs in vision-to-language systems.</p>
    </li>
    <li>
      <p class="eyebrow">2017-2019</p>
      <h3>Computer Technician</h3>
      <p><strong>Funded by:</strong> College of Education, Texas State University</p>
      <p><strong>Summary:</strong> Managed computer labs, operating system troubleshooting, and resource monitoring.</p>
    </li>
    <li>
      <p class="eyebrow">2016-2019</p>
      <h3>Accessibility Technology &amp; Quality Assurance Consultant</h3>
      <p><strong>Funded by:</strong> Savvy Technology Solutions</p>
      <p><strong>Summary:</strong> Conducted accessibility reviews with a UX focus, defined test methods, created procedures, reported results, and recommended fixes.</p>
    </li>
  </ul>
</section>

<section class="section">
  <div class="section-head">
    <h2>Refereed Publications</h2>
  </div>
  <ul class="card-list">
    <li>
      <p>Day, J. R., &amp; Fleischmann, K. R. (2026). Academic libraries and accessibility: How academic librarians assist students with visual impairments in accessing academic reading materials. <em>The Journal of Academic Librarianship</em>, 52, 103238.</p>
    </li>
    <li>
      <p>Day, J. R., Fleischmann, K. R., Rieh, S.-Y., &amp; Choi, Y. (2023). Voice interfaces for library accessibility: Challenges identified by academic librarians. <em>Association for Information Science and Technology (ASIS&amp;T) Mid-Year (MY) Meeting</em>. Virtual. (Presentation, 6 pages)</p>
    </li>
    <li>
      <p>Day, J., &amp; Fleischmann, K. R. (2020). Serving the needs of students with disabilities: How academic librarians can collaborate with publishers and disability services offices. <em>Proceedings of the 83rd Annual Meeting of the Association for Information Science &amp; Technology</em>. Virtual. (Poster, 6 pages)</p>
    </li>
    <li>
      <p>Fleischmann, K. R., Greenberg, S. R., Gurari, D., Stangl, A., Verma, N., Day, J. R., Simons, R. N., &amp; Yeh, T. (2019). Good Systems: Ethical AI for CSCW. <em>22nd ACM Conference on Computer-Supported Cooperative Work (CSCW)</em>, Austin, TX. (Workshop, 7 pages)</p>
    </li>
  </ul>
</section>

<section class="section">
  <div class="section-head">
    <h2>Other Presentations</h2>
  </div>
  <ul class="card-list">
    <li>
      <p>Day, J. R. (2026). Responsible AI for Education: Student Panel. Panelist. <em>Responsible AI for Education 2026</em>, The University of Texas at Austin, Texas Union (Shirley Bird Perry Ballroom), Austin, TX. April 21, 2026.</p>
    </li>
    <li>
      <p>Day, J. R. (2026). Digital Accessibility: Infrastructure Rather Than Request. <em>ET Talk Podcast</em>, Episode 6. Hosted by Cole Camplese, Vice President of Technology and CIO, The University of Texas at Austin. February 10, 2026. <a href="https://www.youtube.com/watch?v=jIikJmAF1ts">View recording</a>.</p>
    </li>
    <li>
      <p>Day, J. R. (2026). From Broken PDFs to Instant Access: How ChatGPT Rebuilds the Research Workflow at UT Austin. <em>OpenAI Academy</em>. April 1, 2026. <a href="https://academy.openai.com/public/blogs/from-broken-pdfs-to-instant-access-how-chatgpt-rebuilds-the-research-workflow-at-ut-austin-2026-04-01">Read feature</a>.</p>
    </li>
    <li>
      <p>Day, J. R. (2024). Accessibility of Academic Reading Materials: Insights from Librarians, Students, and Disability Services. <em>ALISE 2024</em>. October 14-17, 2024. Virtual.</p>
    </li>
    <li>
      <p>Day, J. R., &amp; Burns, S. (2021). Universal usability. <em>Open Texas 2021</em>. March 12, 2021. Virtual.</p>
    </li>
    <li>
      <p>Day, J. R., &amp; Burns, S. (2019). 3rd Annual Accessibility Hackathon. School of Information, The University of Texas at Austin. November 15, 2019.</p>
    </li>
  </ul>
</section>

<section class="section grid two-up">
  <section class="panel">
    <h2>Fellowships and Awards</h2>
    <ul class="stack-list">
      <li>Scott &amp; Vickie Reeve Endowed Fellowship, iSchool, The University of Texas at Austin, 2020-2021, $11,864</li>
      <li>Provost's Fellowship Supplement, iSchool, The University of Texas at Austin, 2019-2023, $20,000</li>
      <li>Mentoring Fellowship, Graduate School, The University of Texas at Austin, 2019-2020, $42,000 (converted to GRAship due to state benefits limitations)</li>
      <li>Outstanding Undergraduate Student in Computer Information Systems &amp; Quantitative Analysis, 2017</li>
      <li>Dean's List, Fall 2013 and Fall 2016</li>
      <li>Texas Association for Education and Rehabilitation of the Blind and Visually Impaired, Student with a Visual Impairment Scholarship, 2014</li>
    </ul>
  </section>

  <section class="panel">
    <h2>Service, Memberships, and Activities</h2>
    <ul class="stack-list">
      <li>Research Associate, Digital Accessibility Center, The University of Texas at Austin, 2025-2026</li>
      <li>Undergraduate Studies Committee, iSchool, The University of Texas at Austin, 2020-2021</li>
      <li>Guest Speaker, INF 385T: Accessible User Experience, April 29, 2021</li>
      <li>Guest Speaker, INF 385T: Accessible User Experience, February 16, 2023</li>
      <li>Guest Speaker, INF 385C: HCI, April 13, 2023</li>
      <li>Attended National Federation of the Blind Convention, 2018</li>
      <li>National Society of Collegiate Scholars, 2017</li>
    </ul>
  </section>
</section>
