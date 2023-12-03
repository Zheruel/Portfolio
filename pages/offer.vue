<template>
  <div id="my-offer">
    <h1>My offer</h1>
    <p>
      As a seasoned
      <span class="highlight">full-stack software engineer</span> with over
      <span class="highlight">{{ dateDifference }} years of experience</span>,
      I've played a pivotal role in
      <span class="highlight">maintaining and developing</span> various
      projects, spearheading the development of both back-end and front-end
      codebases.
    </p>
    <p>
      My expertise spans a comprehensive range of responsibilities, making me
      your go-to professional for diverse project needs:
    </p>
    <ul>
      <li>
        <b>Full-stack Development:</b> I excel in crafting robust back-end and
        front-end solutions, ensuring seamless integration and optimal
        performance.
      </li>
      <li>
        <b>Leadership and Mentorship:</b> With a proven track record, I am adept
        at leading and mentoring teams, fostering an environment of
        collaboration and continuous improvement.
      </li>
      <li>
        <b>System Design & Architecture:</b> I bring a strategic approach to
        system design and architecture, ensuring scalability, flexibility, and
        adherence to best practices.
      </li>
      <li>
        <b>Database Design & Implementation:</b> My proficiency extends to
        crafting efficient and scalable database solutions, optimizing data
        storage and retrieval processes.
      </li>
      <li>
        <b>Technology Research:</b> I am committed to staying ahead of the curve
        by researching and implementing cutting-edge technologies, ensuring your
        project stays at the forefront of innovation.
      </li>
      <li>
        <b>Communication:</b> I understand the importance of clear communication
        with clients, translating technical details into understandable
        insights, and ensuring alignment with project goals.
      </li>
    </ul>
    <p>
      <i
        >Consider me your "Swiss Army Knife" for all your IT needs. I am
        dedicated to delivering not just solutions but excellence across the
        entire spectrum of software development.</i
      >
    </p>

    <hr />

    <h2>Technologies</h2>
    <p>
      <b>Front-end:</b>
      HTML/CSS, JavaScript, TypeScript, jQuery, Angular, Vue, Nuxt, React, Next
    </p>
    <p>
      <b>Back-end/desktop:</b>
      C, C++, C#, .NET, Python, Django, Node, PHP, AWS Serverless
    </p>
    <p>
      <b>Database:</b>
      both SQL and NoSQL, (MySQL, PostgreSQL, MongoDB, DynamoDB, etc.)
    </p>
    <p>
      <b>Other:</b>
      System Design & Architecture, Git, Postman, AWS, NewRelic, Jira,
      Confluence, Agile, Scrum, Kanban, etc.
    </p>

    <p>
      In my journey as a full-stack software engineer, I've not just accumulated
      a diverse skill set across various technologies but cultivated a mindset
      of perpetual learning. Adapting to new technologies swiftly is second
      nature to me; I find that the lessons from one realm often serve as
      accelerators in mastering others, consistently trimming down the learning
      curve.
    </p>
    <p>
      I view life as an ongoing learning process, and each project is an
      opportunity for growth. My commitment to continuous improvement ensures
      that the projects I undertake witness not just development but a steady
      and consistent progression towards success.
    </p>

    <hr />

    <p>
      Recognizing that mastery in every aspect is a lofty goal, I embrace
      specialization. If the design realm seems better suited for another
      expert, feel free to delegate – I'll take charge of the entire code
      development or any role where my strengths can be leveraged best.
    </p>
    <p>
      Even if your team is already in place, and you're seeking that extra
      boost, consider me your adaptable ally. I assure you a seamless fit into
      your existing dynamics, swiftly contributing my skills and insights to
      propel your project forward.
    </p>
    <p>
      Let's tackle your unique challenges
      <NuxtLink class="highlight" to="/contact"> together</NuxtLink>
      .
    </p>
  </div>
</template>

<script setup>
const dateDifference = new Date().getFullYear() - 2018;
</script>

<style scoped>
h1 {
  margin: 0;
  text-transform: uppercase;
  font-weight: 400;
  font-size: 30px;
}

h2 {
  text-transform: uppercase;
  font-weight: 400;
  font-size: 26px;
}

p {
  color: #555;
}

li {
  margin-bottom: 8px;
}

.highlight {
  font-weight: bold;
  color: #40748a;
}

#my-offer {
  padding: 50px;
  max-width: 850px;
  background-color: white;
  color: #555;

  @media screen and (max-width: 1024px) {
    padding: 30px 20px;
  }
}
</style>
