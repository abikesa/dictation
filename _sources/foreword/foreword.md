(fw)=
# Available Resources for Developers

## The Content
That's an excellent approach. You're creating a comprehensive resource that combines educational content with interactive tools for patients. Here's a breakdown of how your current structure supports this goal:

1. Educational Content:
   - The Markdown files (chapter1.md, chapter2.md, chapter3.md, intro.md, index.md) likely contain the main educational content for patients.
   - The Jupyter notebook (chapter2.ipynb) allows for interactive explanations, potentially with code examples or data visualizations.

2. Interactive App:
   - The `app` directory houses your interactive application.
   - `risk.html` is probably the main page for your interactive tool.
   - The `assets` folder contains the necessary CSS (style.css) and JavaScript (script.js) to make your app functional and visually appealing.

3. Jupyter Book Structure:
   - `_config.yml` and `_toc.yml` are used by Jupyter Book to configure the project and define the table of contents.
   - The `_build` directory is where Jupyter Book will generate the final output.

4. Additional Resources:
   - `references.bib` can be used to manage citations and create a bibliography for your educational content.
   - `README.md` likely contains information about the project, how to set it up, or how to use it.
   - `requirements.txt` lists the Python dependencies for your project.

This structure allows you to create a seamless experience where patients can read through educational material and then interact with an app that helps them apply what they've learned. It's a powerful way to combine information delivery with practical application.

If you're looking to expand or improve this setup, you might consider:

1. Adding more interactive elements within the Jupyter notebooks.
2. Ensuring your app is accessible and easy to use for patients with varying levels of technical skill.
3. Incorporating patient feedback mechanisms to continuously improve both the educational content and the interactive app.

Is there any specific aspect of this project you'd like to discuss further or need assistance with?

## Your Feedback
Incorporating feedback into your project is an excellent way to improve its effectiveness and user experience. Here are several approaches you could consider:

1. In-app feedback mechanism:
   - Add a feedback form or button within your interactive app (risk.html).
   - Use JavaScript to capture user input and store it locally or send it to a server.

2. Comment system in Jupyter Book:
   - Jupyter Book supports adding comments to pages using services like Hypothes.is or Utterances.
   - This allows readers to leave feedback directly on specific content.

3. Surveys:
   - Create periodic surveys using tools like Google Forms or SurveyMonkey.
   - Link to these surveys from your Jupyter Book pages or app.

4. User testing sessions:
   - Conduct structured user testing sessions with patients.
   - Observe how they interact with your content and app, noting any difficulties or suggestions.

5. Analytics:
   - Implement web analytics (e.g., Google Analytics) to track user behavior.
   - This can provide insights into which content is most viewed or where users might be struggling.

6. Email feedback:
   - Provide an email address for users to send detailed feedback or questions.

7. Interactive elements:
   - Add quick reaction buttons (e.g., "Was this helpful?") at the end of each chapter.
   - Use JavaScript to capture these reactions.

8. GitHub Issues:
   - If your project is open-source, encourage users to submit issues or feature requests via GitHub.

To implement these, you might need to:

1. Modify your `risk.html` to include feedback forms or buttons.
2. Update `script.js` to handle feedback submission.
3. Add necessary configurations to `_config.yml` for comment systems.
4. Create new HTML/JS files for more complex feedback mechanisms.
5. Set up a backend system to receive and store feedback (this might require additional server-side code).

Remember to consider data privacy and security when collecting user feedback, especially in a healthcare context. Always be clear about how you'll use the feedback and protect user information.

Would you like more detailed information on implementing any of these feedback methods?

```{note}
This section has been recently added, and some chapters are still being reviewed by the project delivery team and community members. If you notice any error, please raise an issue on our GitHub repository.
```

<iframe src="app/risk.html" width="100%" height="600px" style="borders:none"></iframe>

You will find these details in the following chapters:

- {ref}`fw-background`
- {ref}`fw-navigating`
- {ref}`fw-emergent-strategy`
- {ref}`fw-embracing-digital-commons`
- {ref}`fw-community`
- {ref}`fw-governance`
- {ref}`fw-cite`
- {ref}`fw-faqs`

```{figure} https://www.tmc.edu/news/wp-content/uploads/sites/2/2019/08/kidney-copy.jpg
---
width: 500px
name: banner-welcome
alt: Two people, a woman and a man, waving next to a banner that says - welcome.
---
*Frank, 84yo: The Oldest Living Donor as of 2019* source: [Houston Methodist](https://www.tmc.edu/news/2019/05/an-84-year-old-man-becomes-oldest-living-kidney-donor-in-the-united-states-at-houston-methodist-hospital/) 

*But there's an update to this* [BMC Geriatr. 2022; 22: 826, Published online 2022 Oct 27. doi: 10.1186/s12877-022-03511-8](10.1186/s12877-022-03511-8)
```

We hope these resources will help you navigate, understand and be part of our community.

<iframe src="https://abikesa.github.io/music/_downloads/270ce1dc688a64dec497dfe81d0966aa/mozart.pdf"></iframe>
<iframe src="https://abikesa.github.io/music/_downloads/a207eb5446aa5d171a0ba97791498e49/bach.pdf"></iframe>
<iframe src="https://abikesa.github.io/music/_downloads/f1747777a15dcc72b5adef6cfcae8d8e/handel.pdf"></iframe>