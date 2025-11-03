# Thoughtful Coding

Thoughtful Coding is an open-source, interactive platform for Computer Science
teachers to augment their lessons with best-practice, research-backed techniques.

---

![A demo of the Thoughtful Coding platform](/assets/images/section_debugging.png)

---

Thoughtful Coding is designed for...

- **CS Teachers** who want a free, customizable platform to host their own curriculum.
- **Students** who want to learn Python in a self-paced, exploratory way.
- **Contributors** who want to build and share curriculum with a community.

## Core Differentiators

The core differentiators between this project and other, existing teaching platforms
are:

- **Open Source:** Free to use, modify, and host. (GPL v3 License).
- **Pedagogy-First:** Built on PRIMM, Reflection (Journaling), and Active Learning.
- **"Functions First" Approach:** Introduces `def` early to teach abstraction and composition.
- **Customizable:** Easy to create, customize, and share your own lessons.
- **Powerful Tools:** Includes a step-by-step code debugger and Turtle graphics assessment.
- **Formative AI Feedback:** Uses AI to give students feedback *before* they submit,
  allowing them to reflect and iterate.

## Pedagogy

The platform is built around "Learning Sections" that test and reframe material:

- **[PRIMM](https://thoughtful-coding.github.io/python/lesson/00_intro/lessons/01_intro_integers#primm-strings-and-integers):** Students predict code output, run it, and reflect on the differences.
- **[Reflection](https://thoughtful-coding.github.io/python/lesson/02_strings/lessons/01_fstring_practice#fstrings-reflection):** Students journal on new topics and get iterative AI feedback.
- **[Debugging](https://thoughtful-coding.github.io/python/lesson/06_loops/lessons/02_loops_nesting#debug-nesting):**
- **[Testing](https://thoughtful-coding.github.io/python/lesson/06_loops/lessons/01_loops_challenges#octagon-test):** Students solve problems and get immediate feedback from I/O tests.
- Input/Output questions where students must "work backwards" to understand how inputs affect outputs
  - **[Prediction](https://thoughtful-coding.github.io/python/lesson/05_conditionals/lessons/03_cond_if_else#pass-fail-prediction)**
  - **[Coverage](https://thoughtful-coding.github.io/python/lesson/05_conditionals/lessons/05_cond_bool#ride-requirements)** 
- Various deterministic question types to target and correct common misconceptions.
  - **[Multiple Choice](https://thoughtful-coding.github.io/python/lesson/01_variables/lessons/03_var_wrap_up#variable-assignment)**
  - **[Multiple Selection](https://thoughtful-coding.github.io/python/lesson/01_variables/lessons/00_var_intro#variable-parts)**
  - **[Matching](https://thoughtful-coding.github.io/python/lesson/xx_learning/lessons/00_learning_primm#primm-matching)** 

---

## Thoughtful-Coding Architecture

The project can be broken down into three main pieces. All of these pieces can
either be used as is or cloned for greater instructor control. The pieces are:

### [Student Website](https://github.com/thoughtful-coding/thoughtful-coding.github.io)

A website that walks students through learning Python with an iterative, experimental
approach. The core of the website is a series of "learning sections" that allow the material
to be presented and tested in a variety of ways:

### [Instructor Back-End](https://github.com/thoughtful-coding/thoughtful-backend)

An easy to setup back-end (using AWS) that stores students progress, answers, reflections.
The server is front-end agnostic, meaning that the website can present _any_ type of
material and it will be stored without issues.

The server uses Google OAuth to map student's email addresses to their answers. Predicted
costs for running the server in a globally accessible environment is around 25-50 cents
per student.

### [Instructor Website](https://thoughtful-coding.github.io/python/instructor-dashboard)

A portal that allows instructors to track the progress of their students across various
dimensions. The portal provides easy access to high-level markers like "completion
percentage" of a particular unit/lesson but also the ability to dive deep and look at the
various iterations of a student's reflection prior to submitting it for grading.

## License

This project is licensed under the GNU General Public License v3.0.
