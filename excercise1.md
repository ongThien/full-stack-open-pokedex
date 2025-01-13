## [Question](https://fullstackopen.com/en/part11/introduction_to_ci_cd#exercise-11-1):
Think about a hypothetical situation where we have an application being worked on by a team of about 6 people. The application is in active development and will be released soon.

Let us assume that the application is coded with some other language than JavaScript/TypeScript, e.g. in Python, Java, or Ruby. You can freely pick the language. This might even be a language you do not know much yourself.

Write a short text, say 200-300 words, where you answer or discuss some of the points below. You can check the length with https://wordcounter.net/. Save your answer to the file named exercise1.md in the root of the repository that you shall create in exercise 11.2.

The points to discuss:
  - Some common steps in a CI setup include linting, testing, and building.
  - What are the specific tools for taking care of these steps in the ecosystem of the language you picked? You can search for the answers by Google.
  - What alternatives are there to set up the CI besides Jenkins and GitHub Actions? Again, you can ask Google!
  - Would this setup be better in a self-hosted or a cloud-based environment? Why? What information would you need to make that decision?


## Answer:
Assume the application is developed in Java.
- Linting: For Java, Checkstyle is a popular linting tool that helps enforce coding standards and detect potential errors in the codebase. Other options include PMD and FindBugs, which can also be used to analyze code quality and find common issues.

- Testing: Java projects commonly use JUnit for unit testing, with integration support from Mockito or Arquillian for mock objects and containerized testing. Additionally, SonarQube can be integrated into the CI pipeline to track code quality metrics, including test coverage.

- Building: For building the application, Apache Maven and Gradle are the primary build tools in the Java ecosystem. Maven is particularly known for its dependency management, while Gradle is preferred for more complex and performance-oriented builds.

Beyond Jenkins and GitHub Actions, other CI/CD tools include GitLab CI, CircleCI, and TravisCI. These platforms also offer integrations for Java, providing pipeline automation with support for testing, building, and deploying applications.

Regarding deployment environments, there are cloud-based CI setups (e.g., GitHub Actions, GitLab CI) and self-hosted CI setups (e.g., Jenkins). Deciding between the two depends on factors like cost, security requirements, and infrastructure control needs. Cloud-based CI offers scalability, low maintenance, and easy integration with other cloud services. A self-hosted setup may require more maintenance, but it offers flexibility in handling custom configurations.
